1. `ctrl + \` denotes hiding the left directory tree
2. `alt + ctrl + C` LaTeX clean
3. When you compile a tex file contains eps figures, an 'undefined control sequence' error occurs. Don't worry. Just convert your **eps file into a pdf file** with the command `epstopdf xxx.eps` in a terminal. Then directly use the generated pdf file in your tex file.
4. `ctrl + s` save and compile for a tex file
5. `\usefonttheme[onlymath]{serif}` is the solutin to the warning Class beamer warning: “mathserif” isobsolete. Use font theme “serif” with option “onlymath”. It is supposed to be put in the front part.
