# Recording JUKU videos correctly

The main thing is to choose an integer multiple of the JUKU's resolution when recording screen videos, so the result is authentic. Since JUKU's default resolution is 320x240, the possible resolutions are:

* 640x480
* 960x720
* 1280x960
* 1600x1200
* ...

If a JUKU program uses a non-default resolution (e.g. 384x200, 400x192, 256x192, etc.), you should naturally pick an integer multiple of that.

When [using MAME's built-in screen video recording](https://docs.mamedev.org/usingmame/defaultkeys.html) (Scroll Lock -> Left Control+Left Shift+F12), the easiest approach is to set the [recording parameters](https://docs.mamedev.org/commandline/commandline-all.html#mame-commandline-snapsize) from the command line, e.g. `-snapsize 960x720` together with `-nosnapbilinear`, because we want to preserve the video's pixel structure and don't want blurred edges on fonts/graphics (the same setting is in the UI under `General Settings` -> `Advanced Options` -> `Bilinear filtering for snapshots`).

Crisp JUKU&nbsp;&nbsp;&nbsp; |  Blurry JUKU
:-------------------------:|:-------------------------:
![image](https://github.com/user-attachments/assets/a42086ab-e781-4b09-97e4-03299d99d6cf) | ![image](https://github.com/user-attachments/assets/6b213717-2d28-4402-a6c8-f7f3d53d3cac)

For performance reasons it may still be wise to stick with `-snapsize auto`, leave the video unscaled, and archive it in its native resolution. The video can then be converted to whatever resolution you need for display, e.g. [using FFmpeg](http://trac.ffmpeg.org/wiki/Scaling#Specifyingscalingalgorithm):

```
ffmpeg -i mame_original.avi -vf scale=960:720 -sws_flags neighbor exported_video.mp4
```

The FFmpeg flag `-sws_flags neighbor` disables blurring filters during scaling, the same as MAME's `-nosnapbilinear`. Depending on how the video will be used, you may need to add other parameters — for instance Twitter/X requires videos to be in a specific colour mode `-pix_fmt yuv420p`. You can also have FFmpeg multiply the dimensions itself; for variety, here's a command line for scaling screenshots:

```
ffmpeg -i mame_screenshot.png -vf scale=iw*4:ih*4 -sws_flags neighbor -update 1 exported_image.png
```

Most serious tools probably have similar options, but using MAME's own facilities is the most reliable approach — and for cases that need especially good performance, you can also use [`record` and `playback`](https://docs.mamedev.org/commandline/commandline-all.html#core-state-playback-options).
