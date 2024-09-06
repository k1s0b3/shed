# Shed - A simple ed-like text editor implemented in Bash

## ToC

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Commands](#commands)
  - [Tips](#tips)
- [Inspiration](#inspiration)


## Features

- Easy to use as a line editor

## Prerequisites

- `bash`

- `awk`
- `less`
- `sed`
- `xclip`

You can easily modify the code if you don't need them.

## Getting Started

### Installation

```bash
git clone https://github.com/k1s0b3/shed
cd shed
chmod +x shed
./shed
```

### Commands

```bash
shed v0.0.1 - type ~ for commands, otherwise just start typing
~help
~ represents your prefix, if you changed the prefix use that instead
key: ~command arg1/alt_arg1 arg2 [optional_arg] - what the command does
~about - display about text
~clear - clear buffer
~copy [line] - copy line or whole buffer to clipboard
~correct - replace most recent line (interactive)
~delete line/start [end] - immediately delete specified line or range of lines
~exit - exit shed
~help - display this list
~indent line level - indent a line, negative level will un-indent
~insert line - insert text at specified line (interactive)
~open [filename] - load file into buffer
~prefix [prefix]
~prompt [prompt] - set an input prompt
~replace line - replace specified line (interactive)
~run command - run executable or shell builtin
~runhere command - run executable or shell builtin on buffer contents
~save [filename] - save buffer to file
~search term - perform regex search in whole buffer
~show [start] [end] - Display the contents of the buffer.
~showhere [start] [end] - Display the contents of the buffer inline.
~substitute line pattern/replacement - perform regex substitution on specified line
~swap source target - swap two lines
```

### Tips

Piping of buffer works well like this if you have softwares like `bat` and `glow`.

```bash
~runhere bat # show current buffer with `bat`
~runhere glow -l # show current buffer (markdown) with `glow`
```

## Inspiration

`shed` is heavily inspired by [`sued`](https://github.com/AeriaVelocity/sued).
It works well and has more features than `shed`.

