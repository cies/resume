# a resume in LaTeX

 * is maybe a template for yours :)
 * view the resulting [pdf file](https://github.com/cies/resume/raw/master/cies-breijs-resume.pdf)
 * shows you how to make it compile on a recent ubuntu

i've looked at most -- if not all -- of the [LaTeX](http://en.wikipedia.org/wiki/LaTeX) resumes and templates, but not quite liked them. i picked [the best i could find](http://www.toofishes.net/blog/tags/latex) and adapted it to my taste.

go ahead and fork it.. :)  i dont really feel like making it into
'library'.

i like typesetting, so naturally did my best. it uses the pagella font
that is often used for books (with 'low case numbers' -- i love those).

except the h-lines and some bullets everything is made of text. uses
hyper-refs where applicable, in dark blue so 'print safe'.

everything it relies on is open source.



# installing and compiling on ubuntu

to generate a pdf from this file in ubuntu:

        sudo apt-get install texlive-xetex tex-gyre texlive-latex-recommended
        xelatex cies-breijs-resume.tex

i don't use `pdflatex` but `XeTeX` since it allows me to use gyre pagella's lowercase numbers.



# todo

  * separate file for command definitions (can collaborate on that
    file with forks)


# tada

  * ligatures (not very noticable with the gyre/pagella font, one couldtry libertine or hoefler)
  * old style numbers (had to make the apostrophes look nice on double-digit years)
  * cleanup the tex file: some repetitive stuff can move into functions



# terms of sharing

feel free to copy (fork!) it, because this is `Creative Common Attribution Share-Alike 3.0` licensed.
