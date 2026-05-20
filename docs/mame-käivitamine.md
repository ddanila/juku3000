# Running JUKU in the MAME emulator

Starting with [MAME version 0.272](https://github.com/mamedev/mame/releases/tag/mame0272), JUKU is in the venerable list of working abandonware[^1] and you can get Estonia's legendary school computer running on your desktop without much fuss (the web version, for trying it out, is [here](https://infoaed.ee/juku/)). To do so:

1. Download [the desktop version of the MAME emulator](https://www.mamedev.org/release.html)
2. Place [the JUKU firmware ZIP](https://github.com/infoaed/juku3000/raw/refs/heads/master/roms/juku.zip) into the downloaded MAME's `roms` directory
3. Launch MAME, choose JUKU E5104 as the system and EKDOS 2.30
4. Confirm that JUKU starts with the default RomBios 3.43m firmware
5. After the system properties are displayed, power is applied to the rare specimen

The display shows the firmware monitor message `RomBios`, the monitor's version number, and the prompt `∗`, after which the input cursor blinks invitingly:

[![Booting EKDOS 2.30 from the firmware monitor Rombios 3.43m with the control keys «T», «D», «D»](/images/jukubuut.gif)](https://commons.wikimedia.org/wiki/File:Juku_E5101_booting_up_EKDOS_2.30,_displaying_readme_file_on_screen.webm)

To boot the JUKU E5104 operating system EKDOS, press `T`, `D`, `D`; more detailed operating-system instructions can be [found here](juku-k%C3%A4sud.md).

## Running software

But what good is an operating system without software? JUKU's [3](https://elektroonikamuuseum.ee/juku_arvuti_tarkvara.html)+[1](ekdos230.md) system discs with their software are available from MAME's software list starting with version 0.274; historical floppies can be found in the Museum of Electronics' [JUKU file archive](https://elektroonikamuuseum.ee/failid/juku/tarkvara/), and most of the software is described in the [catalog](tarkvara-kataloog.md).

To use a floppy disc, it must be inserted into the emulated JUKU. For that you first need to unlock MAME's system keys using `Scroll Lock` (also known as `MAME Lock`), after which you can open [MAME's system menu](https://docs.mamedev.org/usingmame/mamemenus.html) by pressing `Tab`.

Floppies, i.e. `JUK` files, can be added under `File Manager`, and by default you can choose between various JUKU system discs from MAME's software list (_software list_) — more software and games can be found in the `JUKGAME`/`JUKPROG` series. To mark the emulator being ready, we also released the [JUKU 3000 games disc 2024](mängude-ketas-2024.md), which captures the state of the [`GAME1.JUK`](https://infoaed.ee/juku/game1.juk) disc of the November 2024 web emulator. JUKU-era image material and user programs can be found on the web emulator's [`PROG1.JUK`](https://infoaed.ee/juku/prog1.juk) disc.

MAME floppy menu | Games disc 2024
:-------------------------:|:-------------------------:
[![After pressing Scroll Lock (also known as MAME Lock) you can open MAME's floppy menu with TAB](/images/mame-flopimenyy.png)](https://docs.mamedev.org/usingmame/mamemenus.html)  |  [![To mark the emulator's release, the Juku 3000 games disc 2024 was published](/images/j3k-games2024f.png)](mängude-ketas-2024.md)

You can switch the active disc in EKDOS by typing the drive letter and a colon after the prompt (e.g. `A:` or `B:`); software, i.e. `COM` executables, can be launched by typing the desired program name after the prompt. The command `DIR` shows the list of files on the disc. To check that the system is working, you can try whether you can launch [the well-known JUKU game INDY](https://et.wikipedia.org/wiki/Indy_looking_for_Jewels...) from the `GAME1.JUK` disc.

In general, the first sensible thing to do in MAME for JUKU is to disable all _bilinear filtering_ settings, which suit blurrier TV-game pictures but not a school computer (e.g. under `General Settings` -> `Video Options` — don't forget to choose `Save Settings` from the main menu afterwards).

* If you record screen videos of JUKU games or software, then [do them correctly](videod.md)!
* If you want to create your own JUKU disc images, here's the [technical guide](kettad.md)!

If you want to try programming on JUKU, you can leaf through the [slides on the JUKU software ecosystem](https://p6drad-teel.net/~p6der/juku-hingeelu_2024_videota.pdf) and then try the consolidated compilers/linkers disc [`TERE.JUK`](https://github.com/infoaed/juku3000/raw/refs/heads/master/src/juhan/tere.juk).

[^1]: _He who does not remember the past lives without a future!_ — Juhan Liiv
