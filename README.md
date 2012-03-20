# My resume in LaTeX

 * Is maybe the basis for yours :)
 * Results in a [beautifully typesetted 2 page pdf file](https://github.com/cies/resume/raw/master/cies-breijs-resume.pdf)
 * Compiles (with nice fonts and all) without much trouble on a recent version of Ubuntu

I've looked at most, if not all, of the [LaTeX](http://en.wikipedia.org/wiki/LaTeX) resumes and templates I could find on the internet, but none of them I really liked.  I picked [the best I could find](http://www.toofishes.net/blog/tags/latex) and adapted it to fit my ideas about graphic design and typography.

Go ahead and fork it.. `:)`  I dont really feel like making it into 'library'.

As I love typesetting, I naturally did my best. It uses the TeX Gyre Pagella font
that is often used for books (with 'low case numbers' -- as I love those).

Except the horizonal lines and some bullets everything is made of text.  It uses hyper-refs where applicable, all in dark blue so 'print safe'.

Everything it relies on is open source and is readily available in recent versions of Ubuntu.



# Installing and compiling on ubuntu

To generate a `pdf` in recent Ubuntu versions do:

        sudo apt-get install texlive-xetex tex-gyre texlive-latex-recommended
        xelatex cies-breijs-resume

I don't use `pdflatex` but `XeTeX` since it allows me to use Pagella's lowercase numbers.



# ToDo

  * (none at the moment)


# TaDa

  * Separate file for command definitions (so we can collaborate on that file using forks and pull-requests)
  * Allow ligatures (not very noticable with the Pagella font, one could try Libertine or Hoefler)
  * Use old style numbers (had to make the apostrophes look nice on double-digit years)
  * Cleanup the tex file: some repetitive stuff can move into functions



# Terms of sharing

Feel free to use, copy, fork, share, study and/or modify it because the LaTeX source code of the `resume-commands.tex` file is [GPLv3](http://www.gnu.org/licenses/quick-guide-gplv3.html) licensed.

The text of my resume in the `cies-breijs-resume.tex` file is [CC-NC-ND](http://creativecommons.org/licenses/by-nc-nd/3.0/) licensed.
