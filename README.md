# **Building the Foundations to Coding Success**

## **Dependencies**

Ensure you have a LaTeX distribution installed on your system, such as ```MiKTeX``` or ```TeX Live```

- [TeX Live](https://www.tug.org/texlive/acquire-netinstall.html)
- [MiKTeX](https://miktex.org/howto/download-miktex)

## **Setup**

To set up LaTeX in VSCode for compiling LaTeX files into PDFs

### 1. Install LaTeX Workshop Extension:

- Open VSCode
- Go to the Extensions view by clicking on the Extensions icon in the Activity Bar (or press `Ctrl+Shift+X` or `Cmd+Shift+X`)
- Search for "LaTeX Workshop" in the Extensions Marketplace and install it

### 2. Check LaTeX Distribution

Ensure you have a LaTeX distribution installed on your system. Popular distributions include ```TeX Live``` (recommended for most users) or ```MiKTeX``` (for Windows)

### 3. Configure LaTeX Workshop in VSCode
- Open one of the LaTeX documents (e.g., `beginner.tex`) 
- Set the LaTeX Workshop as the default builder:
   - Open the VSCode Command Palette (`Ctrl+Shift+P` or `Cmd+Shift+P`)
   - Type "LaTeX Workshop: Build LaTeX project" and select it. This sets LaTeX Workshop as the default builder for LaTeX files

### 4. Customize Build Settings **(Optional)**
- You can configure LaTeX Workshop settings based on your preferences:
   - Go to VSCode Settings (`Ctrl+,` or `Cmd+,`)
   - Search for "LaTeX Workshop" settings
   - Adjust settings like LaTeX distribution, build commands, PDF viewer, etc...

### 5. Compile LaTeX to PDF
- With LaTeX Workshop installed and configured, you can now compile your LaTeX files to PDF:
   - Open a `.tex` file
   - Press `Ctrl+Alt+B` or `Cmd+Alt+B` to compile the LaTeX document
   - View the output in the LaTeX Workshop panel at the bottom of the VSCode window


## **Troubleshooting --- LaTeX in Compiling // + Git Bash**

### 1. Check LaTeX Distribution Installation

- Ensure your LaTeX distribution (e.g., [MiKTeX](https://miktex.org/howto/download-miktex) or [TeX Live](https://www.tug.org/texlive/acquire-netinstall.html)) is correctly installed and its binaries are added to the system PATH
- Test by running `pdflatex` or `latexmk` commands in Git Bash to verify if the LaTeX distribution is accessible

### 2. Verify Environment Variables
- Check if the PATH environment variable includes the path to your LaTeX distribution's binaries.
- Open Git Bash and type `echo $PATH` to view the PATH environment variable. Verify if the LaTeX binaries directory is included

### 3. PATH Configuration:
- If the LaTeX distribution's binaries are not in the PATH
  - Locate the directory containing `pdflatex` or `latexmk` (e.g., `C:\texlive\2021\bin\win32` for TeX Live)
  - Add the LaTeX distribution's bin directory to the PATH
    ```bash
    export PATH="/path/to/latex/bin:$PATH"
    ```
    Replace `/path/to/latex/bin` with the actual path to the LaTeX binaries
  - Test LaTeX commands again in Git Bash

### 4. File Permissions
- Ensure that you have appropriate permissions to access and modify files in the LaTeX project directory
- Use `ls -l` command in Git Bash to check file permissions

