![Lute](images/logo.png)

![Version](https://img.shields.io/badge/version-1.0-brown.svg)
![License](https://img.shields.io/badge/license-GPLv3-yellow)
![Size](https://img.shields.io/github/languages/code-size/lartu/lute)

**led**, the *LDPL Text Editor*, is a [line text editor](https://en.wikipedia.org/wiki/Line_editor) 
written in [LDPL](https://github.com/lartu/ldpl), inspired by the ed and sed text editors, but friendlier!

### Watch led in action!
[![asciicast](https://asciinema.org/a/EfF6tiI6DyVKkx6U0KKTUmQuB.svg)](https://asciinema.org/a/EfF6tiI6DyVKkx6U0KKTUmQuB)


## Building led

Clone this repository, `cd` it and run `ldpl led.ldpl -o=led`. Done!

### Releases

You can download pre-compiled binaries of led for amd64 Linux from the
[releases](https://github.com/Lartu/led/releases) section of this repository.

### Usage

Run `led <file>` to open `<file>` and edit it. Alternatively you can just run `led` to create a new, empty file.

led has working two modes, command mode and append mode. When in command mode, all text entered is interpreted as a command.
When in append mode, all text entered is appended to a buffer. To exit append mode, enter a line with just a dot in it
(`.`).

### Commands
 - `h` shows this command list.
 - `l` lists the contents of the buffer.
 - `l <from>` lists the buffer from line `<from>`.
 - `l <from> <count>` lists `<count>` lines from the buffer from line `<from>`.
 - `a` enters append mode.
 - `a <from>` enters append mode and appends text to the buffer at line `<from>`.
 - `d <line>` deletes line `<line>` from the buffer.
 - `d <from> <count>` deletes `<count>` lines from the buffer from line `<from>`.
 - `i` s file information.
 - `q` exits led.
 - `c` clears the screen.
 - `s` saves the buffer to a file.
 - `n` changes the name of the destination file.
 - `r <line>` allows retyping of line `<line>`.

 ### License
 led was created by [Lartu](https://lartu.net) and is released under the GPLv3 license.
