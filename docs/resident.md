# Instructions for using the `JLOAD.LDR` resident-program loader

1. The program to be made resident must contain a unique identifier used to determine whether the program is already resident in memory. The identifier must be the fourth byte of the program. For example:

```
START:: jmp   INIT
ID:     db    08h  ; Identifier
INIT:   mov .....  ; The program itself
        .
        .
        .
```

2. Assemble the program with `M80`, then link it with `LINK` using the `[op]` option. For example:

```
M80 DRIVER.ERL=DRIVER.MAC
LINK DRIVER.ERL [op]
```

When `LINK` has finished, a file with the `.PRL` extension will appear on the disk.

3. The resulting `.PRL` file must be combined with the `JLOAD.LDR` resident-program loader using `SID`. From within `SID`, load `JLOAD.LDR`, then load the resident program (the `.PRL` file) at address `167h`. For example:

```
A>sid

­#ijload.ldr
­#r
­#idriver.prl
­#r167
```

The loader and the program to be loaded are now together in memory, forming the final program, which must be saved to disk with the CP/M `SAVE` command. The amount to save can be determined by examining the memory contents in `SID`. Since the `.PRL` file ends with a large number of hexadecimal `1A` bytes, the end of the program is fairly easy to locate. Once it is clear how much must be written to disk, exit `SID` (`CTRL-C`) and save the final program with a `.COM` extension. For example:

```
A>save <n> driver.com
```
