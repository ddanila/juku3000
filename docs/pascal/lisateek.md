# Pascal/MT+ extension library package for the "JUKU" computer

```

                   *****  Nõo 1990  *****




       

               PASCAL/MT+ EXTENSION LIBRARY PACKAGE

                      FOR THE "JUKU" COMPUTER.



                                         Author: I.Jentson

                                                Nõo KK AK

```

## Preface

Using the package assumes basic knowledge of the Pascal language and
the ability to work with the Pascal/MT+ translator. To acquire basic
knowledge of Pascal, you can use, for instance, the textbook[^2], but
any book covering Pascal is also suitable. Some information on using
Pascal/MT+ on the "Juku" computer is given in[^1]; a more detailed
overview of its use and of Pascal/MT+'s differences from standard
Pascal is given in[^3].

When designing the package, an effort has been made to ensure that
the function names match the analogous functions in Turbo Pascal.



## 1. Overview of the libraries


The Pascal/MT+ extension libraries contain procedures and functions
for graphical work on the "JUKU" computer's display, as well as for
choosing the text-mode display, and for working with disks, the
timer, the printer, the "mouse", and so on.

To use all of these procedures and functions, make sure the
following files are present:

     Graph.H        Graph.ERL
     Screen.H       Screen.ERL
     Utilit.H       Utilit.ERL
     Sprite.H1      Sprite.H2      Sprite.ERL
     Disk.H         Disk.ERL

The file `SPRITE.H1` contains type declarations for the sprite procedures:

```
Type _pointer = ^byte;         
          pic = record             A sprite is characterised by:
                    x : integer;   the x-coordinate of its location
                    y : integer;           y-coordinate
                 xdim : byte;      x-dimension ( pixels/8+1 )
                 ydim : byte;      y-dimension
                place : _pointer;  location in memory
                shift : _pointer   offset (don't touch!)
               end;
        bfail = file of byte;
```

The other files with the `.H` extension hold Pascal-language declarations of
the functions and procedures provided by the package; files with the `.ERL`
extension hold modules ready for linking against them.


The following procedures and functions are in the libraries:

     Graphics library:                       ( Graph )

     BOX                 CIRCLE              INVSCR
     LINE                LINETO              LINEREL             
     MOVETO              MOVEREL             PUTPIXEL            
     SETHGR              SETTEXT

     Display formatting library:             ( Screen )

     CLREOLN             CLREOSCR            CLRSCR
     CLOSEWND            CURSOFF             CURSON
     DOWN                GOTOXY              HOME
     INVERSE             KBEEPOFF            KBEEPON
     LEFT                NORMAL              OPENWND
     READKEY             RIGHT               SCREEN
     SCROLOFF            SCROLON             UP
     WHEREXY

     Miscellaneous:                          ( Utilit )

     INITPR              MOUSE               PRCHR
     RANDOM              RSTTIMER            SOUND
     TIMER               VOLUME

     Sprite library:                         ( Sprite )

     GETMEM              GETPIC              LOADPIC
     MOVEPIC             PUTPIC

     Disk library:                           ( Disk )

     READDISK            SELECTDISK          SETDMA
     SETSECTOR           SETTRACK            WRITEDISK


## 2. Using the libraries


### 2.1  Additions to the user program

To your own program, you need to add the type and procedure
declarations for the extension-library routines. This is done with
the compile-mode switch `$I`, which inserts the Pascal text from
files with the `.H` extension into the program.

EXAMPLE:

```
  program example;
  (*$I a:sprite.h1 *)          type declarations are added

  ......                       declarations of the user
  ......                       program's labels, constants,
  ......                       types and variables

  (*$I a:sprite.h2 *)          procedure declarations are
  (*$I a:graph.h *)            added

  ......                       user procedure and function
  ......                       declarations

  begin
  ......                       main program
  ......
  end.
```


### 2.2 Linking

You must add the corresponding `.ERL` file to the list of parameters
in the link command:

```
LINKMT EXAMPLE,SPRITE,GRAPH,PASLIB/S
```

## 3. Procedures and functions

For every function and procedure, information is presented in the
following form:


    FUNCTION_NAME

   Description: Pascal-language description of the function.

         Usage: Form of the function call. Parameter types
                are given in the description; in addition,
                the following coding by the first letter of
                the parameter is used:
                  n - integer expression;
                  c - character expression;
                  m - integer variable;
                  l - boolean variable;
                  b - variable of a file of bytes;
                  p - sprite-type ( pic ) variable.

        Action: Explanation of the function's action and its
                parameters.

          Note: If the function has any peculiarities, attention
                is drawn to them. References to other functions
                are also given where appropriate.




### 3.1 Graphics library (`GRAPH`)

#### `SETHGR`

   Description: Procedure SetHgr;

         Usage: SetHgr;

        Action: Selects graphics mode.

          Note: All procedures that use monitor
                functions do not work in this mode.

                See also SetText.

                 
#### `SETTEXT`

   Description: Procedure SetText;

         Usage: SetText;

        Action: Selects text mode. In this mode, the
                monitor functions can be used.

          Note: The graphics procedures do not work in this
                mode.

                See also SetHgr.







#### `PUTPIXEL`

   Description: Procedure PutPixel( X,Y,Mood:Integer );

         Usage: PutPixel(nx,ny,nm);
                
        Action: Draws one point on the screen. The point is
                drawn on the screen according to the
                coordinates X and Y. MOOD can be 0 or 1. When
                a new point is placed on top of an existing
                one, with mode 1 the point disappears, with
                mode 0 it stays. The X-coordinate may take
                values from 0 to 319, and the Y-coordinate
                values from 0 to 239. With coordinates above
                or below the screen, nothing happens; with
                coordinates to the left or right, the point
                is drawn on the opposite edge of the screen.
                The values X and Y are kept as the graphics
                cursor's values.

          Note: Works in graphics mode and screen modes
                0 and 1 (see SetHgr and Screen).



#### `LINE`

   Description: Procedure Line( X1,Y1,X2,Y2,Mood:Integer );

         Usage: Line(nx1,ny1,nx2,ny2,nm);

        Action: Draws a line on the screen. The line is drawn
                with start point X1,Y1 and end point X2,Y2.
                The meaning of the Mood parameter is
                explained for the PutPixel procedure.

          Note: Works in graphics mode and screen modes
                0 and 1 (see SetHgr and Screen).

#### `CIRCLE`

   Description: Procedure Circle( X,Y,R,Mood:Integer );

         Usage: Circle(nx,ny,nr,nm);

        Action: Draws a circle on the screen. The circle is
                drawn on the screen with centre X, Y and
                radius R.
                The meaning of the Mood parameter is
                explained for the PutPixel procedure.

          Note: Works in graphics mode and screen modes
                0 and 1 (see SetHgr and Screen).








#### `BOX`

   Description: Procedure Box( X1,Y1,X2,Y2,Mood:Integer );

         Usage: Box(nx1,ny1,nx2,ny2,nm);

        Action: Draws a rectangle on the screen. The
                rectangle is drawn so that the points with
                coordinates X1, Y1 and X2, Y2 mark the
                opposite corners of the rectangle's diagonal.
                The meaning of the Mood parameter is
                explained for the PutPixel procedure.

          Note: Works in graphics mode and screen modes
                0 and 1 (see SetHgr and Screen).



#### `LINETO`

   Description: Procedure LineTo( X,Y,Mood:Integer );

         Usage: LineTo(nx,ny,nm);

        Action: Draws a line on the screen. The line is drawn
                with a start point determined by the graphics
                cursor and end point X, Y.
                The meaning of the Mood parameter is
                explained for the PutPixel procedure.

          Note: Works in graphics mode and screen modes
                0 and 1 (see SetHgr and Screen).

                See also MoveTo, LineRel, MoveRel.




#### `MOVETO`

   Description: Procedure MoveTo( X,Y:Integer );

         Usage: MoveTo(nx,ny);

        Action: The graphics cursor's coordinates take the
                values X, Y.

                See also LineTo, LineRel, MoveRel.


#### `LINEREL`

   Description: Procedure LineRel( DX,DY,Mood:Integer );

         Usage: LineRel(ndx,ndy,nm);

        Action: Draws a line on the screen. The line is drawn
                with a start point determined by the graphics
                cursor, and an end point whose coordinates
                are obtained by adding DX and DY to the start
                point's coordinates.
                The meaning of the Mood parameter is
                explained for the PutPixel procedure.

          Note: Works in graphics mode and screen modes
                0 and 1 (see SetHgr and Screen).

                See also LineTo, MoveTo, MoveRel.


#### `MOVEREL`

   Description: Procedure MoveRel( DX,DY:Integer );

         Usage: MoveRel(ndx,ndy);

        Action: The graphics cursor's new coordinates are
                obtained by adding DX and DY respectively
                to the old values.

                See also LineTo, MoveTo, LineRel.


#### `INVSCR`

   Description: Procedure InvScr;

         Usage: InvScr;

        Action: Inverts the screen.

          Note: Works in graphics mode.
                ( see SetHgr ).





### 3.2 Sprite library (`SPRITE`)


#### `LOADPIC`

   Description: Procedure LoadPic( Var Fail:Bfail;
                                   Var Buf:pic );
         Usage: LoadPic(bf,pb);

        Action: Reads data from a file into a sprite variable.
                A file (with extension .PCC) that was previously
                created and saved as a sprite with the graphics
                editor GTR, and defined with the ASSIGN
                directive in the given program, is read into
                memory. The image size is limited by the amount
                of free memory. If the returned sprite
                variable's element pointing to its location,
                buf.place, has value 0, then there wasn't
                enough memory for that image.


#### `GETPIC`

   Description: Procedure GetPic( X,Y,DX,DY:Integer;
                                  Var Buf:Pic );

         Usage: GetPic(nx,ny,ndx,ndy,pb);

        Action: Reads a sprite from the screen. A rectangular
                area whose top-left corner is at point X,Y
                with side lengths DX and DY is read from the
                screen into the sprite variable.
                The meaning of the Mood parameter is
                explained for the PutPixel procedure.

          Note: Works in graphics mode and screen modes
                0 and 1 (see SetHgr and Screen).


#### `PUTPIC`

   Description: Procedure PutPic( Buf:Pic;
                                  X,Y,Delta,Mood:Integer );

         Usage: PutPic(pb,nx,ny,nd,nm);

        Action: Places a sprite on the screen. The sprite is
                placed on the display so that its top-left
                corner is at the point with coordinates X
                and Y. DELTA gives the offset of the
                background image source from the start of the
                screen (normally DELTA=0).
                The meaning of the Mood parameter is
                explained for the PutPixel procedure.

          Note: Works in graphics mode and screen modes
                0 and 1 (see SetHgr and Screen).


#### `MOVEPIC`

   Description: Procedure MovePic( Var Buf:Pic;
                                   DX,DY,Mood:Integer );

         Usage: MovePic(nb,ndx,ndy,nm);

        Action: Moves a sprite on the screen. A sprite
                previously placed on the display is moved in
                the direction specified by the parameters DX
                and DY.
                The meaning of the Mood parameter is
                explained for the PutPixel procedure.

          Note: Works in graphics mode and screen modes
                0 and 1 (see SetHgr and Screen).


#### `GETMEM`

   Description: Function GetMem( N:Integer ):_Pointer;

         Usage: Var Pnt:_Pointer;
                ...
                Pnt:=GetMem(nx);

        Action: Allocates memory. If N bytes of free memory
                are available, they are reserved and the
                function returns a pointer to that memory
                area. If no free memory is available, the
                pointer value is 0.





### 3.3 Display formatting library (`SCREEN`)



#### `CLRSCR`

   Description: Procedure ClrScr;

         Usage: ClrScr;

        Action: Clears the screen and moves the cursor to
                coordinates 0,0.


#### `CLREOSCR`

   Description: Procedure ClrEoScr;

         Usage: ClrEoScr;

        Action: Clears the screen from the cursor's position
                to the end of the screen.



#### `CLREOLN`

   Description: Procedure ClrEoLn;

         Usage: ClrEoLn;

        Action: Clears the screen from the cursor's position
                to the end of the line.



#### `SCROLON`

   Description: Procedure ScrolOn;

         Usage: ScrolOn;

        Action: Enables display scrolling.



#### `SCROLOFF`

   Description: Procedure ScrolOff;

         Usage: ScrolOff;

        Action: Disables display scrolling.



#### `CURSON`

   Description: Procedure CursOn;

         Usage: CursOn;

        Action: Enables display of the cursor.



#### `CURSOFF`

   Description: Procedure CursOff;

         Usage: CursOff;

        Action: Disables display of the cursor.


#### `GOTOXY`

   Description: Procedure GotoXY( X,Y:Integer );

         Usage: GotoXY(nx,ny);

        Action: Places the cursor at coordinates X,Y.
                The X-coordinate may take values from 0
                to (screen width - 1) and the Y-coordinate
                from 0 to (screen height - 1).


#### `HOME`

   Description: Procedure Home;

         Usage: Home;

        Action: Places the cursor at coordinates 0,0,
                i.e. the top-left corner of the screen.



#### `LEFT`

   Description: Procedure Left;

         Usage: Left;

        Action: Moves the cursor one character to the left.



#### `RIGHT`

   Description: Procedure Right;

         Usage: Right;

        Action: Moves the cursor one character to the right.



#### `UP`

   Description: Procedure Up;

         Usage: Up;

        Action: Moves the cursor one line up.



#### `DOWN`

   Description: Procedure Down;

         Usage: Down;

        Action: Moves the cursor one line down.



#### `WHEREXY`

   Description: Procedure WhereXY( Var X,Y:Integer );

         Usage: WhereXY(mx,my);

        Action: Returns the cursor's coordinates.




#### `INVERSE`

   Description: Procedure Inverse;

         Usage: Inverse;

        Action: Subsequent text is displayed in inverse.



#### `NORMAL`

   Description: Procedure Normal;

         Usage: Normal;

        Action: Subsequent text is displayed normally.


#### `SCREEN`

   Description: Procedure Screen( N:Integer );

         Usage: Screen(nn);

        Action: Selects the text-display mode:
                    N = 0  ->  40x24 characters
                    N = 1  ->  53x24 characters
                    N = 2  ->  64x20 characters



#### `OPENWND`

   Description: Procedure OpenWnd( X1,Y1,X2,Y2:Integer );

         Usage: OpenWnd(nx1,ny1,nx2,ny2);

        Action: Opens a "window". In screen modes 1 and 2,
                X1 and (X2+1) must be divisible by 4.
                ( See Screen )



#### `CLOSEWND`

   Description: Procedure CloseWnd;

         Usage: CloseWnd;

        Action: Closes the "window".



#### `READKEY`




     

     

   Description: Function ReadKey:Integer;

         Usage: Var Code:Integer;
                ...
                Code:=ReadKey;

        Action: Keyboard-read function. If a key on the
                keyboard has been pressed, the function's
                value is the code of the corresponding
                character; otherwise the value is 0.


#### `KBEEPON`

   Description: Procedure KBeepOn;

         Usage: KBeepOn;

        Action: Enables acknowledging key presses with sound.



#### `KBEEPOFF`

   Description: Procedure KBeepOff;

         Usage: KBeepOff;

        Action: Disables acknowledging key presses with sound.




### 3.4  Miscellaneous (`UTILIT`)


#### `RSTTIMER`

   Description: Procedure RstTimer;

         Usage: RstTimer;

        Action: Resets the timer and starts it in stopwatch
                mode.



#### `TIMER`

   Description: Function Timer:Integer;

         Usage: Var Clock:Integer;
                ...
                Clock:=Timer;

        Action: Function for reading the timer's state. The
                function returns the value of the timer
                register started in stopwatch mode (see
                RstTimer), where 1 unit = 20 milliseconds.




#### `MOUSE`

   Description: Procedure Mouse( Var Ud,Rud,Rl,Rrl,
                                     Lsw,Rsw:Boolean );

         Usage: Mouse(lud,lrud,lrl,lrrl,llsw,lrsw);

        Action: Reads "mouse" info. 
                Ud  - last movement in the up–down axis;
                         ( T - down, F - up )
                Rud - current movement in the up–down axis;
                         ( T - moving, F - not moving )
                Rl  - last movement in the horizontal axis;
                         ( T - right, F - left )
                Rrl - current movement in the horizontal axis;
                Rsw - state of the right button;
                Lsw - state of the left button.

          Note: If a "mouse" is not in the computer's
                configuration, calling this procedure causes
                the computer to "hang".



#### `INITPR`

   Description: Function InitPr:Boolean;

         Usage: if Not InitPr then WriteLn('Error!');

        Action: Initialises the parallel port for
                communicating with the printer and checks the
                printer's readiness. If the printer is not
                connected or switched on, the boolean value
                FALSE is returned.



#### `PRCHR`

   Description: Procedure PrChr( Ch:Char );

         Usage: PrChr('a'); PrChr(chr(13)); PrChr(cc);

        Action: The character given by the parameter is sent
                to the printer.

          Note: The function InitPr must be used first.


#### `SOUND`

   Description: Procedure Sound( Freq,Delay:Integer );

         Usage: Sound(nf,nd);

        Action: Starts the audio-frequency generator at the
                frequency given by Freq and for the duration
                in milliseconds given by Delay.



#### `VOLUME`

   Description: Procedure Volume( V:Integer );

         Usage: Volume(nv);

        Action: Sets the volume of the audio signal. If V=0,
                the sound is weak; if V>0, it is strong.




#### `RANDOM`

   Description: Function Random( Range:Integer ):Integer;

         Usage: Var Arv:Integer;
                ...
                Arv:=Random(Random(nr));

        Action: The function returns a number with a value
                from 0 to (Range - 1). The randomness of the
                numbers depends on the Range parameter and on
                the time at which the function is used.




### 3.5  Disk library (`DISK`)


#### `SELECTDISK`

   Description: Procedure SelectDisk( Ds:Char );

         Usage: SelectDisc('B');

        Action: Makes the disk drive indicated by the
                parameter the active one.



#### `SETTRACK`

   Description: Procedure SetTrack( Tr:Integer );

         Usage: SetTrack(ntr);

        Action: Sets the track on the disk that will be
                operated on.



#### `SETSECTOR`

   Description: Procedure SetSector( Sc:Integer );

         Usage: SetSector(nsc);

        Action: Sets the logical sector on the disk that
                will be operated on.



#### `SETDMA`

   Description: Procedure SetDma( M:Integer );

         Usage: Var Buf:Array [ 0..127 ] of Byte;
                ...
                SetDma( Addr(Buf) );

        Action: Sets the address used as the information
                buffer in disk read and save operations. The
                buffer size must be at least 128 bytes.


               
#### `READDISK`

   Description: Procedure ReadDisk;

         Usage: ReadDisk;

        Action: Reads 128 bytes of information from the
                location on the disk set by the SetTrack and
                SetSector procedures, and stores it in memory
                at the location set by the SetDma procedure.



#### `WRITEDISK`

   Description: Procedure WriteDisk;

         Usage: WriteDisk;

        Action: Reads 128 bytes from the location in memory
                set by the SetDma procedure, and stores them
                on the disk at the location set by the
                SetTrack and SetSector procedures.




```
============================================================

  If, while working with this package, you have questions or
                  find errors, please contact:

                    202440 Tartumaa Nõo
                Nõo Keskkooli Arvutuskeskus
                       Indrek Jentson

============================================================
```

### References

[^1]: Интеллектуальный терминал для систем реального времени E5104.
Программное обеспечение. Книга 3.

[^2]: Rein Jürgenson. Programmeerimine Pascalkeeles. Tln. Valgus 1985.

[^3]: Pascal/MT+ Release 5 User's Guide. Third Edition. (c) 1980,1981
by MT MicroSYSTEMS.

