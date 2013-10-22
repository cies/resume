# My Latex resume

 * Is a [nicely typeset 2-page PDF](https://rawgithub.com/cies/resume/master/cies-breijs-resume.pdf) (click the link to download mine)
 * Compiles with or without installing software (read more below).
 * Might well be a starting point for your very own Latex resume.

Linkedin serves well, but not in all situations.  At some point my profile
just cluttered up, while all I wanted 'them' to have is a good looking
two page resume.  Naturally turned to Latex.

Looking at some Latex resumes online I found non that I really liked, so
I gave it my best shot.  The I documented my effort here on Github as I
expect more geeks want their resume to be typeset like this.

It uses TeX Gyre Pagella, a font similar to Pallatino that is often used for
books.  When compiled with XeLaTeX it has 'lower case numerals', which I
think look very nice.

Except the horizonal lines and bullets everything is made of text.
Hyper-refs are used where applicable, all in dark blue so 'print safe'.

A 'last updated at' date is printed on the top-right of the page.

Obviously it only relies on open source stuff.



## Generating the PDF

There are several ways to generate a PDF from the Latex sources.


#### Using ShareLatex (no need to install any software)

[ShareLatex](http://www.sharelatex.com) is a web application for creating
and collaborating on LaTeX documents.  They have a free account that
can be used to compile this resume.

To get this resume compiled into a PDF with ShareLatex:

  1. Go to [sharelatex.com](http://www.sharelatex.com) and create first an account and then a project.
  2. In your new project replace the content of the `main.tex` file with the LaTeX source of resume's content (`cies-breijs-resume.tex` in this case) from Github.
  3. In your new project create a new file `resume.sty` and copy-paste
     the content of the same named file from the Github repo.
  4. Finally hit the "Compile" button to view and/or download the resulting PDF.

The result will be nice, but IMO will be nicer if you change the
rendering engine to XeLaTeX -- you can do so from the projects 'Setting' form
which hides behind the gear-icon on the left.

*TIP:* In the 'User Settings' (under 'Account' menu in the top-right) form you can set the spell-check language.


#### Using XeLaTeX

XeLaTeX is a version of Latex with great font rendering fuctionality (unicode, bidi,
special font features).  Since my resume uses 'lower case numerals' it
looks slightly better with XeLaTeX.

In recent Ubuntu versions you simply clone this project, change
directory to the root of the project and do:

        sudo apt-get install texlive-xetex texlive-latex-recommended tex-gyre
        ./xelatex *-resume.pdf

If all went well an updated version of the PDF is found in your current
working directory, alongside a bunch of `.log` and `.aux` files that
you can safely ignore.


### Using pdfLatex

Follow the same steps as for XeLaTeX, just replace the `./xelatex`
command with `./pdflatex`.



## TODO

  * See if LuaTex can give access to both `fontspec`, `microtype` and unicode (so it can replace Xelatex)
  * Make the vertical spacing configurable in one setting.


## TADA

  * Now uses [rawgithub.com](http://rawgithub.com) for in-browser viewing.
  * [ShareLatex](http://sharelatex.com) is awesome! Point it out to users.
  * When using `pdflatex` the `microtype` package kicks in
  * Made switching to the [Linux Libertine](http://www.linuxlibertine.org) font easier
  * Fixed all outstanding spacing issues (thanks to the `\sloppy` command)
  * Works out of the box with ScribTex
  * Separate file for command definitions (so we can collaborate on that file using forks and pull-requests)
  * Allow ligatures (not very noticable with the Pagella font, one could try Libertine or Hoefler)
  * Use old style numbers (had to make the apostrophes look nice on double-digit years)
  * Cleanup the tex file: some repetitive stuff can move into functions
  * Clever page breaking


## Terms of sharing

Feel free to use, copy, fork, share, study and/or modify it because the LaTeX source code of the `resume.sty` file is [MIT](http://en.wikipedia.org/wiki/MIT_License) licensed.

The text of my resume in the `cies-breijs-resume.tex` file is [CC-NC-ND](http://creativecommons.org/licenses/by-nc-nd/3.0/) licensed.


