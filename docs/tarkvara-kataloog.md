# General list of JUKU software recovered from disks

This catalog lists JUKU E5101–E5104 software recovered from disks,
tapes and ROM chips, as of March 2026. New material is added over
time and the descriptions may change as more becomes known. The
authoritative checksummed version of the list is:

* https://j3k.infoaed.ee/tarkvara-kataloog.txt

The same location also has checksum-free conversions to PDF and Markdown.
Most of the material can be downloaded from:

* https://elektroonikamuuseum.ee/failid/juku/tarkvara/

User sections are numbered starting from 1; deleted files are
in the `E5` section. For partially recovered disks, 0/0 marks the
number of bad sectors on each side of the disk — e.g. 0/32 means
32 bad sectors on the second side of the disk.

## CASTOOLS

A floppy donated to the University of Tartu Computer Museum, containing a manually
and automatically controlled tape OS (MTOS/ATOS, LOS) bootable from an audio cassette,
together with its tools — see https://github.com/UT-Arvutimuuseum/juku-kassett for details.
The disk has a version of EKDOS 2.29 that differs from Baltijets's `EMUSYS` 1–3 series.

SIZE: `800K` (`819200`) / SHA1: `8dbd941ee6241ab40ff012a8ecd83328cf24d9b9`

``ATOS    .SYS   5,0K``    Automatic LOS, i.e. ATOS 7.0 (EKTA '88)  
``CF      .COM   1,0K``    File copy 1.0 (EKTA '89)  
``CF      .HLP   1,5K``    CF quick guide  
``COPA    .COM   6,0K``    COPY 3.0 for ATOS  
``COPM    .COM   4,8K``    COPY 2.0 for MTOS  
``EDIT    .COM   9,0K``    LOS EDIT 2.1 (EKTA '88?)  
``FORM    .COM   5,9K``    FORMAT 3.0 for ATOS  
``GENA    .COM   3,4K``    LSYSGEN 2.0 for ATOS  
``GENM    .COM   2,8K``    LSYSGEN 2.0 for MTOS  
``KOLL    .COM    18K``    Tape copying 1.0 (EKTA '89)  
``KOLL    .HLP   7,5K``    Tape/floppy copying guide  
``MAKK    .HLP    10K``    Tape OS tools guide  
``MTOS    .SYS   3,5K``    Manual LOS, i.e. MTOS 2.0 (EKTA '88)  
``SETS    .COM   1,4K``    Set file(s) status (SETS \*.* $r/o)  
``TCOPY   .COM   2,7K``    Tape-to-tape copying  

## EMUSYS1

Baltijets JUKU E5104 system disk #1, distributed by the Museum of Electronics,
see https://elektroonikamuuseum.ee/juku_arvuti_tarkvara_susteemiketas_1.html;
matches the `MUSEUM01` disk. The OS on the disk is EKDOS 2.29.

SIZE: `800K` (`819200`) / SHA1: `956c82e43e2b1f76a337190f78318428729e845f`

``ASM     .COM   8,0K``    Assembler 2.0 (CP/M)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BASCOM  .COM    32K``    BASIC compiler 5.30 (Microsoft)  
``BASLIB  .REL    49K``      
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``CM6329  .COM   1,8K``    Robotron CM6329 printer driver  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``CPU     .COM    19K``    Microprocessor Test 1.2 (EKTA '85)  
``D100M   .COM   1,4K``    D100M printer driver (EKTA '91)  
``DIAG    .LOG      0``      
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``DUMP    .COM    512``    File dump 1.4  
``ED      .COM   6,5K``    Context editor (CP/M)  
``F80     .COM    27K``    FORTRAN-80 v3.44 (Microsoft '81)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``FMT     .COM   1,3K``    EKDOS 386K floppy formatter 3.4  
``FORLIB  .REL    26K``      
``FORMAT  .COM   1,3K``    EKDOS 786K floppy formatter 3.4  
``FX800   .COM   1,8K``    Epson FX-800 printer driver  
``I       .       128``      
``JBASIC  .COM   8,2K``    BASIC interpreter 1.1 (EKTA '87)  
``KUVA    .COM    768``    Screen centering 1.1 (K.Kevvai)  
``L80     .COM    11K``    LINK-80 3.44 (Microsoft '81)  
``LOAD    .COM   1,8K``    HEX to COM converter (CP/M)  
``MODE    .COM    256``    40x24, 53x24 and 64x20 switch  
``MTEST2  .COM   9,5K``    Memory Test 0100-14FF (EKTA '85)  
``MTEST   .COM   4,5K``    Memory Test 1500-FFFF (EKTA '85)  
``NETD    .COM   7,4K``    Janet 1.0 14/11/00 (EKTA)  
``NETR    .COM   6,5K``    N-EKDOS 1.0 (EKTA)  
``PIP     .COM   7,3K``    File copier (CP/M)  
``QDISK   .COM   7,2K``    Disk Test (EKTA '85)  
``QRUN    .COM   4,8K``    Quick Test (EKTA '85)  
``RDEM    .COM    30K``    JUKU official demo program (EKTA '87)  
``SED     .COM    10K``    Screen text editor 6.1  
``SID     .COM   7,0K``    Machine-code debugger SID 1.4 (CP/M)  
``STAT    .COM   5,2K``    Filesystem statistics (CP/M)  
``SUBMIT  .COM   1,3K``    Command-batch processor (CP/M)  
``TERM    .COM   9,5K``    Terminal Demo/Test 1.2 (EKTA '85)  
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  

## EMUSYS2

Baltijets JUKU E5104 system disk #2, distributed by the Museum of Electronics,
see https://elektroonikamuuseum.ee/juku_arvuti_tarkvara_susteemiketas_2.html;
matches the `MUSEUM02` disk. The OS on the disk is EKDOS 2.29.

SIZE: `800K` (`819200`) / SHA1: `054b854a9bc58383794e74fdc2f778f746bdf55d`

``FPREALS .ERL   7,5K``      
``LINKMT  .COM    12K``    Link/MT+ v5.6.1  
``MTERRS  .TXT   4,8K``      
``MTPLUS  .000    13K``      
``MTPLUS  .001    11K``      
``MTPLUS  .002   7,0K``      
``MTPLUS  .003   7,3K``      
``MTPLUS  .004    17K``      
``MTPLUS  .005   8,5K``      
``MTPLUS  .006   6,2K``      
``MTPLUS  .COM    36K``    Pascal/MT+ v5.6.1  
``PASLIB  .ERL    25K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``TRANCEND.ERL   3,3K``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  

## EMUSYS3

Baltijets JUKU E5104 system disk #3, distributed by the Museum of Electronics,
see https://elektroonikamuuseum.ee/juku_arvuti_tarkvara_susteemiketas_3.html;
matches the `MUSEUM03` disk. The OS on the disk is EKDOS 2.29.

SIZE: `800K` (`819200`) / SHA1: `2bd379212078b892ad07766007507b02bbda3703`

``DBASE   .COM    19K``    dBASE II v2.4  
``DBASEMSG.TXT    52K``      
``DBASEOVR.COM    40K``      
``DBINST  .COM    14K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``INSTALL .COM   6,4K``    Microsoft tools config 1.02 ('81)  
``INSTALL .DAT    21K``      
``INSTALL .MSG    12K``      
``INSTALL .OVR    30K``      
``INSTALL .SPC    256``      
``MP40    .      6,3K``      
``MP80    .      6,3K``      
``MP      .COM    17K``    Multiplan 1.05 (Microsoft '81)  
``MP      .HLP    40K``      
``MP      .OVR    43K``      
``PATTERN .PIC   7,2K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  

## HEIKITAPE

A JUKU storage medium in the form of an audio cassette, labelled `TAPE -HEIKI-`,
which the Museum of Electronics' founder Woldemar converted into an audio file
in 2023. The Audacity `AUP3` file contains 31 minutes 33 seconds of two-channel
audio recorded as 44100 Hz 32-bit floating-point samples, originating from the
first side of the audio cassette. The data is preceded by about a minute of
music by the band Boney M; the first side of the cassette is labelled `FOR -JUKU-`
`ROM 2.42` and `=BASIC-80=`; the second side was empty. The cassette was produced
at the Tallinn audio-cassette factory, the magnetic tape type is marked `Fe`,
and the tape appears to have originally contained the "Choral Festival Tallinn '88"
material.

SIZE: `422M` (`442472368`) / SHA1: `413897f282b622658e40932e0874143c3df6e0b5`

``B80T    .COM    24K``    BASIC-80 5.21/TAPE (Microsoft '81)  
``SAL     .BAS   2,0K``    Program "Archaeologist's joy" ('88)  
``TAR     .DAT    14K``      
``TART    .DAT   6,0K``      
``TARTU1  .DAT   4,0K``      
``TARTU2  .DAT   8,0K``      
``TARTU3  .DAT    16K``      
``TARTU4  .DAT    16K``      
``TARTU   .DAT   4,0K``      
``T@@     .BAS   4,0K``      
``T@@T    .BAS   4,0K``    "Archaeologist's joy" data processing  
``VAD     .DAT    10K``      
``VADJA3  .DAT   6,0K``      
``VADJA4  .DAT    14K``      
``VADJA5  .DAT    14K``      
``VADJA   .DAT   8,0K``      
``VIL     .DAT   2,0K``      
``V@RU1   .DAT    10K``      
``V`RU2   .DAT    12K``      
``V`RU    .DAT    10K``      

## INDY

For the occasion of BBSummer 2022, Ilmar Käär and Rauno Mägi released their 1991
masterpiece "Indiana Jones Looking For Jewels..." into the public domain for
historical-research purposes under the Creative Commons Zero (CC0) licence. The
game was published in the "Filez" section of Matrix BBS.

SIZE: `36K` (`36437`) / SHA1: `8905d0a3601928b4890da92e7187f1e3bb7a7df5`

``FILE_ID .DIZ    297``      
``GAME    .PNG   4,9K``      
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``INDY    .DAT    12K``      
``MENU    .PNG   3,7K``      
``README  .TXT   1,7K``      
``TITLE   .PNG   3,8K``      

## J3KGAME1

The Juku 3000 games disc 2024, with which the arrival of school-computer support
in the MAME emulator (from version 0.272) was celebrated on 23 December 2024.
The disc contains a selection of games that were used to test the emulator, or
that simply made developing the emulator more fun; some of these games have not
been published in their entirety on other JUKU disks. The disc can be downloaded
from https://elektroonikamuuseum.ee/failid/juku/tarkvara/J3KGAME1.JUK.

SIZE: `800K` (`819200`) / SHA1: `4c864901be28e2d075ad9c73040003ce2a1ca069`

``1       .       896``    LAOLEO data file  
``2       .       896``    LAOLEO data file  
``2048    .COM   1,5K``    Puzzle game "2048" (Pehka1985 '22)  
``3       .       896``    LAOLEO data file  
``4       .       896``    LAOLEO data file  
``5       .       896``    LAOLEO data file  
``9       .COM   8,8K``    Puzzle game "9-VANGLA"  
``ATSKOO  .COM    18K``    Card game "Atskoo" (Kohtla-J 1KK)  
``AVTEST  .COM    14K``    Magic squares (=Sudoku, VSW '91)  
``AVTEST  .DOC   2,7K``    AVTEST foreword (V.Sinijärv '91)  
``BOWLING .COM   3,4K``    Bowling (Maxway & I.K.S. '91)  
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``BUGABOO .COM    18K``    Turnip in the maze\* (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``    Modified arrow keys (J3K/EMU '24)  
``BUGABOO .TAB    256``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``CHESS   .COM   8,0K``    Chess "I think & move" 1.1 (T.Ainsaar?)  
``GAMEBOY .COM    23K``    Fly and shoot (A.Säde '91)  
``GAMEBOY .DAT    512``      
``GAMEBOY .Z79   6,0K``      
``GAMEBOY .Z80   4,2K``      
``GAMEBOY .Z81   2,9K``      
``HITCH   .COM   8,7K``    Hitchhiker's guide (80x24, IC '85)  
``HITCHHIK.DAT   111K``      
``HUNTER  .COM   6,8K``    Hunting club (80x24, Vakstu/MIG '86)  
``HUNTER  .DAT    256``      
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``INDY    .DAT    12K``      
``INDY    .TXT   1,7K``    INDY foreword (I.Käär/R.Mägi '22)  
``KAPTEN  .COM    32K``    "Battleship" (ed K.Koppel)  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``LL0     .      6,4K``    LAOLEO data file  
``LOGER   .COM    32K``    Switch logic v1.1 (Nost Neji '90 H)  
``LOGEX1  .CLG    128``    LOGER data file  
``MADUOK  .COM   9,3K``    Classic snake game (=Snake)  
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MOIS    .COM   6,8K``    Manor lord's efficiency (=Sumerian)  
``MOND    .COM    17K``    Launch angle (=Artillery Duel)  
``PUSHER  .COM    23K``    "Pusher" (=Sokoban, A.Mett '91)  
``PUSHER  .DOK   1,3K``    PUSHER foreword (A.Mett '90)  
``PUSHER  .LEV   6,3K``      
``READ    .ME    2,3K``    Brief intro to the J3K games disc '24  
``SHOT    .COM   2,3K``    "Shot Master 2000" v1.1 (I.Käär '91)  
``SHOT    .DAT   9,0K``      
``SNAKE   .COM    12K``    "Snake"\* (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``SPACE   .COM    17K``    "Space Attack" (Vakstu/VSW '90)  
``ZOO     .COM    25K``    "Lode Runner" at the zoo\* (BROKEN!)  
``ZOO     .TXT    426``    ZOO foreword (ed J3K/EMU '24)  
``TANK    .COM    15K``    Tank vs. UFOs (=Sabotage/Invaders)  
``TET     .COM    17K``    "Tetris" with mouse (A.Mett '90 H)  
``TETRIS  .COM   1,9K``    Graphical "Tetris" (T.Ainsaar '90)  
``XONIX   .COM   3,8K``    "Xonix"\* (=Qix, E.Jürviste/EKTA '87)  
``YL1     .LOG    896``    LOGER task #1  
``YL2     .LOG    640``    LOGER task #2  
``YL3     .LOG    896``    LOGER task #3  
``YL4     .LOG   1,7K``    LOGER task #4  

## J3KGAME2

The Juku 3000 games disc 2025 is dedicated to ported games, of which probably
the first is XONIX and the most famous ZOO. The disc has a selection of abandonware
together with new versions; most of the fresh ports were done by Pehka1985, except
for the Hitchhiker's guide and Stupidity, which were ported by Tramm. The most
re-implemented games on JUKU are TETRIS and SOKOBAN — each rewritten 3x. The disc
is in use anno 2026 by the web emulator https://infoaed.ee/juku/ and can be
downloaded from https://elektroonikamuuseum.ee/failid/juku/tarkvara/J3KGAME2.JUK.

SIZE: `800K` (`819200`) / SHA1: `2e5703cf190f8e564bb1be844d5963711148e242`

``1       .       896``    LAOLEO data file  
``2       .       896``    LAOLEO data file  
``3       .       896``    LAOLEO data file  
``4       .       896``    LAOLEO data file  
``5       .       896``    LAOLEO data file  
``ARKANOID.COM    17K``    Arkanoid 1.0 (Brick '90/'25)  
``BINLAND .COM    30K``    Binary Land (Hudson '83/'24)  
``BOMB    .COM    12K``    Bomber Man (Hudson '83/'24)  
``BOULDER .COM    21K``    Boulder Dash (First Star '84/'25)  
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``CBALL   .COM   9,4K``    Cannon Ball (Hudson '83/'25)  
``CLRBALL .COM    10K``    Color Ball (Hudson '84/'25)  
``DIGGER  .COM   1,2K``    Viral star shower (K.Tomingas '91)  
``DTANK   .COM    14K``    Driller Tanks (Hudson '83/'24)  
``FIRE    .COM    17K``    Fire Rescue (Hudson '84/'25)  
``HITCH   .COM   8,7K``    Hitchhiker's guide (80x24, IC '85)  
``HITCHHIK.DAT   111K``      
``INDIAN  .COM    21K``    Indian no Bouken (Hudson '83/'25)  
``LAD     .       896``    Ladder graphics as a font table  
``LAD2    .DAT    512``    Modified arrow keys (J3K '25)  
``LADDER2 .COM    40K``    Platformer Ladder 2 (Yahoo '83)  
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``LF      .COM   2,0K``    Font loader for MODX  
``LL0     .      6,4K``    LAOLEO data file  
``LODEGEN .COM   1,3K``    Zoo level editor (V.Zverkov '90)  
``LR      .COM    13K``    Zoo demo version\* (single level)  
``MADUOK  .COM   9,3K``    Classic snake game (=Snake)  
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``NINJA   .COM    32K``    Ninjya Kage (Hudson '84/'24)  
``PUSHER  .COM    23K``    Pusher\* (=Sokoban, A.Mett '91)  
``PUSHER  .LEV   6,3K``      
``PUSHERPK.COM    16K``    Pusher level packer  
``PUSHER  .TXT   1,2K``    Pusher foreword (A.Mett '90)  
``PUTUP   .COM    18K``    Put Up (Y.Ago/MSX Magazine '87/'25)  
``READ    .ME    2,5K``    Brief intro to the J3K games disc '25  
``ROBBO   .COM    31K``    Robbo (LK Avalon '89/'25)  
``STOP    .COM    30K``    Stop the Train (Hudson '83/'24)  
``ZOKOBAN .COM    16K``    Zokoban (Errorsoft/Syntax '91)  
``ZOKOBAN .SIR    128``      
``ZOO1    .COM    16K``    Zoo original version\* (9 levels, VSW '91)  
``TANK    .COM    18K``    Tank Battalion (Namco '84/'25)  
``TET2    .COM    23K``    "Tetris" 1.1 (A.Mett '90)  
``TETRIS  .COM   1,9K``    Graphical "Tetris" (T.Ainsaar '90)  
``TKUK    .COM   2,0K``    Falling letters (Tramm '90/'25)  
``TOTDEM  .COM   4,8K``    Stupidity demo (Joga/Mamsoft '90/'25)  
``USSIKE  .COM   3,3K``    Zmejka (A.Alekseev '24/'25)  
``WARP    .COM    38K``    Warp & Warp (Namco '84/'24)  
``XONIX   .COM   3,8K``    "Xonix"\* (=Qix, E.Jürviste/EKTA '87)  

## J3KUTIL4

A Juku 3000 reconstruction of EKTA's JUKU PC UTILITIES DISK #4 from December 1989.
The selection of files is based on the `READ.ME` list included with the disc and may
not be complete. The disc can be downloaded from
https://elektroonikamuuseum.ee/failid/juku/tarkvara/J3KUTIL4.JUK. The OS on the disk
is EKDOS 2.30.

SIZE: `800K` (`819200`) / SHA1: `fb8a5239cdd74eced3b0bb7ab8ec6e8b2092f4c3`

``ASCII   .       896``    Latin alphabet font (US layout)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    128``      
``CAL     .COM    18K``    Floating-point calculator (40x24)  
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``CF      .COM   1,0K``    File copy 1.0 (EKTA '89)  
``CF      .HLP   1,5K``    CF quick guide  
``CHESS   .COM    31K``    Chess game "Let me think" (EKTA '89)  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DEMO    .COM   5,2K``    Audio-Video-Text demos (EKTA '88)  
``DEMO    .DOC   8,8K``    DEMO guide  
``DEMO    .HLP   3,5K``    DEMO help file  
``DEMOS   .COM   8,3K``    A-V-T demo preparation (EKTA)  
``DEMOS   .DOC    16K``    DEMOS guide  
``DOCTOR  .COM    36K``    Disk Editor & Diagnostics 1.11 ('83)  
``EKDOS30 .ASM    14K``    Source text of BIOS of EKDOS  
``EST     .       896``    Estonian alphabet font (JUKU)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``FX800   .COM   1,8K``    Epson FX-800 printer driver  
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``JCM     .HLP   7,4K``    JCM guide without title page ('89)  
``JLOAD   .LDR    384``    Resident programs loader  
``JSET    .COM    512``    Set BIOS I/O values  
``KULT    .COM    12K``    EKDOS Disk Test util 1.0 (EKTA '89)  
``KULT    .HLP   8,7K``    KULT guide  
``KUVA    .COM    768``    Screen centering 1.1 (K.Kevvai)  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LF      .COM   2,0K``    Font loader for MODX  
``LINK    .COM    16K``    Object-module linker 1.3 (CP/M '80)  
``MAC     .COM    12K``    Macro Assembler 2.0 (CP/M)  
``MDUMP   .COM    512``    Memory Dump  
``ME      .COM    32K``    Sound editor "Music Editor" 2.4 ('89)  
``MED     .COM   3,0K``    Memory EDitor 1.0 (EKTA)  
``ME      .DOC    12K``    ME 2.3 and PLAYER.ERL module guide  
``MIC     .COM   3,8K``    Micro-editor 1.0 (EKTA '88)  
``MIC     .HLP   6,3K``    MIC guide  
``MIT     .COM    16K``    Move-it: RS232 comms utility 3.0  
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MUSAM   .COM   3,7K``    Piano "Musa Master" (EKTA '89)  
``PLAYER  .ERL    512``    Pascal module for use with ME  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``PRT     .COM   4,0K``    Print file utility 5.3  
``PRT     .DOC   7,3K``    PRT.COM version 5.0 instructions  
``READ    .ME    4,2K``    JUKU util disk #4 info sheet ('89)  
``RESIDENT.DOC   1,7K``    Resident programs guide  
``RUS     .       896``    Cyrillic font (KOI-8)  
``SDEL    .COM    896``    Selective Delete v2.0  
``SED80   .COM    10K``    Screen text editor 6.1 (80x24)  
``SEIKO   .COM   1,8K``    Seikosha SP-800 driver  
``SETS    .COM   1,4K``    Set file(s) status (SETS \*.* $r/o)  
``SK      .COM   4,0K``    Calculator 1.0 (T.Martens/EKTA '89)  
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``SYSINFO .COM   1,2K``    Basic system info (CP/M)  
``WSJ     .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

## JUKGAME1

A consolidated image of recovered games from the January 2020 ELFA forum thread,
compiled by Mees Metsast. The same series also includes three JUKPROG`x` disks
published at the same time. The disks contain content of general interest from the
MAALT/MUUSEUM disks and from the compiler's personal disks, read in using various
DOS tools — mostly ImageDisk.

SIZE: `800K` (`819200`) / SHA1: `efd6e83669777966d523d323ea61e0352eea88ff`

``1       .       896``    LAOLEO data file  
``2       .       896``    LAOLEO data file  
``3       .       896``    LAOLEO data file  
``4       .       896``    LAOLEO data file  
``5       .       896``    LAOLEO data file  
``ASCII   .       896``    Latin alphabet font (US layout)  
``ATSKOO  .COM    18K``    Card game "Atskoo" (Kohtla-J 1KK)  
``AVTEST  .COM    14K``    Magic squares (=Sudoku, VSW '91)  
``AVTEST  .DOC   2,7K``    AVTEST foreword (V.Sinijärv '91)  
``BOWLING .COM   3,5K``    Bowling (Maxway & I.K.S. '91)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    256``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``CHESS   .COM    31K``    Chess game "Let me think" (EKTA '89)  
``EST     .       896``    Estonian alphabet font (JUKU)  
``GAMEBOY .COM    23K``    Fly and shoot (A.Säde '91)  
``GAMEBOY .DAT    512``      
``GAMEBOY .Z79   6,0K``      
``GAMEBOY .Z80   4,2K``      
``GAMEBOY .Z81   2,9K``      
``HUNTER  .COM   6,8K``    Hunting club (80x24, Vakstu/MIG '86)  
``HUNTER  .DAT    256``      
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``INDY    .DAT    12K``      
``KAP     .COM    32K``    "Battleship" (ed K.Koppel)  
``KAPTEN  .COM    32K``    "Merelahing"  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LAND    .COM    31K``      
``LAND    .DAT    640``      
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``LF      .COM   2,0K``    Font loader for MODX  
``LL0     .      6,4K``    LAOLEO data file  
``LOGER   .COM    32K``    Switch logic v1.1 (Nost Neji '90 H)  
``LUKK    .TET    128``      
``MADUOK  .COM   9,3K``    Classic snake game (=Snake)  
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MOND    .COM    17K``    Launch angle (=Artillery Duel)  
``RUS     .       896``    Cyrillic font (KOI-8)  
``SHOT    .COM   2,3K``    "Shot Master 2000" v1.1 (I.Käär '91)  
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``ZOO     .COM    25K``    "Lode Runner" at the zoo (BROKEN!)  
``TANK    .COM    15K``    Tank vs. UFOs (=Sabotage/Invaders)  
``TET     .COM    17K``    "Tetris" with mouse (A.Mett '90 H)  
``TETRIS1 .COM   1,9K``    Graphical "Tetris" (T.Ainsaar '90)  
``TETRIS  .COM    23K``    "Tetris" 1.1 (A.Mett '90)  
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

## JUKPROG1

A consolidated image of recovered programs #1 from the January 2020 ELFA forum thread, compiled by Mees Metsast.
See the JUKGAME1 description for details.

SIZE: `800K` (`819200`) / SHA1: `32708fd095be8ea50bf2ba185c6d5654e0ca3255`

``ALIENS  .PIC   1,7K``      
``ASCII   .       896``    Latin alphabet font (US layout)  
``AVE     .PLR   2,0K``      
``BACH    .PLR    256``      
``BEETHOVE.PLR    256``      
``BIGDASAR.PIC   1,3K``      
``BIKE    .PIC   2,0K``      
``BIZET   .PLR    512``      
``CAL     .COM    18K``    Floating-point calculator (40x24)  
``CD      .PIC   3,4K``      
``CF      .COM   1,0K``    File copy 1.0 (EKTA '89)  
``CF      .HLP   1,5K``    CF quick guide  
``CM6329  .COM   1,8K``    Robotron CM6329 printer driver  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``D100M   .COM   1,4K``    D100M printer driver (EKTA '91)  
``DEMO    .COM   5,2K``    Audio-Video-Text demos (EKTA '88)  
``DEMO    .DOC   8,8K``    DEMO guide  
``DEMO    .DOK   8,0K``    DEMO guide  
``DEMO    .HLP   3,5K``    DEMO help file  
``DEMOS   .COM   8,3K``    A-V-T demo preparation (EKTA)  
``DEMOS   .DOC    16K``    DEMOS guide  
``DIGGER  .COM   1,2K``    Viral star shower (K.Tomingas '91)  
``DOCTOR  .COM    36K``    Disk Editor & Diagnostics 1.11 ('83)  
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``EST     .       896``    Estonian alphabet font (JUKU)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``FLIGHT  .COM    896``      
``FMT     .COM   1,3K``    EKDOS 386K floppy formatter 3.4  
``FORMAT  .COM   1,3K``    EKDOS 786K floppy formatter 3.4  
``FRIENDS .PIC   2,4K``      
``FX800   .COM   1,8K``    Epson FX-800 printer driver  
``GAMEBOY1.PIC    896``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``GTR     .DOK    13K``    GTR editor instructions (partial '89)  
``HOTEL   .PIC   4,0K``      
``JAIL    .PIC   2,3K``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``JCM     .HLP   7,4K``    JCM guide without title page ('89)  
``JEESUS  .PIC   6,9K``      
``JOBU    .PIC   4,7K``      
``JSET    .COM    512``    Set BIOS I/O values  
``KAAK-MAD.PIC   2,9K``      
``KAALIKAS.PIC   2,5K``      
``KING    .PIC   2,7K``      
``KLAABUTV.PIC   1,2K``      
``KLIRR   .PIC   8,0K``      
``KORVITS2.PIC   2,9K``      
``KORVITS .PIC   2,5K``      
``KULT    .COM    12K``    EKDOS Disk Test util 1.0 (EKTA '89)  
``KULT    .HLP   8,7K``    KULT guide  
``KUVA    .COM    768``    Screen centering 1.1 (K.Kevvai)  
``LAEVADEP.PIC   2,2K``      
``LF      .COM   2,0K``    Font loader for MODX  
``MAASTIK .PIC   5,0K``      
``MAJA    .PIC   4,2K``      
``MAKK    .PIC   1,9K``      
``ME      .COM    32K``    Sound editor "Music Editor" 2.4 ('89)  
``MED     .COM   3,0K``    Memory EDitor 1.0 (EKTA)  
``ME      .DOC    12K``    ME 2.3 and PLAYER.ERL module guide  
``MEHHAAN2.PIC   5,2K``      
``MEHHAAN .PIC   3,4K``      
``MIC     .COM   3,8K``    Micro-editor 1.0 (EKTA '88)  
``MIC     .HLP   6,3K``    MIC guide  
``MIKA    .PIC   1,2K``      
``MODE    .COM    256``    40x24, 53x24 and 64x20 switch  
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MUSAM   .COM   3,7K``    Piano "Musa Master" (EKTA '89)  
``MUSKETAR.PIC   1,3K``      
``NSVL    .PIC   3,3K``      
``PACIUS  .PLR    256``      
``PATTERN .PIC   7,2K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``PLAYER  .ERL    512``    Pascal module for use with ME  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``PRT     .DOC   7,3K``    PRT.COM version 5.0 instructions  
``PUNK    .PIC    640``      
``RAHA    .PIC   1,8K``      
``RDEM    .COM    30K``    JUKU official demo program (EKTA '87)  
``READ    .ME    4,2K``    JUKU util disk #4 info sheet ('89)  
``RUS     .       896``    Cyrillic font (KOI-8)  
``SDEL    .COM    896``    Selective Delete v2.0  
``SED80   .COM    10K``    Screen text editor 6.1 (80x24)  
``SED     .COM    10K``    Screen text editor 6.1  
``SEIKO   .COM   1,8K``    Seikosha SP-800 driver  
``SETS    .COM   1,4K``    Set file(s) status (SETS \*.* $r/o)  
``SIPELGAS.PIC   3,4K``      
``SK      .COM   4,0K``    Calculator 1.0 (T.Martens/EKTA '89)  
``STAT    .COM   5,2K``    Filesystem statistics (CP/M)  
``SYSINFO .COM   1,2K``    Basic system info (CP/M)  
``TORUD   .PIC   7,5K``      
``URMAS   .PIC    896``      
``VALGRE  .PLR    128``      
``WSJ     .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  
``X-FILE  .PIC   1,7K``      

## JUKPROG2

A consolidated image of recovered programs #2 from the January 2020 ELFA forum thread, compiled by Mees Metsast.
See the JUKGAME1 description for details.

SIZE: `800K` (`819200`) / SHA1: `725233ba5f8943ff2778bf4d70dbf25f71a5854d`

``ASM     .COM   8,0K``    Assembler 2.0 (CP/M)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BASCOM  .COM    32K``    BASIC compiler 5.30 (Microsoft)  
``BASCOM  .DOK    11K``    BASCOM guide (EKTA '88)  
``BASLIB  .REL    25K``      
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``CF      .COM   1,0K``    File copy 1.0 (EKTA '89)  
``CF      .HLP   1,5K``    CF quick guide  
``CPU     .COM    19K``    Microprocessor Test 1.2 (EKTA '85)  
``DBAAS   .DOK    28K``    Introduction to dBASE II commands  
``DBASE   .COM    19K``    dBASE II v2.4  
``DBASEMSG.TXT    52K``      
``DBASEOVR.COM    40K``      
``DBINST  .COM    14K``      
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``DUMP    .COM    512``    File dump 1.4  
``ED      .COM   6,5K``    Context editor (CP/M)  
``EKDOS30 .ASM    14K``    Source text of BIOS of EKDOS  
``FORMAT  .COM   1,3K``    EKDOS 786K floppy formatter 3.4  
``INSTALL .COM   6,4K``    Microsoft tools config 1.02 ('81)  
``INSTALL .DAT    21K``      
``INSTALL .MSG    12K``      
``INSTALL .OVR    30K``      
``INSTALL .SPC    256``      
``JBASIC  .COM   8,2K``    BASIC interpreter 1.1 (EKTA '87)  
``JLOAD   .LDR    384``    Resident programs loader  
``L80     .COM    11K``    LINK-80 3.44 (Microsoft '81)  
``LINK    .COM    16K``    Module linker 1.3 (CP/M '80 V)  
``LOAD    .COM   1,8K``    HEX to COM converter (CP/M)  
``MAC     .COM    12K``    Macro Assembler 2.0 (CP/M)  
``MDUMP   .COM    512``    Memory Dump  
``MIT     .COM    16K``    Move-it: RS232 comms utility 3.0  
``MP40    .      6,3K``      
``MP80    .      6,3K``      
``MP      .COM    17K``    Multiplan 1.05 (Microsoft '81)  
``MP      .HLP    40K``      
``MPLAN   .DOK    32K``      
``MP      .OVR    43K``      
``MTEST2  .COM   9,5K``    Memory Test 0100-14FF (EKTA '85)  
``MTEST   .COM   4,5K``    Memory Test 1500-FFFF (EKTA '85)  
``NETD    .COM   7,4K``    Janet 1.0 14/11/00 (EKTA)  
``NETR    .COM   6,5K``    N-EKDOS 1.0 (EKTA)  
``PRT     .COM   4,0K``    Print file utility 5.3  
``QDISK   .COM   7,2K``    Disk Test (EKTA '85)  
``QRUN    .COM   4,8K``    Quick Test (EKTA '85)  
``RESIDENT.DOC   1,7K``    Resident programs guide  
``SID     .COM   7,0K``    Machine-code debugger SID 1.4 (CP/M)  
``SID     .DOK    19K``    Debugger user manual (EKTA '89)  
``SUBMIT  .COM   1,3K``    Command-batch processor (CP/M)  
``TERM    .COM   9,5K``    Terminal Demo/Test 1.2 (EKTA '85)  

## JUKPROGX

A consolidated image of recovered programs #3 from the January 2020 ELFA forum thread, compiled by Mees Metsast.
See the JUKGAME1 description for details.

SIZE: `800K` (`819200`) / SHA1: `7ac496b74bc5f0d6beeae5231b3f379b53ad8284`

``BASLIB  .REL    49K``      
``BIO80   .BAS   2,0K``      
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``F80     .COM    27K``    FORTRAN-80 v3.44 (Microsoft '81)  
``FORLIB  .REL    26K``      
``FORMAT  .COM   1,3K``    EKDOS 786K floppy formatter 3.4  
``FORT    .DOK    42K``    F80 compiler guide (EKTA '88)  
``FPREALS .ERL   7,5K``      
``LINKMT  .COM    12K``    Link/MT+ v5.6.1  
``MATIC80 .BAS   2,7K``      
``MR      .NOS   1,8K``      
``MTERRS  .TXT   4,8K``      
``MTPLUS  .000    13K``      
``MTPLUS  .001    11K``      
``MTPLUS  .002   7,0K``      
``MTPLUS  .003   7,3K``      
``MTPLUS  .004    17K``      
``MTPLUS  .005   8,5K``      
``MTPLUS  .006   6,2K``      
``MTPLUS  .COM    36K``    Pascal/MT+ v5.6.1  
``PASLIB  .ERL    25K``      
``STIIL   .BAS    512``      
``TRANCEND.ERL   3,3K``      
``YL80    .BAS   1,3K``      

## JUKUROMS

JUKU firmware monitors and extensions recovered from ROM chips, read in or collected
at various times by Pehka1985, Woldemar and others. The firmware `2.*` series is
generally for the tape system and the `3.*` series for floppy drives — most of these
for the FD1793, with Monitor 3.3 and EKTA series #0024 being for the FD1791. For
EKTA series #0043, the first chip's checksum does not match; the seventh chip of
Monitor 2.2 was read with a couple of errors, and the eighth chip with a total of
50 discrepancies across seven read attempts.

SIZE: `94K` (`95634`) / SHA1: `32eb55be835dccb84e24ee36522bb4014fd0d845`

``EKTA24  .BIN    16K``    RomBios 3.42, JUSS keyb (#0024 '88)  
``EKTA31  .BIN    16K``    RomBios 3.43 (#0031 '88)  
``EKTA32  .BIN    16K``    RomBios 2.43m (#0032 '88)  
``EKTA35  .BIN    16K``    RomBios 3.43m, JUSS keyb (#0035 '88)  
``EKTA37  .BIN    16K``    RomBios 3.43m, Baltijets (#0037 '88)  
``EKTA43  .BIN    16K``    RomBios 2.43m, AT keyb (#0043 '90)  
``JBASIC11.BIN   8,0K``    EKTA JBASIC 1.1? ('87)  
``JMON22  .BIN    16K``    Monitor 2.2, JBASIC ('85)  
``JMON33  .BIN    16K``    Monitor/Bootstrap 3.3, JBASIC ('85)  

## JUKUSYS

Operating systems found on various disks that JUKU is able to boot.

SIZE: `25K` (`25142`) / SHA1: `86df07916a834cc71d38a2885f439e5ceba42c25`

``CPM22   .BIN    10K``    CP/M 2.2  
``CPM231E .BIN    10K``    CP/M 2.31e (=EKDOS 2.30)  
``EKDOS229.BIN    10K``    EKDOS 2.29  
``EKDOS230.BIN    10K``    EKDOS 2.30  
``EKDOSVSW.BIN    10K``    "VSW working disk" (=EKDOS 2.29)  

## MAALT01

The disks of the MAALT`nn` series, together with the MUSEUM`nn` series, form the
basis of JUKPROG`n` and JUKGAME`1`. The disks were first read with the DOS ImageDisk
utility and then again with KryoFlux. Of the disks listed here, most come from the
ImageDisk batch, except disks 12, 15, 20 and 23, which ImageDisk originally read
incompletely. If something very important needs to be retrieved from the disks, the
two batches can be combined, but the original magnetic-flux recordings of the disks
have not been preserved and the condition of some disks deteriorated noticeably as
a result of reading them — already on the second read. Disks 14 and 17 were empty
and disk 19 was unreadable.

SIZE: `800K` (`819200`) / SHA1: `41c4064de6114dde4af54882fd6c1430e78f2a8b`

``7A1     .       896``      
``8BT     .       640``      
``8BT1    .       640``      
``9A      .      1,2K``      
``9A1     .       768``      
``9AT     .       896``      
``A       .       640``      
``ANRI    .      1,0K``      
``ANRI    .BAK   1,0K``      
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BEIB    .PIC   1,4K``      
``BIO80   .BAS   2,0K``      
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    256``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``CHESS   .COM    31K``    Chess game "Let me think" (EKTA '89)  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``COOL    .       640``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``HR P\TS .PIC    384``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``KIRI    .      2,8K``      
``KIRI    .BAK    896``      
``KIRJAND .      1,5K``      
``KIRJAND .BAK   1,5K``      
``KOOSOLEK.       512``      
``KP      .       384``      
``MATIC80 .BAS   2,7K``      
``MEELIS  .PIC    768``      
``MERLIN  .       640``      
``MERLIN  .BAK    768``      
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MR      .ALE    384``      
``MR      .NOS   1,8K``      
``MUSAM   .COM   3,7K``    Piano "Musa Master" (EKTA '89)  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``TAIMO   .       640``      
``URMAS   .PIC    896``      
``WSJ     .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  
``YL80    .BAS   1,3K``      

## MAALT02

SIZE: `800K` (`819200`) / SHA1: `d56922f9e75fec1705016429b3f30a047383b691`

``ANNELI  .      1,3K``      
``COMPU   .COM   1,8K``      
``ENOR    .       640``      
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``KIRJAND .      1,4K``      
``K|RT    .      1,2K``      
``LEPING  .      3,4K``      
``ME      .COM    32K``    Sound editor "Music Editor" 2.4 ('89)  
``MED     .COM   3,0K``    Memory EDitor 1.0 (EKTA)  
``PACIUS  .PLR    256``      
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``TAAVI   .       512``      
``TOOMAS  .       256``      
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      

### E5

``ANNELI  .BAK   1,3K``      
``ENOR    .BAK    640``      
``KIRJAND .BAK   1,4K``      
``K|RT    .BAK   1,2K``      
``LEPING  .BAK   3,4K``      
``PACIUS  .PLR    256``      
``TAAVI   .BAK    512``      
``UUS     .       128``      

## MAALT03

SIZE: `800K` (`819200`) / SHA1: `64b16291e7fdf850a1e3d6aabbd464b760aa3f88`

``ATSKOO  .COM    18K``    Card game "Atskoo" (Kohtla-J 1KK)  
``BOWLING .COM   3,5K``    Bowling (Maxway & I.K.S. '91)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    256``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``HUNTER  .COM   6,8K``    Hunting club (80x24, Vakstu/MIG '86)  
``HUNTER  .DAT    256``      
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``INDY    .DAT    12K``      
``KAP     .COM    32K``    "Battleship" (ed K.Koppel)  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``LOGER   .COM    32K``    Switch logic v1.1 (Nost Neji '90 H)  
``MADUOK  .COM   9,3K``    Classic snake game (=Snake)  
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MOND    .COM    17K``    Launch angle (=Artillery Duel)  
``SHOT    .COM   2,3K``    "Shot Master 2000" v1.1 (I.Käär '91)  
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``TETRIS  .COM   1,9K``    Graphical "Tetris" (T.Ainsaar '90)  
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

### E5

``LADCONF .COM      0``      

## MAALT04

SIZE: `800K` (`819200`) / SHA1: `e4223e2bba25dc4b2b3ba4de6a4f63b156566b8a`

``BUGABOO .       18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DBASE   .       19K``      
``DBASE   .COM    19K``      
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``GAMEBOY .       512``      
``GAMEBOY .COM    512``      
``GTR     .       27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``HUNTER  .COM   6,8K``    Hunting club (80x24, Vakstu/MIG '86)  
``HUNTER  .DAT    256``      
``JCM     .       12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``KAPTEN  .       32K``    "Merelahing"  
``KAPTEN  .COM    32K``      
``LADDER  .COM    40K``      
``LADDER  .DAT    512``      
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``LLL     .       31K``      
``LLL     .COM    31K``      
``ME      .COM    32K``    Sound editor "Music Editor" 2.4 ('89)  
``MED     .COM   3,0K``    Memory EDitor 1.0 (EKTA)  
``MODE    .       256``    40x24, 53x24 and 64x20 switch  
``MODE    .COM    256``    40x24, 53x24 and 64x20 switch  
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MOND    .COM    17K``    Launch angle (=Artillery Duel)  
``MP      .       17K``    Multiplan 1.05 (Microsoft '81)  
``MP      .COM    17K``    Multiplan 1.05 (Microsoft '81)  
``PIP     .COM   7,3K``    File copier (CP/M)  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``SHOT    .COM   2,3K``    "Shot Master 2000" v1.1 (I.Käär '91)  
``ZOO     .       25K``    "Lode Runner" at the zoo (BROKEN!)  
``ZOO     .COM    25K``      
``TANK    .       15K``    Tank vs. UFOs (=Sabotage/Invaders)  
``TANK    .COM    15K``      
``TET     .       17K``      
``TETRIS  .COM   1,9K``    Graphical "Tetris" (T.Ainsaar '90)  
``WS      .       16K``    MicroPro WordStar 3.0 (64x20)  
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

## MAALT05

SIZE: `800K` (`819200`) / SHA1: `2f13321727444f53e502591acf7a97b93b44e193`

``DBASE   .COM    19K``      
``DBASEMSG.TXT    52K``      
``DBASEOVR.COM    40K``      
``DBINST  .COM    14K``      
``FRIENDS .PIC   2,4K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``HOONED  .PIC   6,4K``      
``HOTEL   .PIC   4,0K``      
``INSTALL .COM   6,4K``    Microsoft tools config 1.02 ('81)  
``INSTALL .DAT    21K``      
``INSTALL .MSG    12K``      
``INSTALL .OVR    30K``      
``INSTALL .SPC    256``      
``LLMATTEE.PIC    768``      
``MP40    .      6,3K``      
``MP80    .      6,3K``      
``MP      .COM    17K``      
``MP      .HLP    40K``      
``MP      .OVR    43K``      
``PATTERN .PIC   7,2K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  

## MAALT06

SIZE: `800K` (`819200`) / SHA1: `ce3509c93b718c982f228e99b713ce87a965bb0c`

``1       .       896``    LAOLEO data file  
``2       .       896``    LAOLEO data file  
``3       .       896``    LAOLEO data file  
``4       .       896``    LAOLEO data file  
``5       .       896``    LAOLEO data file  
``7A      .       512``      
``8A34    .       512``      
``8B 0C   .PIC      0``      
``9A      .$$$      0``      
``AGENT 56.PIC      0``      
``ALLAN   .PIC      0``      
``ATSKOO  .COM    18K``    Card game "Atskoo" (Kohtla-J 1KK)  
``AVTEST  .COM    14K``    Magic squares (=Sudoku, VSW '91)  
``AVTEST  .DOC   2,7K``    AVTEST foreword (V.Sinijärv '91)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BIO80   .BAS   2,0K``      
``BOWLING .COM   3,5K``    Bowling (Maxway & I.K.S. '91)  
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``BUGABOO .COM    18K``      
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    256``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``FDDTREQE.PIC    128``      
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``FORMAT  .COM   1,3K``    EKDOS 786K floppy formatter 3.4  
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``HARLEY  .PIC      0``      
``HUNTER  .COM   6,8K``    Hunting club (80x24, Vakstu/MIG '86)  
``HUNTER  .DAT    256``      
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``INDY    .DAT    12K``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``KAP     .COM    32K``    "Battleship" (ed K.Koppel)  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LAND    .COM    31K``      
``LAND    .DAT    640``      
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``LAO     .LL       0``      
``LL0     .      6,4K``    LAOLEO data file  
``LOGER   .COM    32K``    Switch logic v1.1 (Nost Neji '90 H)  
``LUKK    .TET    128``      
``MP      .COM    17K``      
``MP      .HLP    40K``      
``MP      .OVR    43K``      
``MURDERS .PIC      0``      
``PATTERN .PIC   7,2K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``QQ574[] .PIC    256``      
``RAIN    .LL       0``      
``RDEM    .COM    30K``    JUKU official demo program (EKTA '87)  
``REX     .PIC      0``      
``S]BER   .PCD      0``      
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``STIIL   .BAS    512``      
``TUUBAVAH.PIC      0``      
``TUUSA   .         0``      
``URMAS   .PCD      0``      
``URMAS   .PIC   4,9K``      
``VGHJHJNH.LL     128``      
``VIKI    .PIC      0``      
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

## MAALT07

SIZE: `800K` (`819200`) / SHA1: `5c86653a2a1656bce163d92c1b774d3a7e39aae6`

``AVTEST  .COM    14K``      
``AVTEST  .DOC   2,7K``    AVTEST foreword (V.Sinijärv '91)  
``BOWLING .COM   3,5K``    Bowling (Maxway & I.K.S. '91)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    256``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MOND    .COM    17K``    Launch angle (=Artillery Duel)  
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

### E5

``SNAKE   .DAT   1,0K``      

## MAALT08

SIZE: `800K` (`819200`) / SHA1: `e06467eafb906cdf21da1f896d4beb040f37302a`

``1       .       896``    LAOLEO data file  
``2       .       896``    LAOLEO data file  
``3       .       896``    LAOLEO data file  
``4       .       896``    LAOLEO data file  
``5       .       896``    LAOLEO data file  
``ATSKOO  .COM    18K``    Card game "Atskoo" (Kohtla-J 1KK)  
``AVTEST  .COM    14K``    Magic squares (=Sudoku, VSW '91)  
``AVTEST  .DOC   2,7K``    AVTEST foreword (V.Sinijärv '91)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BIO80   .BAS   2,0K``      
``BOWLING .COM   3,5K``    Bowling (Maxway & I.K.S. '91)  
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    256``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DEL     .LL     128``      
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``GB      .COM    23K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``INDY    .DAT    12K``      
``KAP     .COM    32K``    "Battleship" (ed K.Koppel)  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LAND    .COM    31K``      
``LAND    .DAT    640``      
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``LL0     .      6,4K``    LAOLEO data file  
``LOGER   .$$$      0``      
``LUKK    .TET    128``      
``MADUOK  .$$$      0``      
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MOND    .COM    17K``    Launch angle (=Artillery Duel)  
``PATTERN .PIC   7,2K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``PUSHER  .$$$      0``      
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``TET     .         0``      
``TETRIS  .COM   1,9K``    Graphical "Tetris" (T.Ainsaar '90)  
``TORUD   .PIC   7,5K``      
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

### E5

``KRISTJAN.       512``      
``KRISTJAN.BAK    768``      

## MAALT09

SIZE: `800K` (`819200`) / SHA1: `1bab084d9d7869327319fbc9cc3de245df9eab32`

``ATSKOO  .COM    18K``    Card game "Atskoo" (Kohtla-J 1KK)  
``AVTEST  .COM    14K``    Magic squares (=Sudoku, VSW '91)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``GAMEBOY .COM    23K``    Fly and shoot (A.Säde '91)  
``GAMEBOY .DAT    512``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``KAP     .COM    32K``    "Battleship" (ed K.Koppel)  
``KAPTEN  .COM    32K``    "Merelahing"  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``LLL     .COM    31K``      
``MODE    .COM    256``    40x24, 53x24 and 64x20 switch  
``MOND    .COM    17K``    Launch angle (=Artillery Duel)  
``MP      .$$$      0``      
``MUSAM   .COM   3,7K``    Piano "Musa Master" (EKTA '89)  
``PIP     .COM   7,3K``    File copier (CP/M)  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``ZOO     .COM    25K``    "Lode Runner" at the zoo (BROKEN!)  
``TANK    .COM    15K``    Tank vs. UFOs (=Sabotage/Invaders)  
``TET     .COM    17K``      
``TETRIS  .COM    23K``    "Tetris" 1.1 (A.Mett '90)  
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

## MAALT10

SIZE: `800K` (`819200`) / SHA1: `79a8b5a7b31e98a800ebbfbaedc440dec22a8db9`

``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``G       .       384``      
``HERB    .      3,3K``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``LOOMAB  .      9,8K``      
``LOOMAB  .BAK   6,8K``      
``MP40    .      6,3K``      
``MP80    .      6,3K``      
``MP      .COM    17K``      
``MP      .HLP    40K``      
``MP      .OVR    43K``      
``POHL    .      1,4K``      
``PTUK    .      3,8K``      
``PUTUK   .      8,0K``      
``PUTUK   .BAK   8,0K``      
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      

### E5

``PUTUK   .BAK   7,9K``      

## MAALT11

SIZE: `800K` (`819200`) / SHA1: `cd9e2f4cf660f439ed769ed48f1520356f2b4a34`

``========.===   4,0K``      
``5AINED  .       768``      
``5B13-15B.       384``      
``5B13-16 .       640``      
``5KALAD  .       768``      
``5L5A    .       768``      
``5L5B    .       640``      
``5LAHUS  .       512``      
``5L}LK   .       512``      
``5METS-1 .      1,0K``      
``6AED    .       768``      
``6BMETS  .      1,4K``      
``6BTMETSB.      1,3K``      
``7A11    .      1,9K``      
``7A17B   .       896``      
``7AAK    .      5,7K``      
``7AK     .      1,5K``      
``7AK10   .      1,4K``      
``7AK11   .      1,0K``      
``7AK12   .      1,2K``      
``7AK13   .      1,8K``      
``7AK2    .      2,4K``      
``7AK4    .      2,3K``      
``7AK5    .      2,0K``      
``7AK6    .       896``      
``7AK7    .      2,0K``      
``7AK8    .      2,3K``      
``7AK9    .      1,7K``      
``7AKT    .      1,5K``      
``7AKT1   .      1,2K``      
``7AT11   .       640``      
``7AT4    .      1,2K``      
``7AT46   .       512``      
``7AT48   .       768``      
``7AT51   .       256``      
``7AT54   .       896``      
``7BAK    .       11K``      
``7BK2    .      1,4K``      
``7BK3    .      1,0K``      
``7BK4    .      1,2K``      
``7BK5    .      1,5K``      
``7BT423  .       768``      
``7INIM-A .      2,2K``      
``7}IS    .      2,0K``      
``7KIRIK  .      1,5K``      
``7SEEDE03.      2,4K``      
``7SEEDE-2.      1,4K``      
``7SEEDE-3.      2,4K``      
``7TALUP  .       768``      
``7USUP-KT.      1,2K``      
``7UUS-AEG.      1,4K``      
``7VEGET  .      2,2K``      
``8A18    .      1,7K``      
``8A19    .       640``      
``8A20A   .       384``      
``8A20B   .       384``      
``8A21    .      1,3K``      
``8A21A   .      1,7K``      
``8A22    .      1,0K``      
``8A23    .       768``      
``8A24    .      1,0K``      
``8A25    .       896``      
``8A30    .       896``      
``8A31    .      1,2K``      
``8AAK    .      4,0K``      
``8AK17-18.      3,7K``      
``8AKT1   .      1,3K``      
``8AKT25A .      1,4K``      
``8AKT25B .      1,3K``      
``8AT12   .      1,2K``      
``8AT18   .       768``      
``8AT43   .       768``      
``8AT6    .       768``      
``8AT9    .      1,0K``      
``8AT     .NAP   1,9K``      
``8B      .       768``      
``8B4     .1A     512``      
``8B4     .1B     512``      
``8B4     .2      256``      
``8BKT1   .       896``      
``8BKT2   .       896``      
``8BKT3   .       896``      
``8BKT4   .      1,2K``      
``8BKT5   .      1,4K``      
``8BKT6   .       640``      
``8BKT7   .      1,2K``      
``8BKT8   .       768``      
``8PR     .REV   2,7K``      
``8}T     .       768``      
``8VETIK  .      1,2K``      
``9A21    .      1,3K``      
``9A22    .      1,5K``      
``9AK15   .       896``      
``9AK16   .       768``      
``9AK17   .      1,3K``      
``9AK21   .      1,7K``      
``9AT1-19 .      1,0K``      
``9AT1-19A.      1,0K``      
``9B      .       384``      
``9BB     .       384``      
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DULE DD .PIC    512``      
``EL      .       896``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``HINDED  .PIC    384``      
``KAP     .PIC    512``      
``­ KASTID .PCD    128``      
``MAASTIK .PIC   5,0K``      
``MUSAM   .COM   3,7K``    Piano "Musa Master" (EKTA '89)  
``PUNK    .PIC    640``      
``RAHA    .PIC   1,8K``      
``RDEM    .COM    30K``    JUKU official demo program (EKTA '87)  
``SIPELGAS.PIC   3,4K``      
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    16K``      
``WSOVLY1 .OVR    34K``      
``X8AK2   .      1,2K``      
``X-FILE  .PIC   1,7K``      
``XZSDCCBR.PIC   1,2K``      

### E5

``7AAK    .BAK   4,8K``      
``7AK11   .BAK   1,0K``      
``7BAK    .BAK   8,5K``      
``8A25    .BAK    896``      
``8A30    .BAK    896``      

## MAALT12

SIZE: `800K` (`819200`) / SHA1: `e0f6bbcd84eabb2e65cc2e82c09fbc45051c474e`

``DBASE   .COM    19K``      
``DBASEMSG.TXT    52K``      
``DBASEOVR.COM    40K``      
``DBINST  .COM    14K``      
``GTR     .COM    27K``      
``INSTALL .COM   6,4K``    Microsoft tools config 1.02 ('81)  
``INSTALL .DAT    21K``      
``MP40    .      6,3K``      
``MP80    .      6,3K``      
``MP      .COM    17K``      
``MP      .HLP    40K``      
``MP      .OVR    43K``      
``PATTERN .PIC   7,2K``      

## MAALT13

SIZE: `800K` (`819200`) / SHA1: `e8e34c5ea5f643fae3045026f265cda57238e077`

``04PALK  .      2,5K``      
``1993    .CMD    512``      
``1993    .DBF   8,0K``      
``1993    .MEM    512``      
``AHV     .PIC   2,2K``      
``AMBU    .DBF   5,0K``      
``AMBUL   .      1,0K``      
``AMBULANT.DBF   3,5K``      
``AMBU    .MEM    512``      
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .TAB    384``      
``D100M   .COM   1,4K``    D100M printer driver (EKTA '91)  
``DBASE   .COM    19K``      
``DBASEMSG.TXT    52K``      
``DBASEOVR.COM    40K``      
``DBINST  .COM    14K``      
``DDDHHHHH.PCD    128``      
``EEEEEEEE.PIC    128``      
``FFFFHELH.ADD      0``      
``FFFFHELH.PIC    256``      
``GAMEBOY .COM    23K``    Fly and shoot (A.Säde '91)  
``GAMEBOY .DAT    512``      
``GAMEBOY .Z79   6,0K``      
``GAMEBOY .Z80   4,2K``      
``GAMEBOY .Z81   2,9K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``HAIGLA  .DBF    17K``      
``HAIGLA  .MEM    512``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``JKS     .DBF   1,0K``      
``KAALIKAS.PIC   2,5K``      
``KAPTEN  .COM    32K``    "Merelahing"  
``LLL     .COM    31K``    Chess game "Let me think" (EKTA '89)  
``MODE    .COM    256``    40x24, 53x24 and 64x20 switch  
``MP40    .      6,3K``      
``MP80    .      6,3K``      
``MP      .COM    17K``    Multiplan 1.05 (Microsoft '81)  
``MP      .HLP    40K``      
``MP      .OVR    43K``      
``PALK    .      2,3K``      
``PULL    .PIC   1,7K``      
``SSSSSSSE.PIC    128``      
``ZOO     .COM    25K``    "Lode Runner" at the zoo (BROKEN!)  
``TANK    .COM    15K``    Tank vs. UFOs (=Sabotage/Invaders)  
``TET     .COM    17K``    "Tetris" with mouse (A.Mett '90 H)  
``TETRIS  .COM    23K``    "Tetris" 1.1 (A.Mett '90)  
``UK      .DBF   1,0K``      
``UUS     .       128``      
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      

## MAALT15

SIZE: `800K` (`819200`) / SHA1: `f507c24710e92e4a22385191309e429aeeba2b59`

``9MAT    .       896``      
``9VENE2  .      1,9K``      
``9VENE4  .      2,2K``      
``9VENE6  .      2,5K``      
``A       .      1,0K``      
``ARGO    .      1,2K``      
``B       .      1,4K``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``D       .       640``      
``ELEKTRA .       384``      
``H       .PIC    768``      
``K       .      2,8K``      
``KOOLIST .       640``      
``KOR     .       512``      
``KUTSE   .PIC   2,0K``      
``KVIITUNG.       640``      
``M       .      1,5K``      
``MA      .      1,2K``      
``MAARIKA .      1,2K``      
``N       .       256``      
``P       .       896``      
``PRIIDU  .      1,0K``      
``R       .       768``      
``TAIRI   .      1,0K``      
``TEATIS  .       128``      
``UUS     .       128``      
``V|RK    .       128``      
``WS      .COM    16K``      
``WSJ     .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      

### E5

``9MAT    .BAK    896``      
``9VENE4  .BAK   2,2K``      
``9VENE6  .BAK   2,5K``      
``A       .BAK   1,0K``      
``ARGO    .BAK   1,2K``      
``ELEKTRA .BAK    384``      
``KOR     .BAK    384``      
``KVIITUNG.BAK    640``      
``MAARIKA .BAK   1,2K``      
``MA      .BAK   1,2K``      
``PRIIDU  .BAK    896``      
``R       .BAK    768``      
``TAIRI   .BAK   1,0K``      
``TEATIS  .BAK    128``      

## MAALT18

An empty system disk whose boot sectors hold the standard EKDOS 2.30.

SIZE: `800K` (`819200`) / SHA1: `1f6b7ade822ba563de16153d272f12add337a3d5`

## MAALT20

SIZE: `800K` (`819200`) / SHA1: `9612a6d94a2587848cafc342bc1706e83c9e0ed3`

``1       .       896``    LAOLEO data file  
``2       .       896``    LAOLEO data file  
``3       .       896``    LAOLEO data file  
``4       .       896``    LAOLEO data file  
``5       .       896``    LAOLEO data file  
``AVTEST  .COM    14K``    Magic squares (=Sudoku, VSW '91)  
``AVTEST  .DOC   2,7K``    AVTEST foreword (V.Sinijärv '91)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BIO80   .BAS   2,0K``      
``CATCHIUM.$$$      0``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``CHESS   .COM    31K``    Chess game "Let me think" (EKTA '89)  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``FORMAT  .COM   1,3K``    EKDOS 786K floppy formatter 3.4  
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``ME      .COM    32K``    Sound editor "Music Editor" 2.4 ('89)  
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``NS      .$$$      0``      
``PACIUS  .PLR    256``      
``PATTERN .PIC   7,2K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``SIGRID  .PIC    128``      
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``STIIL   .BAS    512``      
``ZOO     .COM    25K``    "Lode Runner" at the zoo (VAKSTU '91)  
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

## MAALT21

SIZE: `800K` (`819200`) / SHA1: `30b6d50335891834596fa058cf7de09892cf40ec`

``DBASE   .COM    19K``      
``DBASEMSG.TXT    52K``      
``DBASEOVR.COM    40K``      
``DBINST  .COM    14K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``INSTALL .COM   6,4K``    Microsoft tools config 1.02 ('81)  
``INSTALL .DAT    21K``      
``INSTALL .MSG    12K``      
``INSTALL .OVR    30K``      
``INSTALL .SPC    256``      
``MP40    .      6,3K``      
``MP80    .      6,3K``      
``MP      .COM    17K``    Multiplan 1.05 (Microsoft '81)  
``MP      .HLP    40K``      
``MP      .OVR    43K``      
``PATTERN .PIC   7,2K``      

## MAALT22

SIZE: `800K` (`819200`) / SHA1: `787ae3e0776d9feefb079ce397a8ed4ee759c5ec`

``AASTAD  .      2,2K``      
``ATSKOO  .COM    18K``    Card game "Atskoo" (Kohtla-J 1KK)  
``AVTEST  .COM    14K``      
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BIKE    .PIC   2,0K``      
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``CHESS   .COM    31K``    Chess game "Let me think" (EKTA '89)  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``GAMEBOY .COM    512``      
``GB      .COM    23K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``INDY    .DAT    12K``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``JOBU    .PIC   4,7K``      
``KAAK MAD.PIC   2,9K``      
``KAPTEN  .COM    32K``    "Merelahing"  
``KING    .PIC   2,7K``      
``K@RVITS .PIC   2,5K``      
``LADDER  .COM    40K``      
``LAEVADEP.PIC   2,2K``      
``LAOLEO  .COM    32K``      
``MAKK    .PIC   1,9K``      
``MEHHAAN .PIC   3,4K``      
``MODE    .COM    256``    40x24, 53x24 and 64x20 switch  
``MOND    .COM    17K``    Launch angle (=Artillery Duel)  
``MUSAM   .COM   3,7K``    Piano "Musa Master" (EKTA '89)  
``NSVL    .PIC   3,3K``      
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``ZOO     .COM    25K``      
``TANK    .COM    15K``      
``TETRIS  .COM   1,9K``    Graphical "Tetris" (T.Ainsaar '90)  
``VISIT   .PIC   1,0K``      
``WS      .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``WSJ     .COM    16K``    MicroPro WordStar 3.0 (64x20)  
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

### E5

``LADCONF .COM      0``      

## MAALT23

SIZE: `800K` (`819200`) / SHA1: `9d37a51bba816f18eeee643ecf6652ff69d73c67`

``B80     .COM    24K``      
``BIO80   .BAS   2,0K``      
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    256``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``CHESS   .COM    31K``    Chess game "Let me think" (EKTA '89)  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``K\RT    .PIC    768``      
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``SUMMA   .BAS    256``      
``V}RRAND .BAS    512``      

### E5

``JCM2    .$$$      0``      
``WSJ     .COM    16K``      
``WSMSGS  .$$$    28K``      

## MAALT24

SIZE: `800K` (`819200`) / SHA1: `11e18ae89b5943386a538cbff53d18c46dcb4798`

``1       .       896``    LAOLEO data file  
``2       .       896``    LAOLEO data file  
``3       .       896``    LAOLEO data file  
``5       .       896``    LAOLEO data file  
``ATSKOO  .COM    18K``    Card game "Atskoo" (Kohtla-J 1KK)  
``AVTEST  .COM    14K``    Magic squares (=Sudoku, VSW '91)  
``AVTEST  .DOC   2,7K``    AVTEST foreword (V.Sinijärv '91)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BIO80   .BAS   2,0K``      
``BOWLING .COM   3,5K``    Bowling (Maxway & I.K.S. '91)  
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    256``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DEL     .LL     128``      
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``GAMEBOY .Z79   6,0K``      
``GB      .COM    23K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``INDY    .DAT    12K``      
``KAP     .COM    32K``    "Battleship" (ed K.Koppel)  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LAND    .COM    31K``      
``LAND    .DAT    640``      
``LAOLEO  .COM    32K``    "Laoleo" (=Sokoban, Kompuuter '91 H)  
``LL0     .      6,4K``    LAOLEO data file  

## MAALT25D

SIZE: `800K` (`819200`) / SHA1: `58c157f28a3a49ce7b0f0fbffba939ee2a851116`

``1       .       896``    LAOLEO data file  
``2       .       896``    LAOLEO data file  
``3       .       896``    LAOLEO data file  
``5       .       896``    LAOLEO data file  
``AASTAD  .PIC   2,2K``      
``ATSKOO  .COM    18K``    Card game "Atskoo" (Kohtla-J 1KK)  
``AVTEST  .COM    14K``    Magic squares (=Sudoku, VSW '91)  
``AVTEST  .DOC   2,7K``    AVTEST foreword (V.Sinijärv '91)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BIGDASAR.PIC   1,3K``      
``BIKE    .PIC   2,0K``      
``BIO80   .BAS   2,0K``      
``BOWLING .COM   3,5K``    Bowling (Maxway & I.K.S. '91)  
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    384``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``­ CIRCLES.PIC   6,9K``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DASAKSRK.PIC   2,4K``      
``DEL     .PIC    128``      
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``FILOTRIP.PIC   2,5K``      
``FILOTROP.PIC   2,0K``      
``GB      .COM    23K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``INDY    .COM    27K``    Indy Looking for Jewels (I.Käär '91)  
``INDY    .DAT    12K``      
``JAIL    .PIC   2,3K``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``­ JEESUS .PIC   6,9K``      
``JOBUUUUU.PIC   4,7K``      
``KAAK MAD.PIC   2,9K``      
``KAP     .COM    32K``    "Battleship" (ed K.Koppel)  
``KAST    .PIC    512``      
``KINGKONG.PIC   2,7K``      
``KLAABUTV.PIC   1,2K``      
``KLIRR   .PIC   8,0K``      
``­ K`RVITS.PIC   2,9K``      
``K`RVITS .PIC   2,5K``      
``KUTSE   .PIC   1,0K``      
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LAEVADEP.PIC   2,2K``      
``LL0     .      6,4K``    LAOLEO data file  
``LUKK    .TET    128``      
``MAKK    .PIC   1,9K``      
``­ MEHHAAN.PIC   5,2K``      
``MEHHAAN .PIC   3,4K``      
``MIKA    .PIC   1,2K``      
``MOND    .COM    17K``    Launch angle (=Artillery Duel)  
``MUSAM   .COM      0``      
``MUSKET\R.PIC   1,3K``      
``NSVL    .PIC   3,3K``      
``PATTERN .PIC   7,2K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``POWW    .PIC   3,2K``      
``PR ELLA .PIC   1,0K``      
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``­ TITANIK.PIC   2,2K``      
``TITANIK .PIC   2,3K``      
``ULLA TRU.PIC    896``      
``VISIIT  .P     1,0K``      
``­ V\RDJAS.PIC   2,3K``      
``V\RDJAS .PIC   1,7K``      

## MAALT26

SIZE: `800K` (`818688`) / SHA1: `ddf3bf83e7bf1247215470b869eb553eaab89424`

``1       .       384``      
``7AAK    .       14K``      
``7AAK    .BAK    14K``      
``7AKT    .      1,2K``      
``7AT8;9  .      1,8K``      
``7B3     .1      640``      
``7BAK    .      6,8K``      
``7G1     .3     1,0K``      
``7G3     .      3,5K``      
``7GAK    .      3,2K``      
``7KAART  .      1,0K``      
``8AAK    .       13K``      
``8BAK    .       13K``      
``8BKT    .      2,0K``      
``8BT     .      1,0K``      
``9AAK    .       12K``      
``9AK2    .A     1,8K``      
``9B1     .4      896``      
``9B1     .4B    1,2K``      
``9B4     .2     1,3K``      
``9BAK    .      8,0K``      
``9BKT9   .      2,4K``      
``AED2001 .      1,2K``      
``COMPU   .COM   1,8K``      
``L}AK    .       21K``      
``LAK     .      8,9K``      
``LOODUS  .      3,4K``      
``LOOM    .2      15K``      
``MAA     .       768``      
``MLG     .       43K``      
``MP40    .      6,3K``      
``MP80    .      6,3K``      
``MP      .COM    17K``      
``MP      .HLP    40K``      
``MP      .OVR    43K``      
``PROJ    .       12K``      
``PS      .       384``      
``RAKK    .      4,4K``      
``VM      .      7,9K``      
``WS      .COM    16K``      
``WSMSGS  .OVR    28K``      
``WSOVLY1 .OVR    34K``      

### E5

``7AAK    .BAK    14K``      

## MAALT27

SIZE: `800K` (`819200`) / SHA1: `c695e5833d7aa7dd2bb161b6948819c027dac0b8`

``ALIENS  .PIC   1,7K``      
``ANDMED  .DBF   1,0K``      
``AVTEST  .$$$      0``      
``AVTEST  .COM    14K``    Magic squares (=Sudoku, VSW '91)  
``AVTEST  .DOC   2,7K``    AVTEST foreword (V.Sinijärv '91)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``CD      .PIC   3,4K``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``DOCTOR  .COM    36K``    Disk Editor & Diagnostics 1.11 ('83)  
``F-1     .PI    2,0K``      
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``GAMEBOY .COM    23K``      
``GAMEBOY .DAT    512``      
``GAMEBOY .Z79   6,0K``      
``GAMEBOY .Z80   4,2K``      
``GAMEBOY .Z81   2,9K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``HAIGLA  .DBF    17K``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``JESUS CH.PIC   2,7K``      
``MA      .PIC    256``      
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``POWER   .COM    16K``    Disk manager 3.03 (P.Breder '82)  
``SARVIK  .PIC   2,9K``      
``ZOO     .COM    25K``    "Lode Runner" at the zoo (BROKEN!)  
``TANK    .COM    15K``    Tank vs. UFOs (=Sabotage/Invaders)  
``TET     .COM    17K``      
``TETRIS  .COM    23K``    "Tetris" 1.1 (A.Mett '90)  
``WS      .COM    16K``      
``WSMSGS  .$$$      0``      

## MANUALID

SIZE: `26K` (`25697`) / SHA1: `dacdaaf586dd6144d24f9baa8cfe62555fc48587`

``DBASE   .DOK    37K``    dBASE II guide (EÕK '90)  
``GTR     .DOK    12K``    GTR editor instructions #1 (EKTA '89)  
``GTRLISA .DOK   9,9K``    GTR editor instructions #2 (EKTA '89)  
``JCM     .DOK   7,8K``    JCM guide (EÕK '90)  

## MUSEUM01

The four disks of the MUSEUM`nn` series, together with the MAALT`nn` series, form the
basis of JUKPROG`n` and JUKGAME`1`. For the back story of these disks, see the `MAALT01`
description.

SIZE: `800K` (`819200`) / SHA1: `956c82e43e2b1f76a337190f78318428729e845f`

``ASM     .COM   8,0K``    Assembler 2.0 (CP/M)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BASCOM  .COM    32K``    BASIC compiler 5.30 (Microsoft)  
``BASLIB  .REL    49K``      
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``CM6329  .COM   1,8K``    Robotron CM6329 printer driver  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``CPU     .COM    19K``    Microprocessor Test 1.2 (EKTA '85)  
``D100M   .COM   1,4K``    D100M printer driver (EKTA '91)  
``DIAG    .LOG      0``      
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``DUMP    .COM    512``    File dump 1.4  
``ED      .COM   6,5K``    Context editor (CP/M)  
``F80     .COM    27K``    FORTRAN-80 v3.44 (Microsoft '81)  
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``FMT     .COM   1,3K``    EKDOS 386K floppy formatter 3.4  
``FORLIB  .REL    26K``      
``FORMAT  .COM   1,3K``    EKDOS 786K floppy formatter 3.4  
``FX800   .COM   1,8K``    Epson FX-800 printer driver  
``I       .       128``      
``JBASIC  .COM   8,2K``    BASIC interpreter 1.1 (EKTA '87)  
``KUVA    .COM    768``    Screen centering 1.1 (K.Kevvai)  
``L80     .COM    11K``    LINK-80 3.44 (Microsoft '81)  
``LOAD    .COM   1,8K``    HEX to COM converter (CP/M)  
``MODE    .COM    256``    40x24, 53x24 and 64x20 switch  
``MTEST2  .COM   9,5K``    Memory Test 0100-14FF (EKTA '85)  
``MTEST   .COM   4,5K``    Memory Test 1500-FFFF (EKTA '85)  
``NETD    .COM   7,4K``    Janet 1.0 14/11/00 (EKTA)  
``NETR    .COM   6,5K``    N-EKDOS 1.0 (EKTA)  
``PIP     .COM   7,3K``    File copier (CP/M)  
``QDISK   .COM   7,2K``    Disk Test (EKTA '85)  
``QRUN    .COM   4,8K``    Quick Test (EKTA '85)  
``RDEM    .COM    30K``    JUKU official demo program (EKTA '87)  
``SED     .COM    10K``    Screen text editor 6.1  
``SID     .COM   7,0K``    Machine-code debugger SID 1.4 (CP/M)  
``STAT    .COM   5,2K``    Filesystem statistics (CP/M)  
``SUBMIT  .COM   1,3K``    Command-batch processor (CP/M)  
``TERM    .COM   9,5K``    Terminal Demo/Test 1.2 (EKTA '85)  
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  

## MUSEUM02

SIZE: `800K` (`819200`) / SHA1: `054b854a9bc58383794e74fdc2f778f746bdf55d`

``FPREALS .ERL   7,5K``      
``LINKMT  .COM    12K``    Link/MT+ v5.6.1  
``MTERRS  .TXT   4,8K``      
``MTPLUS  .000    13K``      
``MTPLUS  .001    11K``      
``MTPLUS  .002   7,0K``      
``MTPLUS  .003   7,3K``      
``MTPLUS  .004    17K``      
``MTPLUS  .005   8,5K``      
``MTPLUS  .006   6,2K``      
``MTPLUS  .COM    36K``    Pascal/MT+ v5.6.1  
``PASLIB  .ERL    25K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``TRANCEND.ERL   3,3K``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  

## MUSEUM03

SIZE: `800K` (`819200`) / SHA1: `2bd379212078b892ad07766007507b02bbda3703`

``DBASE   .COM    19K``    dBASE II v2.4  
``DBASEMSG.TXT    52K``      
``DBASEOVR.COM    40K``      
``DBINST  .COM    14K``      
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``INSTALL .COM   6,4K``    Microsoft tools config 1.02 ('81)  
``INSTALL .DAT    21K``      
``INSTALL .MSG    12K``      
``INSTALL .OVR    30K``      
``INSTALL .SPC    256``      
``MP40    .      6,3K``      
``MP80    .      6,3K``      
``MP      .COM    17K``    Multiplan 1.05 (Microsoft '81)  
``MP      .HLP    40K``      
``MP      .OVR    43K``      
``PATTERN .PIC   7,2K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  

## MUSEUM04

SIZE: `800K` (`819200`) / SHA1: `76289c35e1e4a858ae4b9dcdfe81cc2e175559cb`

``2       .      7,4K``    JCM guide without title page ('89)  
``BASCOM  .DOK    11K``    BASCOM guide (EKTA '88)  
``DBAAS   .DOK    28K``    Introduction to dBASE II commands  
``DEMO    .DOK   8,0K``    DEMO guide  
``DIR     .       12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``DOCTOR  .COM    36K``      
``FORT    .DOK    42K``    F80 compiler guide (EKTA '88)  
``GTR     .$$$      0``      
``GTR     .DOK    13K``    GTR editor instructions (partial '89)  
``JCM     .       12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``JCMHELP .      7,4K``    JCM guide without title page ('89)  
``ME      .COM    32K``      
``ME      .DOC    12K``    ME 2.3 and PLAYER.ERL module guide  
``MP      .HLP    40K``      
``MPLAN   .DOK    32K``      
``PACIUS  .PLR    256``      
``SID     .DOK    19K``    Debugger user manual (EKTA '89)  
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  

## OKSJON01

The OKSJON`nn` series consists of test purchases made in 2021–2022 mainly via the
Osta.ee auction site, with the aim of locating JUKU disks; the disks were read with
Greaseweazle. The disks were recovered by Pehka1985.

SIZE: `800K` (`819200`) / SHA1: `f380b3751385b0cf95bd599664f94742d45a69de`

``ASM     .COM   8,0K``    Assembler 2.0 (CP/M)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BASCOM  .COM    32K``    BASIC compiler 5.30 (Microsoft)  
``BASLIB  .REL    49K``      
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``CM6329  .COM   1,8K``    Robotron CM6329 printer driver  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``CPU     .COM    19K``    Microprocessor Test 1.2 (EKTA '85)  
``DIAG    .LOG      0``      
``DOSGEN  .COM    896``    System disk generator 3.4 (CP/M)  
``DUMP    .COM    512``    File dump 1.4  
``ED      .COM   6,5K``    Context editor (CP/M)  
``F80     .COM    27K``    FORTRAN-80 v3.44 (Microsoft '81)  
``FDMAINT .COM    11K``      
``FMT     .COM   1,3K``    EKDOS 386K floppy formatter 3.4  
``FORLIB  .REL    26K``      
``FORMAT  .COM   1,3K``      
``FX800   .COM   1,8K``      
``JBASIC  .COM   8,2K``    BASIC interpreter 1.1 (EKTA '87)  
``KUVA    .COM    768``      
``L80     .COM    11K``    LINK-80 3.44 (Microsoft '81)  
``LOAD    .COM   1,8K``    HEX to COM converter (CP/M)  
``LSC     .ASM    768``      
``LSC     .COM    128``      
``LSC     .HEX    384``      
``LSC     .PRN   1,5K``      
``LSC     .SYM    128``      
``MODE    .COM    256``      
``MTEST2  .COM   9,5K``    Memory Test 0100-14FF (EKTA '85)  
``MTEST   .COM   4,5K``    Memory Test 1500-FFFF (EKTA '85)  
``NETD    .COM   7,4K``    Janet 1.0 14/11/00 (EKTA)  
``NETR    .COM   6,5K``    N-EKDOS 1.0 (EKTA)  
``PACK    .PAS   1,2K``      
``PD      .COM    15K``    Printer's Driver v1.0 (H)  
``PIP     .COM   7,3K``    File copier (CP/M)  
``QDISK   .COM   7,2K``    Disk Test (EKTA '85)  
``QRUN    .COM   4,8K``    Quick Test (EKTA '85)  
``RDEM    .COM    30K``    JUKU official demo program (EKTA '87)  
``SED     .COM    10K``    Screen text editor 6.1  
``SID     .COM   7,0K``      
``STAT    .COM   5,2K``      
``SUBMIT  .COM   1,3K``    Command-batch processor (CP/M)  
``TERM    .COM   9,5K``      
``VIRUS   .BAK    768``      
``VIRUS   .TXT    768``      
``XDIR    .COM   2,3K``      

### E5

``DISKTST .TST   1,3K``      
``LSC     .HEX    384``      

## OKSJON02

SIZE: `800K` (`819200`) / SHA1: `1b1ceb9cb450b37413f6ef590feeae1932193afe`

``BUGABOO .COM      0``      
``COPY    .COM   1,5K``      
``CURSOR  .PCC   1,0K``      
``EXTERN  .BAS    256``      
``FTYPE   .COM   8,4K``      
``FX800   .COM   1,8K``    Epson FX-800 printer driver  
``LINKMT  .COM    12K``    Link/MT+ v5.6.1  
``MT      .COM    36K``    Pascal/MT+ v5.6.1  
``MTPLUS  .000    13K``      
``MTPLUS  .001    11K``      
``MTPLUS  .002   7,0K``      
``MTPLUS  .003   7,3K``      
``MTPLUS  .004    17K``      
``MTPLUS  .005   8,5K``      
``MTPLUS  .006   6,2K``      
``PD      .COM    15K``    Printer's Driver v1.0 (H)  
``PORTREE .      6,3K``      
``PROOV   .BAS    256``      
``SDEL    .COM    896``    Selective Delete v2.0  
``SED     .COM    10K``    Screen text editor 6.1  
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  

### 01

``INDY    .BAK    13K``      
``INDY    .TAB    13K``      
``TABEL   .       13K``      

### E5

``????????.DIR    384``      
``DISK    .ERL    384``      
``DISK    .H      256``      
``ERROR   .COM   5,7K``      
``FPREALS .ERL   7,5K``      
``FTYPE   .ERL    768``      
``GRAPH   .H      512``      
``INDY    .BAK    13K``      
``KEYB    .ERL    512``      
``PRINT   .ERL   1,7K``      
``PRINT   .H     3,3K``      
``SCREEN  .H      768``      
``SCREEN  .HH     768``      
``SPRITE  .H1     384``      
``SPRITE  .H2     384``      
``TABEL   .DCD      0``      
``TRANCEND.ERL   3,3K``      
``UTILIT  .ERL    768``      
``UTILIT  .H      384``      
``XXX     .       768``      

## OKSJON03

SIZE: `800K` (`819200`) / SHA1: `68a097591cf2ac4dafdd7a5a55c498241b0dd7ab`

``9       .      3,9K``      
``9       .BAK   3,9K``      
``9       .SYP   3,9K``      
``9       .COM    26K``      
``9       .ERL   4,3K``      
``9       .SYP   4,3K``      
``9       .PRN   8,3K``      
``9       .SYP   8,3K``      
``BUSINESS.BAS   8,3K``      
``CF      .COM   1,0K``    File copy 1.0 (EKTA '89)  
``CURSOR  .PCC   1,0K``      
``DISK    .ERL    384``      
``DISK    .H      256``      
``FPREALS .ERL   7,5K``      
``GRAPH   .ERL   2,0K``      
``GRAPH   .H      512``      
``KEYB    .ERL    512``      
``KEYB    .H      512``      
``KEYC    .ERL    640``      
``KEYC    .H1     128``      
``KEYC    .H2     640``      
``LINKMT  .COM    12K``    Link/MT+ v5.6.1  
``MOULD   .COM   9,2K``      
``MTPLUS  .000    13K``      
``MTPLUS  .001    11K``      
``MTPLUS  .002   7,0K``      
``MTPLUS  .003   7,3K``      
``MTPLUS  .004    17K``      
``MTPLUS  .005   8,5K``      
``MTPLUS  .006   6,2K``      
``MTPLUS  .COM    36K``    Pascal/MT+ v5.6.1  
``PACK    .PAS   1,2K``      
``PASLIB  .ERL    25K``      
``PRINT   .ERL   1,7K``      
``PRINT   .H     3,3K``      
``SCREEN  .ERL    896``      
``SCREEN  .H      768``      
``SPRITE  .ERL   2,8K``      
``SPRITE  .H1     384``      
``SPRITE  .H2     384``      
``TRANCEND.ERL   3,3K``      
``UTILIT  .ERL    768``      
``UTILIT  .H      384``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  
``XGRAPH  .ERL   1,9K``      
``XGRAPH  .H      768``      
``YHEKSA  .BAK    896``      

### 01

``INDY    .DAT    12K``      
``TEKST   .$$$      0``      

### E5

``9       .COM   8,8K``      
``9       .SYP      0``      
``STR     .       256``      
``STR     .COM   4,2K``      
``STR     .ERL    384``      
``STR     .SYM    256``      
``STR     .SYP      0``      

## OKSJON04

SIZE: `400K` (`409600`) / SHA1: `34860b8a9e718588ec4a4cb636c2053ec08ee433`

``ASM     .COM   8,0K``    Assembler 2.0 (CP/M)  
``B80     .COM    24K``    BASIC-80 5.21 (Microsoft '81)  
``BASCOM  .COM    32K``    BASIC compiler 5.30 (Microsoft)  
``DISK    .ERL    384``      
``FPREALS .ERL   7,5K``      
``FX800   .COM   1,8K``    Epson FX-800 printer driver  
``GRAPH   .ERL   2,0K``      
``LINKMT  .COM    12K``    Link/MT+ v5.6.1  
``MGR     .COM    15K``    Mgr 1.0 (A.Soolo '93)  
``PASLIB  .ERL    25K``      
``RAHA    .BAS   1,5K``      
``REGLEMEN.      2,3K``      
``SCREEN  .ERL    896``      
``SED     .COM    10K``    Screen text editor 6.1  
``SID     .COM   7,0K``    Machine-code debugger SID 1.4 (CP/M)  
``SPRITE  .ERL   2,8K``      
``TRANCEND.ERL   3,3K``      
``UTILIT  .ERL    768``      
``XDIR    .COM   2,3K``    File catalog viewer 3.5 (CP/M)  
``YLES2   .BAS   1,2K``      

### E5

``BASLIB  .$$$      0``      
``LOAD    .$$$      0``      
``LPT1:   .       128``      
``MTERRS  .TXT   4,8K``      
``MTPLUS  .000    13K``      
``MTPLUS  .001    11K``      
``MTPLUS  .002   7,0K``      
``MTPLUS  .003   7,3K``      
``MTPLUS  .004    17K``      
``MTPLUS  .005   8,5K``      
``MTPLUS  .006   6,2K``      
``MTPLUS  .COM    36K``    Pascal/MT+ v5.6.1  
``OTSIME  .         0``      
``PASTEMP .TOK      0``      
``REGLEMEN.BAK   2,4K``      
``RUUTVO2 .COM   3,4K``      
``RUUTVO3 .COM   3,4K``      
``RUUTVO3 .SYM    256``      
``RUUTVO4 .COM      0``      
``RUUTVO4 .SYM      0``      
``RUUTVO4 .SYP      0``      
``RUUTVORR.COM    15K``      
``RUUTVORR.ERL    512``      
``RUUTVORR.SYP      0``      
``SCREEN  .ASM      0``      
``SET     .COM    256``      
``TRIPS   .PAS    896``      

## OKSJON05

SIZE: `400K` (`409600`) / SHA1: `bacab942d6f7cce703449306cec87c85d7efc4a3`

``1994    .PIC   3,4K``      
``1995    .PIC   3,5K``      
``DIAGRAMM.PIC   1,0K``      
``GTR     .COM    27K``      
``IKOONID .PIC   3,0K``      
``IKOON   .PIC   4,5K``      
``KAART   .PIC   4,9K``      
``K\ED    .PCC   1,0K``      
``LEIUTISE.PCD    128``      
``MUSTRID .PCC   1,0K``      
``PATTERN .PIC   7,2K``      
``PEALUU  .PCC   1,0K``      
``PIP∕    .$$$      0``      
``PIP     .COM   7,3K``      
``XDIR    .COM   2,3K``      

## OKSJON06

SIZE: `800K` (`819200`) / SHA1: `e8620ed9392a24463d145d28c0fc76ddac1eeb27`

``CURSOR  .PCC   1,0K``      
``PR      .COM   2,7K``      
``WURMI   .LNK   6,7K``      

## STEF2

A damaged disk found in a JUKU disk drive, recovered by the Museum of Electronics' founder Woldemar on 31 March 2024.
KryoFlux was used to recover the disk, Fluxengine to decode it, and the recovery score is 0/32.

SIZE: `800K` (`819200`) / SHA1: `17eefcd63de191d00059516aacfc16d9abf56400`

``5       .PIC      0``      
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``BUGABOO .COM    18K``    Turnip in the maze (EKTA '89)  
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG   1,4K``      
``BUGABOO .TAB    384``      
``DIR     .PIC    256``      
``DOOM2   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  
``DOOM2   .PIC    256``      
``DUKE    .COM      0``      
``EIT@@TA .COM    17K``      
``EXSIT   .PIC   2,8K``      
``FDMAINT .COM    11K``    Floppy Maintenance 1.1 (EKTA '88)  
``GTR     .COM    27K``    Turbo GTR 2.5B (M.Gladin/EKTA '87)  
``GTR     .PCD    128``      
``GTR     .PIC      0``      
``HOUSE   .PIC    512``      
``HUNTER  .COM   6,8K``    Hunting club (80x24, Vakstu/MIG '86)  
``HUNTER  .DAT    256``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``JJ      .PIC    512``      
``JUKU    .PIC    768``      
``KOPTER3 .COM    256``      
``LOGER   .COM    32K``    Switch logic v1.1 (Nost Neji '90 H)  
``LOPP    .PIC   2,3K``      
``L       .PIC   4,5K``      
``MM      .COM   3,0K``      
``MUSAM   .COM   3,7K``    Piano "Musa Master" (EKTA '89)  
``PRIIT   .       17K``      
``PUSHER  .COM    23K``    "Pusher" (=Sokoban, A.Mett '91)  
``PUSHER  .DAT    17K``      
``PUSHER  .DOK   1,3K``    PUSHER foreword (A.Mett '90)  
``PUSHER  .LEV   6,3K``      
``SAKOOL  .PIC   2,4K``      
``SHOT    .COM   2,3K``    "Shot Master 2000" v1.1 (I.Käär '91)  
``SHOT    .DAT   9,0K``      
``SIGA    .PIC   1,0K``      
``SKA     .PIC   1,9K``      
``SK      .PIC   1,4K``      
``SNAKE   .COM    12K``    "Snake" (M.Gladin/EKTA '87)  
``SNAKE   .DAT   1,0K``      
``S       .PIC   1,4K``      
``TRRTRTFG.PIC      0``      
``TY ROM  .PIC   4,5K``      
``WARCRAFT.COM      0``      
``WE      .PIC   2,8K``      

### E5

``MOIS    .COM   6,8K``    Manor lord's efficiency (=Sumerian)  
``ZOO     .COM    25K``    "Lode Runner" at the zoo (VAKSTU '91)  

## VAKSTU01

An image of the "VSW working disk" was donated by Vahur Sinijärv on 7 June 2022.
The disk has EKDOS 2.29; on boot it shows the customised message `VSW tööketas (c)`.
For background on the VAKSTU series, see https://p6drad-teel.net/~p6der/juku-hingeelu_2024.pdf
(slide 27ff).

SIZE: `800K` (`819200`) / SHA1: `b7efca324ddffc6c31476adff2228e3b5e2e792e`

``3VMUSIC .ASM    29K``      
``ASCII   .       896``      
``ASM     .COM   8,0K``    Assembler 2.0 (CP/M)  
``CHECK   .ASM   2,3K``      
``CHECKSUM.ASM    512``      
``CHECKSUM.HEX    256``      
``CMON    .COM   4,3K``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``COSMIC  .BAS   6,5K``      
``CP/M    .COD    10K``      
``DISASM  .COM   8,3K``    Super CP/M disassembler 4.00 ('78)  
``EASYSTR .LAD   1,5K``      
``FUNDSK  .ASM    768``      
``GAMEPRAC.ASM    20K``    SPACE ATTACK source code (Vakstu '91)  
``GAMEPRAC.COM   4,5K``      
``GRBASIC .COM   7,8K``      
``GRMOOD  .ASM   3,0K``      
``GRMOOD  .COM    256``      
``GTRDOS30.ASM    13K``      
``GTRDOS30.BAK    13K``      
``GTRDOS30.HEX   2,9K``      
``GTRDOS30.PRN    23K``      
``GTRDOS30.REL   1,3K``      
``GTRDOS30.SYM   1,9K``      
``GTRDOS  .BAK    256``      
``GTRDOS  .HEX      0``      
``GTRDOS  .SYM    384``      
``H2      .ASM    640``      
``HIIR    .ASM   1,8K``      
``INBYT   .ASM    256``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``KETAS   .ASM   1,4K``      
``KETAS   .COM    640``      
``L80     .COM    11K``    LINK-80 3.44 (Microsoft '81)  
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADTAB  .COM    12K``    Ladder level editor (VAKSTU '90)  
``LADTAB  .PAS   2,7K``    Ladder editor source code  
``LASER   .MAC    128``      
``LINK    .COM    16K``    Object-module linker 1.3 (CP/M '80)  
``LIST    .ASM   1,8K``      
``LOAD    .COM   1,8K``    HEX to COM converter (CP/M)  
``LODEGEN .MAC   6,5K``    ZOO editor source code (VAKSTU '91)  
``LODERUN .MAC    20K``    ZOO assembly source code (VAKSTU '91)  
``M80     .COM    20K``    Macro-80 3.44 (Microsoft '81)  
``MAC     .COM    12K``    Macro Assembler 2.0 (CP/M)  
``MALE    .MOD   5,0K``      
``MARGID  .PAS   1,5K``      
``MARKT   .COM    21K``      
``MERGE   .ASM   4,7K``      
``MODE    .ASM    384``      
``MUS     .MAC    128``      
``OUTBYT  .ASM    128``      
``PALL    .ASM    768``      
``PIIP    .MAC    128``      
``PILT    .COM    19K``      
``PILT    .PAS    896``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``PLAYER  .ASM   2,4K``      
``PLAYER  .COM    384``      
``PMOOD   .ASM   3,7K``    GTR image-reading module  
``PMOOD   .COM   1,0K``      
``PMOOD   .MAC   3,7K``      
``READ    .COM   7,8K``      
``READ    .PAS    256``      
``SAT-TV  .PAS    256``      
``SBAAS   .COM   7,5K``      
``SBASIC  .COM   7,5K``      
``SCPROOV .ASM    512``      
``SCPROOV .COM    128``      
``SCREDIT .ASM   4,2K``      
``SCREDIT .COM    768``      
``SCREDIT .MOD    512``      
``SCROLL  .ASM   1,2K``      
``SED     .COM    10K``    Screen text editor 6.1  
``SEQIO   .LIB    11K``      
``SID3    .COM   7,8K``    Machine-code debugger SID 3.0 (CP/M)  
``SID     .COM   7,0K``    Machine-code debugger SID 1.4 (CP/M)  
``SIDT    .COM   7,7K``    Machine-code debugger SIDT 2.1 (EKTA '85)  
``SOKO    .ASM    128``      
``SOKO    .COM    640``      
``SOKO    .MAC    384``      
``SPAC    .COM    17K``      
``SPACE   .COM    17K``    "Space Attack" (Vakstu/VSW '90)  
``SPRITE  .ASM    128``      
``SPRITE  .COM    256``      
``SSBAS   .COM   7,5K``      
``ZOO     .PLT    22K``    ZOO main menu background image  
``ZOO     .TAB   4,3K``    VAKSTU design and M-K levels  
``TRAPS   .COM   2,5K``      
``TRIPS   .COM    16K``      
``TYPER   .ASM   1,4K``      
``TYPER   .COM    256``      

### E5

``JALG    .PCC   1,0K``      
``KAST    .PCC   1,0K``      
``KEHA    .PCC   1,0K``      
``KOHT    .PCC   1,0K``      
``LODERUN .$$$    16K``      
``MEES    .PCC   1,0K``      
``PMOOD   .ASM   3,7K``      
``PMOOD   .PRN   7,8K``      
``PUNKT   .PIC    128``      
``REI     .PCC   1,0K``      
``RUUT    .PCC   1,0K``      
``SEIN    .PCC   1,0K``      
``SIHTP   .PCC   1,0K``      

## VAKSTU02

Physical floppies from the VAKSTU series were handed over for reading by Kalle Tomingas
in December 2024. Of the seven floppies, three were JUKU disks, two of which were read
without problems. The second disk of the series, `VAKSTU02`, contains no OS and was read
with errors — both sides have an estimated 133 bad sectors in total and 58% of the disk
was recovered. The floppies were read using Greaseweazle together with a TEAC floppy drive.

SIZE: `800K` (`819200`) / SHA1: `05cdb99b04b1972118acf95119cda4a7dd297c82`

``3VMUSIC .COM   6,3K``      
``ADDR    .ASM   1,0K``      
``ASM     .      4,2K``      
``AVTEST  .COM    14K``      
``BEEP    .ASM    896``      
``BOW     .COM    12K``      
``CE      .ASM   1,2K``      
``CODE    .ASM    640``      
``COPY    .ASM   2,9K``      
``CPFH80  .COM    512``      
``DEMO    .      8,2K``      
``DEMO    .COM   5,2K``    Audio-Video-Text demos (EKTA '88)  
``DEMO    .HLP   3,5K``    DEMO help file  
``DIGGER  .COM   1,2K``    Viral star shower (K.Tomingas '91)  
``DISASM  .COM   8,3K``      
``DTTEST  .COM    14K``      
``EXER1   .CLG    128``      
``GOLO    .COM    11K``      
``GRAPH   .       896``      
``GRDEMO  .COM    20K``      
``H2      .ASM    384``      
``HELP    .SYM   1,2K``      
``HIIR    .COM    512``      
``KAOTAJA .COM    12K``      
``KAP     .COM    32K``    "Battleship" (ed K.Koppel)  
``KAPU    .BAS    19K``    "Battleship" source code  
``KETAS   .ASM   1,4K``      
``KETAS   .COM    640``      
``KULT    .COM    12K``      
``KUMMARDA.PAS    640``      
``KUVA    .COM    768``      
``KYU     .      2,8K``      
``L1      .ASM   9,9K``      
``LADTAB  .COM    12K``    Ladder level editor (VAKSTU '90)  
``LF      .ASM    15K``      
``LF      .COM   2,0K``      
``LISATEEK.       27K``      
``LOAD1   .ASM   1,0K``      
``LOAD2   .ASM   6,4K``      
``LOGER   .      5,3K``      
``LOGER   .COM    32K``      
``LUKK    .$$$    128``      
``M80     .COM    20K``      
``MARGID  .PAS   1,5K``      
``MAUMAU  .COM   2,5K``      
``MODE    .ASM    896``      
``MODX    .COM   3,5K``      
``MOUSE   .ASM   2,7K``      
``MR      .ASM   2,7K``      
``MVDOS   .ASM    512``      
``OP      .ASM   3,4K``      
``PALL    .COM   1,7K``      
``P       .ASM   9,5K``      
``PLAY    .ASM   1,5K``      
``PLAYER  .ASM   2,5K``      
``PMOOD   .ASM   3,7K``      
``PORKA   .COM    13K``      
``POWER   .       28K``      
``PRT     .COM   4,0K``      
``PS      .COM    15K``      
``RAKETT  .COM    11K``      
``RALLY   .ASM    768``      
``R       .ASM   1,3K``      
``RCOPY   .COM    14K``      
``RG      .ASM   1,9K``      
``RS      .MAC   2,4K``      
``S       .ASM    512``      
``SEIKO   .COM   1,8K``    Seikosha SP-800 driver  
``SP      .ASM    256``      
``SPEED   .ASM   1,8K``      
``SPEEDY  .PAS   1,2K``      
``STJUKU  .COD    16K``      
``STOP    .ASM    640``      
``STOP    .COM    128``      
``SY      .ASM    12K``      
``SYMB    .PAS   1,5K``      
``SYNT    .ASM    12K``      
``SYSINFO .COM   1,2K``    Basic system info (CP/M)  
``TANK    .COM    15K``    Tank vs. UFOs (=Sabotage/Invaders)  
``TEST    .COM    16K``      
``TIMER   .ASM   1,3K``      
``TRANS   .ASM    128``      
``TRIPS   .COM    512``      
``TURMIIT .COM   7,4K``      
``V1      .ASM   1,2K``      
``VIIR1   .ASM    768``      
``VVV     .COM   7,5K``      
``YL0     .LOG    256``      
``YL1     .LOG    896``    LOGER task #1  
``YL2     .LOG    640``      
``YL3     .LOG    896``      
``YL4     .LOG   1,7K``    LOGER task #4  
``YL5     .LOG    768``      

## VAKSTU05

A VAKSTU-series floppy handed over for reading by Kalle Tomingas in December 2024. The
disk has EKDOS 2.29; on boot it shows the customised messages `VSW tööketas (c)` and
`SKC-Floppy Disk`, and the `DIR` command is disabled. For more about the series see the
descriptions of the earlier floppies.

SIZE: `800K` (`819200`) / SHA1: `b91edfdbee67cee8fed9429340f2a72140e576e3`

``3VMUSIC .COM    12K``    Music Editor 1.0 (Vakstu '91)  
``3VMUSIC .MAC    29K``      
``AASTA   .KEM    640``      
``AB      .COM    20K``      
``ABI     .COM    20K``      
``ABI     .TAB    16K``      
``AEG     .COM   9,4K``      
``ARVUTA  .COM    14K``      
``ASM     .      4,2K``    Assembly instruction table  
``BIORYTM .COM    18K``      
``BOWLING .COM   3,5K``    Bowling (Maxway & I.K.S. '91)  
``COF     .COM    640``    Copy files 6.6 (I.Käär)  
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``CONV    .PAS   1,9K``      
``CSPRITE .COM    12K``      
``DISK    .H      512``      
``GRAAF   .COM    13K``      
``GRAPH   .H      768``      
``GRLIB   .ERL   8,2K``      
``ISO     .COM    13K``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``KAST    .PCC   1,0K``      
``KEEMIA  .HLP   1,2K``      
``KEEMIA  .KEM   2,3K``      
``KELEMENT.COM    29K``      
``KOHT    .PCC   1,0K``      
``KRAK    .COM    14K``      
``KRAKOUT .PAS   1,8K``      
``KRAK    .PAS   2,2K``      
``KUMMARDA.PAS    640``      
``KUM     .PCC   1,0K``      
``LAD2    .DAT    512``      
``LADDER2 .COM    40K``    Platformer Ladder 2 (Yahoo '83)  
``LADDER2 .FNT    896``    Ladder graphics as a font table  
``LADTAB  .PAS   2,7K``    Ladder editor source code  
``LA      .TAB    128``      
``LI      .      1,9K``      
``LINNAD  .COM    18K``      
``LODEGEN .COM   1,3K``    Zoo level editor (V.Zverkov '90)  
``LR      .COM    13K``    ZOO preliminary version (single level)  
``MAT     .       384``      
``MATICO  .COM    19K``      
``MEES    .PCC   1,0K``      
``MENDEL  .COM    18K``      
``MENDEL  .DAT   1,9K``      
``MFD     .COM   2,3K``    Dumper \w music (I.K.S/Writer)  
``MIC     .COM   3,8K``    Micro-editor 1.0 (EKTA '88)  
``MUSUBI  .PCC   1,0K``      
``MUUTUJAD.TST    896``      
``NIELS   .COM    22K``      
``PALL    .PCC   1,0K``      
``PMOOD   .ASM   3,7K``      
``PMOOD   .REL    640``      
``PORKA   .PAS   1,4K``      
``PRT     .COM   4,0K``    Print file utility 5.3  
``PS1     .COM   7,0K``      
``PULK    .PCC   1,0K``      
``PUSHER  .COM    23K``    "Pusher" (=Sokoban, A.Mett '91)  
``PUSHER  .DAT    17K``      
``PUSHER  .LEV   6,3K``      
``PUSHERPK.COM    16K``    Pusher level packer  
``REI     .PCC   1,0K``      
``RUUT    .PCC   1,0K``      
``SCREEN  .H     1,0K``      
``SCSOUND .COM    256``      
``SED     .COM    10K``    Screen text editor 6.1  
``SEIN    .PCC   1,0K``      
``SHOT    .COM   2,3K``    "Shot Master 2000" v1.1 (I.Käär '91)  
``SPRITE  .H1     512``      
``SPRITE  .H2     640``      
``STOP    .ASM    640``      
``STOP    .COM    128``      
``SYMBOL  .KEM   5,3K``      
``ZOKOBAN .COM    16K``    Zokoban (Errorsoft/Syntax '91)  
``ZOKOBAN .SIR    128``      
``ZOO1    .COM    16K``    ZOO original version (9 levels)  
``ZOO     .COM    35K``    ZOO unpacked development version  
``TEST2   .       384``      
``TETRIS  .COM    17K``    "Tetris" with mouse (A.Mett '90 H)  
``UTILIT  .H      640``      

## VAKSTU06

A VAKSTU-series floppy handed over for reading by Kalle Tomingas in December 2024. The
disk has EKDOS 2.29; on boot it shows the customised message `TDK Mini-Floppy Disk`. For
more about the series see the descriptions of the earlier floppies.

SIZE: `800K` (`819200`) / SHA1: `8338f674672f38fa9128377f850186c429025835`

``A&A1    .PIC   2,4K``      
``A&A2    .PIC   2,4K``      
``A&A     .PIC   1,2K``      
``AA      .PIC   2,8K``      
``ASCII   .       896``    Latin alphabet font (US layout)  
``AVE     .PLR   2,0K``      
``BACH    .PLR    256``      
``BCLOAD  .       128``      
``BEETHOVE.PLR   2,0K``      
``BIZET   .PLR    256``      
``BRUN    .COM    16K``    BASIC runtime 5.30 (Microsoft)  
``BUGABO  .MSG   1,4K``      
``BUGABOO .COM    18K``      
``BUGABOO .DAT   1,0K``      
``BUGABOO .MSG    128``      
``BUGABOO .TAB    384``      
``CATCHUM .COM    29K``    Well-known CP/M PAC-MAN clone\* (80x24)  
``CATCHUM .DAT    512``      
``CHESS   .COM    31K``    Chess game "Let me think" (EKTA '89)  
``COM     .COM   3,0K``      
``COMPU1  .COM   3,0K``      
``COMPU   .COM   1,8K``    Compute Mate 160 printer driver  
``CP∕M    .       10K``      
``DEMOS   .COM   8,3K``    A-V-T demo preparation (EKTA)  
``DOCTOR  .COM    36K``    Disk Editor & Diagnostics 1.11 ('83)  
``DUUR    .PIC   1,8K``      
``EASY    .LAD   1,3K``      
``EASYSTR .LAD   1,5K``      
``EKSINF1 .PIC   2,3K``      
``E       .PLR    256``      
``EVSW    .PIC   1,0K``      
``FDMAINT .COM    11K``      
``FGY     .PIC    896``      
``FTB     .COM   6,5K``      
``GNR     .PIC    512``      
``GRW     .COM    896``      
``GTR     .COM    27K``      
``GTR     .PCC      0``      
``JCM     .COM    12K``    JUKU File/Copy Master 1.0 (EKTA '89)  
``KAR     .PLR    384``      
``KAST    .PCC   1,0K``      
``KLAVER  .PIC   3,9K``      
``KOMP    .PLR    256``      
``KRAKOUT .SYM    768``      
``KUM     .PCC   1,0K``      
``KUVA    .COM    768``      
``LAD     .       896``    Ladder graphics as a font table  
``LADD    .COM   7,5K``      
``LADDEN  .COM    40K``      
``LADDEN  .DAT    512``      
``LADDER  .COM    40K``    Platformer LADDER (80x24, Yahoo '83)  
``LADDER  .DAT    512``      
``LAEV    .PCC   1,0K``      
``LAMBA   .PLR    384``      
``LEEK1   .PCC   1,0K``      
``LEEK2   .PCC   1,0K``      
``LF      .ASM   1,7K``      
``LF      .COM   2,0K``    Font loader for MODX  
``LIFESTYL.PIC    768``      
``MAURO   .PLR   1,5K``      
``ME      .COM    32K``    Sound editor "Music Editor" 2.4 ('89)  
``MEES    .PCC   1,0K``      
``MEMEDIT .PIC   3,9K``      
``MM      .PIC    384``      
``MODX    .COM   3,5K``    80x24 screen-mode driver  
``MODX    .PRN      0``      
``MONALISA.      5,0K``      
``MOTA    .PIC   1,2K``      
``MOTO    .PIC   1,4K``      
``MTEST   .COM   8,4K``    Memory test 2.1 (K.Tomingas/VSW '91)  
``MTLLC   .PIC    256``      
``MTV     .PIC    768``      
``MUSAM   .COM   3,7K``    Piano "Musa Master" (EKTA '89)  
``MUSA    .PIC    128``      
``N       .PLR    512``      
``PACIUS  .PLR    256``      
``PATTERN .PIC   7,2K``      
``PBODY   .PCC   1,0K``      
``PIP     .COM   7,3K``    File copier (CP/M)  
``PLAYER  .COM    384``      
``POWER   .COM    15K``      
``RDEM    .PIC   1,7K``      
``RDIR    .COM    896``      
``RTL     .PIC    256``      
``RUUT    .PCC   1,0K``      
``SC      .PIC   1,8K``      
``SCSOUND .COM    256``      
``SED80   .COM    10K``    Screen text editor 6.1 (80x24)  
``SED     .COM    10K``      
``SEIN    .PCC   1,0K``      
``SH      .PCD    128``      
``SID     .COM   7,0K``    Machine-code debugger SID 1.4 (CP/M)  
``SIDT    .COM   7,7K``    Machine-code debugger SIDT 2.1 (EKTA '85)  
``SK      .COM   4,0K``      
``SOKO    .PIC   3,9K``      
``SPACE   .COM    17K``    "Space Attack" (Vakstu/VSW '90)  
``SPACE   .PIC   3,0K``      
``SPRITES .PIC   2,2K``      
``SS      .PIC    384``      
``TEST    .COM   5,2K``    Memory test, 20 iterations (K.Tomingas '91)  
``T       .PCC   1,0K``      
``TX      .PCC   1,0K``      
``VALGRE  .PLR    256``      
``VIIR    .COM    256``      
``VSW     .PIC   1,9K``      
``WAR     .PIC   5,9K``      
``XONIX   .COM   3,8K``    "Qix" clone (E.Jürviste/EKTA '87)  
``XTC     .PIC    512``      
``YDAY    .PLR    256``      

