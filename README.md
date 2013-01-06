# Introduction

Plouf! is an old Amiga game I wrote a long time ago.

It is a top-down 2-or-3-players game which features people sitting on floats,
trying to sink the other players by throwing sea urchins at them.

You control your float like an RC car: you can accelerate, slow down and rotate
left or right.

You start with a very limited number of sea urchins, so you need to collect them
as they appear randomly in the sea. You can also grab float bonuses which
increase the strength of your float by one point.

# Running Plouf!

## Hardware

To run Plouf! You need either an Amiga 500 or an emulator. On Linux it runs fine
with E-UAE or FS-UAE. I expect it to work without problems on other platforms
where a version of UAE is available.

## Controls

By default player 1 uses the joystick, other players use the keyboard. This can
be changed in the `Options` menu.

Controls per players are:

- Player 1: Joystick 1 (default) - or - 5, 2, 1, 3, Numpad Return
- Player 2: Joystick 2 - or - E, D, O, P, Space (default)
- Player 3: Arrow keys, Return

While it is possible to play a 3-player game solely on the Amiga keyboard, using
joysticks is highly recommended.

# Licensing

Plouf! was originally released as shareware, but license has been changed to
GPLv3 or later.

# History

Plouf! was created using AMOS, a game-oriented Basic language. It was released
as a shareware in 1994: a floppy disk of the demo version (limited to 4 plays)
could be ordered from a few Amiga freeware and shareware floppy disk dealers.

To my knowledge, it was never made available on the Internet. The floppy disks
containing the source code stayed for 18 years together with my Amiga in a
storage room.

Some time ago I decided to release it as free software. I bought a NULL-modem
cable and transfered the source code to my laptop. I then adjusted a few things,
got rid of the demo limitations, translated all visible strings to English and
released it.

# About the source code

The source code for the game is in the `plouf.AMOS` file. A `.AMOS` file is a
binary format, bundling together the source code and the program assets. You
need the AMOS Editor to read it.

There was also an asset editor named "Plouf! Config". This editor was available
with the full version. Its source code is in `plouf config.AMOS`.

Note that while all visible strings have been translated to English, I did not
go through the trouble of translating the source code: all comments, variables
and procedure names are still in French.

## Compiling a new version of Plouf!

(This section is more like a personal note in case I decide to work on Plouf!
again.)

Make sure AMOS Compiler has been installed on AMOS main disk.

- Start AMOS
- Open Compiler.AMOS
- Click the target button until it reads "Cli"
- Click the "Compile" button
- As source code: use `Plouf.AMOS`
- As destination: enter `Plouf!`
