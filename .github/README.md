
# `reptheorem`

When writing a large manuscript, it is sometimes beneficial to repeat a theorem (or lemma or…) at an earlier or later point for didactical purposes. However, `thmtools`'s built-in `restatable` only allows replicating theorems *after* they have been stated, and only in the same document. `reptheorem` solves the issue by making use of the `.aux` file, and also introduces its own file extension, `.thm`, to replicate theorems in other files.
## Installation

Run the following in the command line:
1. If reptheorem.ins is present: `latex reptheorem.ins`
2. If reptheorem.ins is absent: `latex reptheorem.dtx`

Move `reptheorem.sty` to a folder that TeX can find.

## Documentation

Run the following in the command line:
```
pdflatex reptheorem.dtx
makeindex -s gind.ist -o reptheorem.ind reptheorem.idx
makeindex -s gglo.ist -o reptheorem.gls reptheorem.glo
pdflatex reptheorem.dtx
```
This automatically unpacks the package, as well.

Alternatively, the documentation can be found on the [CTAN page](https://ctan.org/tex-archive/macros/latex/contrib/reptheorem).

---

&copy; 2024- Jesse Straat

License: [LPPL1.3c](https://www.latex-project.org/lppl.txt)

[CTAN page](https://ctan.org/tex-archive/macros/latex/contrib/reptheorem)
