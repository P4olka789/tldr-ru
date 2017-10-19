# latexmk

> Automated LaTeX document generation.

- Compile a LaTeX file into a PDF file:

`latexmk -pdf {{filename.tex}}`

- Force `latexmk` to generate a document even if there are errors:

`latexmk -f {{filename.tex}}`

- Clean up the current directory from all files generated by `latexmk` except DVI, PostScript and PDF:

`latexmk -c`

- Run `latexmk` with minimal terminal output:

`latexmk -silent {{filename.tex}}`