# Cyberpunk RED LaTeX Character Sheet Template
LaTeX template for typesetting Cyberpunk Character Sheets

## Features
- 3-page Character Sheet
- Player input via custom commands for a clean and compact tex file and easy usage
- Automatic text wrap
- Example character to illustrate usage

#### Currently in development:
- Automatic calculation of Stat & Base (for Skills) and more auto-calculated values
- Mooks Sheets

## Usage
#### TL;DR
1. Copy ```empty.tex```
2. Fill commands with your values and text
3. Compile with XeTeX

Look at ```example-character.tex``` for guidance

#### More Tips
- Each stat has a custom command, listed and sorted in the empty sheet. The names of the commands should tell you, what Stat goes in there. If there are options, multiple arguments or other things special to one command, they will be explained in a comment right above the command.

- Multiline-fields have automatic line-wrap, for others use ```\\``` where needed
- All fields have a default font size. You can change for selected fields by adding a size command before your actual input.
    - Sizes: ```\Huge```, ```\huge```, ```\LARGE```, ```\Large```, ```\large```, ```\normalsize```, ```\small```, ```\footnotsize```, ```\scriptsize```, ```\tiny```

<!--
#### Auto-calculation of stats
If you want auto-calculation, make sure to leave the fields supporting this feature blank.

When working with auto-calculation, you can overwrite selected values with your own input (e.g. when an item you have changes that value), simply by using the command like you would in a sheet without auto-calculation. The calculated value is only set as the default and can be overwritten this way.
-->

## Compilation & Dependencies
This Template is designed to be compiled with **XeLaTeX**. XeTeX may also work but is not explicitely tested.

If you are encountering issues, please make sure you have ```xetex-pstricks``` installed.

## Credits
This package was created based on the standard Talsorian Games PDF character sheet template and uses it as background image

The basic code structure and some concepts were adapted from matsavages [DnD 5e LaTeX Character Sheet Template](https://github.com/matsavage/DND-5e-LaTeX-Character-Sheet-Template)
