# Modifications
Added a 'Start Step' button that will start the tournament in a paused state, will also create a 'step' button to allow the user to step through each cycle. I've done this to make it slightly easier to debug.

# r2wars

C# implementation for r2wars tournament

Tournament api from: https://github.com/otac0n/tournaments

## Description

r2wars is a game similar to corewars, where 2 programs run on a
shared memory space trying to catch each other in order to trash
their code and make them crash.

This game was initially developed by pancake as a PoC in here

* https://github.com/radare/radare2-extras/tree/master/r2wars

You can find an explanation of the game in the first competition
that happened during the 2nd r2con in 2017.

* https://www.youtube.com/watch?v=sB-i5yUatx4

This repository contains an evolved implementation of the engine
written in C# by SkUaTeR dropping the MFC requirement that was
making it impossible to run outside Windows.

The solution was to use an embedded webserver that provides a
web interface using websockets to stream the process changes
from the M

## Dependencies

* Mono / .NET Runtime
* radare2

On windows you need to have radare2.exe and rasm2.exe in the same
directory as the r2wars.exe executable.

On Mac/Linux/BSD, r2wars will try to find them in the PATH.

--pancake
