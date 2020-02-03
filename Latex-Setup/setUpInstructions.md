#Contributing 

This Repo is a common store for creating and archiving LaTeX documents.

##Prerequisites

- Access to GitHub Papers Repository
- LaTeX setup on your local machine
- SSH terminal software
- Git client installed 

##Using Git                   

This repo is hosted from Github. Git will be used for cloning the repo, creating branches, updating changes to your branch and making pull requests. We use [Git-Flow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) approach to version control.

-  Cloning the repo:  `git clone https://github.com/aescalona-doitt/papers`
-  Creating a branch:  New branches can be created from Github's site. New branches should be created from the `develop/<document-type>/<your-new-branch>` branch. Document type is one of the document class (e-g., Articles, Books, and Papers etc.). New branches should follow the naming rules as follows:


-  Committing and pushing updates: Commits and pushes to your branch can be done from your IDE or command line. Please provide meaningful commit messages to your commits.
-  Merging your branch into `develop`:  Do not commit or push into the `develop` branch. When your branch is ready for merging into `develop`, create a pull request in GitHub.

##Naming convention for base LaTeX file
The same naming convention used for naming your document repository applies to the root LaTeX file as well:


##Getting Started with LaTeX

You need two things to start producing documents using LaTeX: A text editor to write the documents, and a compiler to produce the LaTeX generated output. We give detailed instructions for getting started with LaTeX on Mac and Linux (ubuntu).

###Windows

####Download and install TeXworks
1. Go to http://www.tug.org/texworks/
2. Download TeXworks for WIndows
3. Go to https://miktex.org/, Download tab
4 Windows tab, click download and install

###Mac

####Download and install MacTeX

1. Go to http://www.tug.org/mactex
2. Download the MacTeX (~1GB)
3. Unzip and install
4. Setup path to LaTeX executables by running the following command in terminal. To make the changes permenant, you might add the line to ~/.bash_profile and run 'source .bash_profile' in terminal. 

        export PATH=$PATH:/Library/TeX/texbin

####Create HelloWorld Document

Now, we are ready to create a simple helloworld document using MacTex.

####Using Terminal
1. Create: In your feature branch execute the following command:

		vi helloworld.tex
  
2. Write: In the window, type this:

        \documentclass{article}
        \begin{document}
        Hello World!
        \end{document}

3. Save: press ESC key, the type ':wq' and hit ENTER.
4. Compile: Execute the following command to generate pdf file:

		pdflatex helloworld.tex

5. View: Execute the following command to view the generated pdf file: 

		open helloworld.pdf

####Using IDE

1. Open: TexShop (search TexShop in Finder). This will open a blank document.  
2. Write: In the window, type this:

        \documentclass{article}
        \begin{document}
        Hello World! 
        \end{document}

3. Compile:  Now click on the  "typeset" icon on the upper-left. You will be prompted to save the file. Save the file with a .tex (not .txt) extension to your feature branch on disk. 
4. View: A PDF file will automatically pop up.

###Linux (Ubuntu)

####Download and install LaTeX

1. Open terminal (Ctrl - Alt + T).
2. Update APT cache (if you haven't already done so) by executing the following command:

		sudo apt-get update

3. Install LaTeX package by executing the following command on terminal:

		sudo apt-get install texlive-full

####Create Hello World Document

Now, we are ready to create a simple helloworld document using LaTeX.

1. Open/create: a tex file using 'vim helloworld.tex' in the terminal.
2. Write: In the editor, type this:

        \documentclass{article}
        \begin{document}
        Hello World!
        \end{document}

4. Save: press ESC key, the type ':wq' and hit ENTER.
3. Compile: to generate a pdf file using LaTeX execute the following command on terminal:

		pdflatex helloworld.tex

4. Display: to open the generated pdf file using evince, type the following command in terminal:

		evince helloworld.pdf

##LaTeX Resources and Templates

###Useful Links and Tutorials

1. [LaTeX tutorials](http://www.latex-tutorial.com/tutorials/)
2. [LaTeX2 for authors](http://latex-project.org/guides/usrguide.pdf)

###Templates

We have added some useful LaTeX templates [here](../Templates). Feel free to suggest more. 

