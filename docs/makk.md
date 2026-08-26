# Instructions for using the cassette-recorder utilities

Abbreviations:

`MLOS` — unmanaged tape OS  
`JLOS` — managed tape OS  
`CP/M` — standard disk OS  
`BLOS` — base tape OS  

Programs:

|              | Purpose |
| ------------ | ------- |
| `FORM  .COM` | Format a tape and write the system |
| `COPA  .COM` | Copy `CP/M` → `JLOS`, `JLOS` → `CP/M`, and `CP/M` → `CP/M` |
| `COPM  .COM` | Copy `CP/M` → `MLOS`, `MLOS` → `CP/M`, and `CP/M` → `CP/M`<br>When run under `JLOS`, also `JLOS` → `MLOS` and `MLOS` → `JLOS` |
| `GENA  .COM` | Generate JLOS |
| `GENM  .COM` | Generate MLOS |
| `ATOS  .SYS` | Managed tape OS<br>(not a load module) |
| `MTOS  .SYS` | Unmanaged tape OS<br>(not a load module) |
| `SETS  .COM` | Display and change file statuses |

## `FORM.COM`

A program for formatting JLOS tapes and writing the system. It can be run under `CP/M`, `JLOS`, and `MLOS`.

`FORMAT` — format the tape.

* How many blocks should be written? If the answer is 0, the blocks must already have been written.
* How many blocks should be read? At least 8 blocks must be read.
* Verify the catalogue? After the catalogue is written to tape, it is read back and compared. If verification finds errors, the catalogue can be written to the tape again.
* Write the system? If an OS has been loaded with `LOAD`, the user can also write the system to tape after formatting.
* Verify the system? Verify the system that was written.

`SYSGEN` — write the system to tape.

* If the system is already loaded into memory, insert the tape on which it is to be saved.
* If the system has not been loaded, first read it from a system tape, then change tapes and save it.

`LOAD` — load a tape OS from a disk/tape file into memory.

* OS for a managed cassette recorder: `ATOS.SYS`
* OS for an unmanaged cassette recorder: `MTOS.SYS`

`EXIT` — exit the program.

* `Ctrl-ESC` always returns to the program's main menu.
* This program can also create `MLOS` system tapes: format only the first 8 blocks and save the `MLOS` system (`MTOS.SYS`).
* The program can also be run under `MLOS` to format tapes and put systems on them.
* If the program was started under `JLOS`, before exiting place in the cassette recorder the tape that was open when the program started.

## `COPA.COM`

A program for copying files from disk to managed tape, tape to disk, and disk to disk. It can only be run under `CP/M`.

|               | Purpose |
| ------------- | ------- |
| `O - (OPEN)`  | Open the tape catalogue. |
| `L - (CLOSE)` | Close the tape catalogue; the catalogue remains open. |
| `D - (DIR)`   | Display the disk/tape catalogue.<br>`A...D` — disk drive<br>`T` — tape |
| `E - (EXIT)`  | Exit. If a tape is open, the program asks whether to close it. |
| `R - (RESET)` | Rewind the tape and reset the disks. |
| `C - (COPY)`  | Copy files. First enter the source file name. If the file is not found, a message is displayed. Entering no name returns to the main menu. Next enter the destination file name (it may consist of only a device designator; the source name is then copied automatically). If the file already exists, the program asks whether to overwrite it. A negative answer prompts for the name again; a positive answer overwrites the file, even if its status is `R/O`.<br>File names may use these device designators:<br>`A...D` — disk drive<br>`T` — tape<br>If omitted, the default device is used. |

## `COPM.COM`

A program for copying files from disk to unmanaged tape, tape to disk, and disk to disk. It can be run under `CP/M`, and by an experienced user also under `JLOS`. Its dialogue is analogous to `COPA.COM`.

## `GENA.COM`

A program for writing the managed tape OS. It can be run under `CP/M` and `JLOS`.

* Insert the source tape (the tape containing the system).
* After the system has been read, insert the tape on which it is to be written.
* Note: when exiting under `JLOS`, insert the tape that was open when the program started.
* `Ctrl-ESC` always returns control to the program.
* `Ctrl-C` interrupts the program.

## `GENM.COM`

A program for writing the unmanaged tape OS. It can be run under `CP/M`, `JLOS`, and `MLOS`.

When using `COPM.COM` and `GENM.COM`, the following messages are displayed:

|               | Meaning |
| ------------- | ------- |
| `Set to Mtos` | Initialise the unmanaged tape OS: remove the cassette-recorder control cable from socket `X4`. |
| `Set to Atos` | Initialise the managed tape OS: connect the cassette-recorder control cable to socket `X4`. |

## `SETS.COM`

A program for displaying and changing file statuses. It can be run under `CP/M` and `JLOS`. Under `JLOS`, displaying file statuses also shows the file's location (first and last block and length).

```
A>SETS [filename] [status]
```

|         | Values |
| ------- | ------ |
| status: | `R/W` — file can be read and written<br>`R/O` — read-only file<br>`DIR` — non-system file<br>`SYS` — system file |

## JLOS functions

|                 | Purpose |
| --------------- | ------- |
| `DIR [f]`       | List files |
| `REN f1=f2`     | Rename a file<br>`f1` — new name<br>`f2` — old name |
| `ERA f`         | Delete files |
| `REST f`        | Restore a deleted file |
| `MEM`           | Display general tape-space usage information |
| `TYPE f`        | Display a text file |
| `DUMP f`        | Display file contents in hexadecimal |
| `LOAD f [a]`    | Load a file into RAM<br>`a` — start address (default `100H`) |
| `RUN [p1] [p2]` | Run the program in memory; parameters are stored in file control blocks |
| `SAVE n f [a]`  | Save memory contents to a file<br>`n` — number of 2K-byte blocks<br>`a` — start address (default `100H`) |
| `CLOSE`         | Write the catalogue to tape; the catalogue remains open |
| `OPEN`          | Read the catalogue from tape into memory |
| `MONID`         | Exit the OS to the monitor |
| `HELP`          | List resident functions |
| `CHECK`         | Display system information and calculate a new catalogue checksum |
| `DUMP ;a`       | Display RAM in hexadecimal<br>`a` — start address |
| `SAVE ;a`       | Modify RAM<br>`a` — start address |

`Ctrl-C` interrupts execution of a function.

## Working with JLOS

The managed tape OS is operated in the same way as the standard `CP/M` disk OS.

## MLOS functions

|                 | Purpose |
| --------------- | ------- |
| `DIR`           | List blocks |
| `TYPE f`        | Display a text file |
| `DUMP f`        | Display file contents in hexadecimal |
| `LOAD f [a]`    | Load a file into RAM<br>`a` — start address (default `100H`) |
| `BLOAD [a]`     | Load blocks into RAM<br>`a` — start address |
| `RUN [p1] [p2]` | Run the program in memory; parameters are stored in file control blocks |
| `SAVE n f [a]`  | Save memory contents to a file<br>`n` — number of 2K-byte blocks<br>`a` — start address (default `100H`) |
| `MONID`         | Exit the OS to the monitor |
| `HELP`          | List resident functions |
| `DUMP ;a`       | Display RAM in hexadecimal<br>`a` — start address |
| `SAVE ;a`       | Modify RAM<br>`a` — start address |

`Ctrl-C` interrupts execution of a function.

## Working with MLOS

When searching for a file (with `LOAD`, `TYPE`, `DUMP`, or while launching a load module), the headers of blocks that do not belong to that file are displayed.

If a user program uses `BLOS` function 17 (find file) or 18 (find next file), the following question is displayed on the first line:

> `FILE EXIST(Y/N)` (Does the file exist?)

An affirmative answer means that a file with the requested name is assumed to be already present on the tape.

When function 20 (read a 128-byte block) or 42 (read a 2K-byte block) is invoked, the following text flashes on the first line for a few seconds: `SWITCH TO READING`. This means that the cassette recorder must be switched to playback mode.

If `CHECKSUM ERROR` is displayed while reading from tape, rewind the tape a little before retrying that block.

When function 21 (write a 128-byte block) or 43 (write a 2K-byte block) is invoked, the following text flashes on the first line for a few seconds: `SWITCH TO RECORDING`. This means that the cassette recorder must be switched to recording mode.

If `STOP THE TAPE` flashes on the first line, stop the tape.

`DIR` displays a 2K-byte block header:

> `n` `name` `m`

|        | Meaning |
| ------ | ------- |
| `n`    | Block number |
| `name` | File name |
| `m`    | Number of the file's first block |

When reading a managed tape:

|        | Meaning |
| ------ | ------- |
| `n`    | Absolute block number |
| `name` | File name if the block belongs to a file; tape name if it is an empty block |
| `m`    | `0` if the block does not belong to a file; otherwise the file's first block number |

When reading an unmanaged tape:

|        | Meaning |
| ------ | ------- |
| `n`    | Block's sequence number within the file (starting at 0) |
| `name` | File name |
| `m`    | Always `0` |

If no block header is found after reading the tape for 1.5 minutes, the error `TIME OUT` is displayed, meaning that the tape is empty.

## Connecting the cassette recorder

The computer set includes a cable for connecting the cassette recorder. With a managed recorder, computer sockets `X5` and `X4` are used for data transfer and recorder control respectively. The recorder must not be in pause mode. With an unmanaged recorder, disconnect the cable from socket `X4`.
