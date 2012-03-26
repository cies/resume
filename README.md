# My resume in LaTeX

 * Is a [nicely typesetted 2 page pdf file](https://github.com/cies/resume/blob/master/cies-breijs-resume.pdf?raw=true) (click the link to download mine)
 * Compiles with or without installing software (read more below)
 * Might well be a starting point for your very own Latex resume...

Linkedin serves well, but not in all situations.  At some point my profile
just cluttered up, while all I wanted 'them' to have is a good looking
two page resume.  Naturally turned to Latex.

Looking at some Latex resumes online I found non that I really liked, so
I gave it my best shot.  I made it into a well documented project as I
expect more geeks want their resume to be typeset like this.  I don't really
feel like making it into 'library', unless someone can convince me of the
benefits; in the meantime just "fork it on GitHub".

It uses TeX Gyre Pagella, a font similar to Pallatino that is often used for
books.  When compiled with `XeLateX` it has 'lower case numerals', which I
think look very nice.

Except the horizonal lines and bullets everything is made of text.
Hyper-refs are used where applicable, all in dark blue so 'print safe'.

Obviously it only relies on open source stuff.



## Generating the PDF

There are several ways to generate a PDF from the Latex sources.  I
describe only 2 of them here...


#### Using ScribTex (no need to install any software)

[ScribTex](http://www.scribtex.com) is a web application for creating
and collaborating on Latex documents.  They have a free account that
requires no login and can be used to compile this resume.

To get this resume compiled with ScribTex:

  1. Copy the source of the [combined resume file](https://github.com/cies/resume/blob/master/combined/cies-breijs-resume.tex)
  2. Go to [ScribTex.com](http://www.scribtex.com) and click the "Try it now" button to immediately start a free but *not saved* project.
  3. In your new project click the `main.tex` file and replace the content with what you copied in step 1.
  4. Hit the "Compile" button to see the resulting PDF.

The build script `build.sh` automatically combines the
`resume-commands.tex` with any `*-resume.tex` files and puts them in the
`combined/` folder.  So if you decide to fork this project, then running
`./build.sh` is necessary to in case you want to follow these steps.


#### Using XeLaTeX

XeLaTeX is a version of Latex with great font rendering fuctionality (unicode, bidi,
special font features).  Since my resume uses 'lower case numerals' it
looks slightly better with XeLaTeX.

In recent Ubuntu versions you simply clone this project, change
directory to the root of the project and do:

        sudo apt-get install texlive-xetex tex-gyre texlive-latex-recommended
        ./build.sh

If all went well an updated version of the PDF is found in your current
working directory.


## ToDo

  * (none at the moment)


## TaDa

  * Works out of the box with ScribTex
  * Separate file for command definitions (so we can collaborate on that file using forks and pull-requests)
  * Allow ligatures (not very noticable with the Pagella font, one could try Libertine or Hoefler)
  * Use old style numbers (had to make the apostrophes look nice on double-digit years)
  * Cleanup the tex file: some repetitive stuff can move into functions
  * Clever page breaking


## Terms of sharing

Feel free to use, copy, fork, share, study and/or modify it because the LaTeX source code of the `resume-commands.tex` file is [MIT](http://en.wikipedia.org/wiki/MIT_License) licensed.

The text of my resume in the `cies-breijs-resume.tex` file is [CC-NC-ND](http://creativecommons.org/licenses/by-nc-nd/3.0/) licensed.



