## 0. content

1. how to install
  1. on windows
  2. on linux
  3. on mac
2. Error solving
3. Reporting issues

## 1. How to Install?

### 1.1 Windows

**Make sure you have [python 3.3 or newer](https://www.python.org/) ([Download Page](https://www.python.org/downloads/)) and [PyQT4](http://www.riverbankcomputing.com/software/pyqt/intro) ([Download Page](http://www.riverbankcomputing.com/software/pyqt/download)) installed**

1. grab the zip file, unzip everything in it to a folder
2. run OBS_Stream_Topbar-x.y.z.exe
3. Success! not? > read chapter 2: _"Error Solving"_

### 1.2 Linux

**make sure to install [wine](https://www.winehq.org/) ([Download Page](https://www.winehq.org/download/)). _DO NOT RUN WITH MONO!_**

1. install Python3 and PyQT4 in wine
2. Follow the steps for windows, but use _wine_ instead of just running the executable

### 1.3 Mac

**I DO NOT OWN A MAC, I DON'T OFFICIALLY SUPPORT IT; I DO _NOT_ KNOW IF THIS WORKS**

1. Install [WineBottler](http://winebottler.kronenberg.org/) ([Download Page](http://winebottler.kronenberg.org/downloads))
2. install Python3 and PyQT4 in winebottler
3. follow the steps for windows, but use _winebottler_ instead of running the executable

(Who streams (and games) on a mac anyways)

## 2. Error Solving

#### Error: listen EACCESS _(general)_
what is this?
> Eaccess is thrown when the port you are trying to bind to is already in use

how to solve:
> Try using a different port in settings.js

#### Error: listen EACCESS, Permission denied
what is this?
> Eaccess permission denied is thrown when you are trying to use a port under 1024 on linux (and maybe mac), it means that you don't have the right permissions to use the port

how to solve:
> there are 2 options:
1. use a port higher than 1024 OR
2. run with sudo/root permissions **(please use solution 1 as running with root _can_ be very dangerous: [Murphy's law](http://en.wikipedia.org/wiki/Murphy%27s_law) )**

#### Error: spawn ENOENT
what is this?
> spawn ENOENT is probably caused because the python process couldn't start

how to solve:
> **Make sure you are using the right wine/winebottler instance if on linux/mac**

>try reinstalling python3 and PyQT4.

#### Cannot open assembly 'OBS_Stream_Topbar-x.y.z.exe': File does not contain a valic CIL image
what is this?
> Mono trying to find an assembly which does not exist

how to solve:
> USE _WINE_ ([Download Page](https://www.winehq.org/download/)); NOT MONO, **MONO is for C#/C#.NET**, not for other languages!

#### if these answers don't solve your issue, read chapter 3: Reporting Issues

## 3. Reporting Issues

if you can't figure it out, please use ~~the [issue tracker @ github.com](https://github.com/jojoxd/stream-topbar-issues/issues)~~ the issue tracker on your right side.
