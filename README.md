![JUKU 3000](https://raw.githubusercontent.com/infoaed/juku3000/master/images/juku3000.jpg)
# What is juku3000?

**Our goal is to let future generations vividly experience the early history of Estonian computing — the legendary 1990s school computer JUKU must remain usable even in the year 3000!**

If you don't know what JUKU is, it's time to take a look at [Wikipedia](https://et.wikipedia.org/wiki/Juku_(arvuti)), the [Estonian Museum of Electronics](https://elektroonikamuuseum.ee/juku_arvuti_lugu.html), or to get acquainted with our [JUKU timeline](docs/ajajoon.md).

This site's content of general interest is available at [j3k.infoaed.ee](https://j3k.infoaed.ee/); the source-code directory also contains [some interesting test programs](src).

Although thousands of physical JUKUs were produced in the 1990s, today it is easier to experience JUKU through an emulator running on [an ordinary computer](dos/mame-käivitamine.md) or even in [a web browser](https://infoaed.ee/juku):

* [MAME](docs/mame-käivitamine.md) is the gold standard of JUKU emulation, which can also be [tried in a browser](https://infoaed.ee/juku) (the keyboard layout is [here](https://infoaed.ee/juku/layout.html) and the RomBios 3.43m/JBASIC 1.1 firmware needed to start it up is [here](roms))
* [Универсальный эмулятор](http://bashkiria-2m.narod.ru/index/fajly/0-11) (emulates about 80% of both [Juku](https://et.wikipedia.org/wiki/Juku_(arvuti)) and [Iskra 1080 Tartu](https://et.wikipedia.org/wiki/Tartu_(arvuti)); config files are extendable, audio and disk support can be configured if needed, but JUKU's additional graphics and text modes are missing; closed source — generally we recommend MAME for emulation, but this emulator together with its debugger and settings is good comparative material)
* [EMU80](https://github.com/vpyk/emu80v4) (a lightweight open-source candidate that can be adapted to emulate Juku and other chips from the same family)
* [PCjs Project](https://www.pcjs.org/) contains the [beginnings](https://github.com/jeffpar/pcjs/tree/master/machines/pcx80/juku) of JUKU emulation

A selection of short guides:

* [Running the JUKU E5104 operating system](docs/juku-k%C3%A4sud.md)
* [Recording JUKU videos correctly](docs/videod.md)
* [Reading/writing JUKU disks with libdsk/cpmtools](docs/kettad.md)

JUKU's operating system EKDOS:

* [EKDOS 2.30](https://p6drad-teel.net/~p6der/ekdos230.zip) (released December 1989, [announcement](docs/ekdos230.txt))
  * [Source code](src/EKDOS30.ASM), cf. CP/M 2.2 [adaptation guide from Digital Research](http://www.gaby.de/cpm/manuals/archive/cpm22htm/ch6.htm)
* [EKDOS 2.29](https://p6drad-teel.net/~p6der/ekdos229.zip) (released 05.01.1988)

## How the project came to be

> What follows was originally a hackathon project, documented below — by now there is the [LVLup museum](https://et.wikipedia.org/wiki/LVLup) and computer museums in [Tallinn](https://et.wikipedia.org/wiki/Arvutimuuseum) and [at the Institute of Computer Science of the University of Tartu](https://et.wikipedia.org/wiki/Tartu_%C3%9Clikooli_arvutimuuseum), whose cooperation could realise this kind of effort. Historical text follows...

### Experiences and Expositions 22.09–24.09 2017

Museums would like to put on exhibitions of Jukus, ZX Spectrums, Ataris, Amigas, Commodores, Iskras, Yamahas, Tartus, Entels and so on together with the era's software/games — but there is one big problem: if visitors are also allowed to touch these computers, then the unique pieces tend to break. But what's the point of computers if you can't touch them?

The solution is to build a computer system out of modern components that offers a user experience similar to those old computers, but is intuitive enough and idiot-proof enough for modern users that hordes of schoolchildren could troop through it daily.

### Team members

* (names removed)

## What's needed for this?

* Emulators, lots of emulators. Emulating JUKU's EKDOS with all its interfaces is not a one-evening project, but for most old widely-used platforms emulators already exist. We can use those.
* Software, lots of software stuck on hard disks, floppies, cassettes and tapes — especially software that was adapted, hacked or even produced by the locals for local use. Do you have software that won't run on any known modern computer system? Did you write computer games in the 1990s yourself? Send them to us, we'll figure out how to breathe life into them.
* A hardware set with an old-school CRT monitor, archaic-looking sturdy keyboard, and the legendary control device — the joystick!
* A user-interface top layer that lets you choose between different emulators and their games.
* A museum layer that lets you get to know the cultural and technological foundations of the early history of computer games. Night watch in the computing centre? The game room on Kalevi Street? The key to the school's Juku class? Zero-day cracks from Dutch BBSes via a 2600-baud modem on Estonian Telephone's dime? BBSummer and ee.kevad? Mudplayer socks on the keyboard of an ATI terminal? All this ethnographic material deserves to be collected and told to future generations.

## How do we get there?

The first step is taken on 22–24 September 2017 at the Garage48 hackathon in Tartu, ["Experiences and Expositions"](http://garage48.org/events/garage48-elamused-ja-ekspositsioonid). If you're interested, want to give advice, contribute, or simply share your memories, get in touch at tramm@infoaed.ee or +372 55643754 — it helps us if you can drop by the hackathon just to chat with us on this topic, but even better if you join our team to create a prototype that could find use in a real museum at real exhibitions. We plan to hold a pilot exhibition already in early November, when ERM hosts a conference focused on contemporary digital museum work, ["Open licences, open content, open data: tools for developing digital humanities"](http://dh.org.ee/category/events/dhe2017/), where Outi Penninkangas — a key figure of Finland's first computer game museum — will also speak.
