# Cyberpunk RED LaTeX Character Sheet Template
LaTeX template for typesetting Cyberpunk Character Sheets

## Features
- 3-page Character Sheet
- Automatic calculation of Stat & Base (for Skills) and for Derived Stats (e.g. Death Save)
- Player input via custom commands for a clean and compact tex file
- Example character to illustrate usage

#### Currently in development:
- Background as svg or via tikz to make resulting pdfs much more lightweight and load faster
- Mooks Sheets

## Usage
#### TL;DR
1. Copy ```empty.tex```
2. Fill commands with your values and text
3. Compile with XeLaTeX

Look at ```example-character.tex``` for guidance

#### Auto-calculation of stats
If you want auto-calculation, make sure to leave the fields supporting this feature blank or remove their commands entirely.

When working with auto-calculation, you can overwrite selected values with your own input (e.g. when an item you have changes that value), simply by using the command like you would in a sheet without auto-calculation. The calculated value is only set as the default and can be overwritten this way.

#### More Tips
- Each stat has a custom command, listed and sorted in the empty sheet. The names of the commands should tell you, what Stat goes in there. If there are options, multiple arguments or other things special to a command, they will be explained in a comment right above it.
- For most fields, if you want to leave a command blank for auto-calculation or because that field should stay blank, you can just delete the command for a cleaner tex-file and everything should still work as expected.

- Multiline-fields have automatic line-wrap, for others use ```\\``` where needed
- All fields have a default font size to fit with a normal amount of input. You can change the size for selected fields by adding a size command before your actual input.
    - Sizes: ```\Huge```, ```\huge```, ```\LARGE```, ```\Large```, ```\large```, ```\normalsize```, ```\small```, ```\footnotsize```, ```\scriptsize```, ```\tiny```

## Compilation & Dependencies
This Template is designed to be compiled with **XeLaTeX**. XeTeX may also work but is not explicitely tested.

*Personally, I opened the folder in VSCodium with LaTeX Workshop Extension and ran ```Recipe: latexmk (xelatex)```*

If you are encountering issues, please make sure you have ```xetex-pstricks``` installed.

## Credits
This package was created based on the standard Talsorian Games PDF character sheet template and uses it as background image

The basic code structure and several concepts were adapted from matsavages great [DnD 5e LaTeX Character Sheet Template](https://github.com/matsavage/DND-5e-LaTeX-Character-Sheet-Template), with his explicit permission.

## Feedback & Bugs
I appreciate any feedback and bug reports on this project.
Please open an issue on github, describing the bug and adding code snippets, screenshots (if needed) and information about your compiler
