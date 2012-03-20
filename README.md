# My resume in LaTeX

 * Results in a [beautifully typesetted 2 page pdf file](https://github.com/cies/resume/raw/master/cies-breijs-resume.pdf) (click the link to download mine)
 * Compiles with simple apt-get instruction (below) on a recent version of Ubuntu or other distro with `tex-live` packages
 * Is maybe the basis for yours! (fork-it)


I dont really feel like making it into 'library', unless someone can
convince me of the benefits.

It uses TeX Gyre Pagella, a font similar to Pallatino that is often used for books, and uses 'low case numbers'.

Except the horizonal lines and bullets everything is made of text.  It uses hyper-refs where applicable, all in dark blue so 'print safe'.

It only relies on is open source and is readily available in recent versions of Ubuntu.



# Installing and compiling on ubuntu

To generate a `pdf` in recent Ubuntu versions do:

        sudo apt-get install texlive-xetex tex-gyre texlive-latex-recommended
        xelatex cies-breijs-resume

I don't use `pdflatex` but `XeTeX` since it allows me to easily use Pagella's lowercase numbers.



# ToDo

  * (none at the moment)


# TaDa

  * Separate file for command definitions (so we can collaborate on that file using forks and pull-requests)
  * Allow ligatures (not very noticable with the Pagella font, one could try Libertine or Hoefler)
  * Use old style numbers (had to make the apostrophes look nice on double-digit years)
  * Cleanup the tex file: some repetitive stuff can move into functions
  * Clever page breaking


# Terms of sharing

Feel free to use, copy, fork, share, study and/or modify it because the LaTeX source code of the `resume-commands.tex` file is [GPLv3](http://www.gnu.org/licenses/quick-guide-gplv3.html) licensed.

The text of my resume in the `cies-breijs-resume.tex` file is [CC-NC-ND](http://creativecommons.org/licenses/by-nc-nd/3.0/) licensed.
