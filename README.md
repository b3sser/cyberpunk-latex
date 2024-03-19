# Cyberpunk RED LaTeX Character Sheet Template
LaTeX template for typesetting Cyberpunk Character Sheets

## Features
- 3-page Character Sheet
- Player input via custom commands for a clean and compact tex file and easy usage
- Automatic text wrap
- Example character to illustrate usage

#### Currently in development:
- automatic calculation of Stat & Base

## Usage
In the ```characters``` folder, you will find an empty sheet, which you may copy and rename for each character you create. There you will also find an example character, illustrating the usage.

Each stat has a custom command, listed and sorted in the empty sheet. The names of the commands should tell you, what Stat goes in there. If there are options, multiple arguments or other things special to one command, they will be explained in a comment right above the command.

As usual with LaTeX, the text you put in the boxes will not be automatically sized, so please work with commands like ```\small``` where necessary.

## Compilation & Dependencies
This Template is designed to be compiled with **XeLaTeX**. XeTeX may also work but is not explicitely tested.

## Credits
This package was created based on the standard Talsorian Games PDF character sheet template and uses it as background image

The basic code structure and some concepts were adapted from matsavages [DnD 5e LaTeX Character Sheet Template](https://github.com/matsavage/DND-5e-LaTeX-Character-Sheet-Template)
