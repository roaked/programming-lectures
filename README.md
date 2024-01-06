# **Building the Foundations to Coding Success**

## Dependencies

Ensure you have a LaTeX distribution installed on your system, such as ```MiKTeX``` or ```TeX Live```

- [TeX Live](https://www.tug.org/texlive/acquire-netinstall.html)
- [MiKTeX](https://miktex.org/howto/download-miktex)

## Setup 

To set up LaTeX in VS Code for compiling LaTeX files into PDFs

1. Install LaTeX Workshop Extension:

- Open VSCode
- Go to the Extensions view (```Ctrl+Shift+X``` or ```Cmd+Shift+X```)
- Search for "LaTeX Workshop" and install it

2. Check LaTeX Distribution

Ensure you have a LaTeX distribution installed on your system. Popular distributions include ```TeX Live``` (recommended for most users) or ```MiKTeX``` (for Windows)

3. Configure LaTeX Workshop

- Open VSCode and go to Settings (```Ctrl+```, or ```Cmd+```,)
- Search for ```"LaTeX Workshop"``` settings
- In the settings, locate the ```"Latex > Tools > Build > Recipes"``` section
- Check the ```latexmk``` recipe and make sure the path to ```latexmk``` is correctly set

4. Set LaTeX Distribution Path

- In the settings, look for ```"Latex > Workshop: Latex > Command"``` setting
- Set the path to your LaTeX distribution's binaries (e.g., ```latexmk```, ```pdflatex```)

5. Environment Variables

- Open a terminal or command prompt and run ```latexmk``` or ```pdflatex``` to ensure these commands are accessible from the command line. 
If not, it might indicate an incomplete LaTeX distribution installation or an issue with the ```PATH environment variable```. Then, it should work

```bash
pdflatex beginner.tex
open beginner.pdf
```