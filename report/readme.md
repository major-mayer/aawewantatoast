# Readme Latex Report

## Required build tools
###  Arch Linux packages
- texlive-core          # Contains base latex packages like the lualatex compiler
- texlive-latexextra    # Contains a huge amount of extra latex packages
- texlive-bibtexextra   # Latex packages to support reference management with biblatex
- biber                 # Biblatex backend
- perl-file-homedir     # idk
- perl-yaml-tiny        # idk
- hunspell-en_gb        # English hunspell dictionaries for spell checking

### Windows
Maybe have a look at the texlive latex distribution: https://www.tug.org/texlive/acquire-netinstall.html  
Additional packages can be downloaded from here: https://ctan.org/

### Using Docker and VSCode's Remote Containers functionality 
I never tried this, but it could be easier than installing the packages manually  
https://github.com/James-Yu/LaTeX-Workshop/wiki/Install#using-docker

## Required VSCode Extensions
- Latex Workshop
- Optional: Spellright for spell checking

## Build project
- Open anx `*.tex` file in the editor
- Press `F1`
- Select "LaTeX Workshop: Build LaTeX Project"


Or
- Use the Menu bar on the left and build the document there

Then 
- The LaTeX Compiler Output should contain a lot of stuff including warnings and hopefully not errors
- When it ends with something like this: 
``` 
Output written on main.pdf (19 pages, 5968089 bytes).
SyncTeX written on main.synctex.gz.
Transcript written on main.log.
``` 
- It means that the compilation was successful and you can find the generated PDF file [here](report/output/main.pdf)
- You have a few choices how to open the generated PDF
    - Open it with any PDF viewer of your choice 
    - Use the LaTeX Workshop tab from the VSCode sidebar, go to "View LaTeX PDF", then "View in VSCode tab"
        - this will open the PDF in an integrated window