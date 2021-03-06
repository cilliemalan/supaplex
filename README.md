# Supaplex
[Supaplex](https://en.wikipedia.org/wiki/Supaplex) is a game made in the early nineties.

![image](https://user-images.githubusercontent.com/3305301/42215866-25134eb4-7ec0-11e8-913d-b64604632fa8.png)

Since then the source code has been lost. Some enthusiasts have disassembled the game,
fixed many bugs, and added many features. Today the game and the so-called speed fix can
be downloaded free from [here](http://www.elmerproductions.com/sp/dlinst.html). 

The source code for the speed fix is likewise, unavailable.

# What this is
This project  is an effort to disassemble and understand the speed fix
code once again.

Here you'll find assembly files, and an IDA database that contains the dissasembled and
analyzed source of the SPFIX63.EXE file.

## Getting Started
### Prerequisites
- You need [DosBox](https://www.dosbox.com/) to build and run.
- You will need the [original Supaplex files](https://cdn.chills.co.za/supaplex.zip).
    Extract the files into the `build` directory.
- You will need [TASM 4.1](https://cdn.chills.co.za/tasm4.zip).
    Extract the files into the `tasm` directory. Feel free to put them in your path
    (in dosbox)

### Building
Open DOSBox and mount this directory. To do this, start DOSBox and type this:
```
mount C <wherever this is>
C:
```

To build, run `TASM\MAKE`:
```
C:\>TASK\MAKE
MAKE Version 4.0  Copyright (c) 1987, 1996 Borland International
        TASM\TASMX /m2 SUPAPLEX.ASM BUILD\SUPAPLEX.OBJ BUILD\SUPAPLEX.LST
Turbo Assembler  Version 4.1  Copyright (c) 1988, 1996 Borland International

Assembling file:   SUPAPLEX.ASM  to  BUILD\SUPAPLEX.OBJ


...

```
Note: if the build is too slow, press F12 repeatedly or change your DOSBox config to use
more CPU.

### Running
Run `build\supaplex.exe` after building.

### Testing
For tests you have to [download some solves](https://cdn.chills.co.za/solve.zip) and
extract to the `solve` directory. Then
Run `TEST.BAT` to run some tests. output will be put in `TESTOUT.TXT`.


# License
I could not find any license with the original executable prohibiting
disassembly and modification of the source code. As such I release the
disassembled source code of the game under the MIT license. If you have
a problem with this please don't hesitate to contact me.
