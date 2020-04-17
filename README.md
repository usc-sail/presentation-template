# A presentation template for SAIL based on mtheme (former Metropolis)

This theme has been adapted from the mtheme theme: https://github.com/matze/mtheme. Please visit the link for instructions (including a usage manual).

# License

The license slide ***must be kept in the presentation!***

# Usage
## Overleaf
Use XeLaTeX (`Menu > Compiler > XeLaTeX`). The compiler knows where to find the `.sty` file due to the configuration in the `latexmkrc` file.

For the configuration in the `latexmkrc` to work, `demo.tex` and and `sty/` need to be in the parent folder.

## Your computer
To compile the presentation in your computer using the correct styles, compile the document using the following command:
```bash
TEXINPUTS=".:sty:$TEXINPUTS" xelatex demo.tex
```
This tells XeLaTeX where to find the approrpiate `.sty` file.

You can also use `latexmk` directly:
```bash
latexmk demo.tex
```
(check out all the options: `latexmk --help`).
