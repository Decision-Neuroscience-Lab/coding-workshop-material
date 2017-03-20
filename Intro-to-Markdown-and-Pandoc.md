# Introduction to Markdown and Pandoc

This section of the workshop introduces Markdown (a simple  language designed for easy formatting of documents) and Pandoc (a program that converts between document types). You can use Markdown and Pandoc to collaboratively write documents and track text modifications. Markdown is also excellent for noting down ideas and writing guides for experiments or analyses.
<br/><br/>


## Writing as coding (introduction to Markdown)

Markdown is a language with simple syntax that is useful for writing clear and well-formatted documents. You can do things like insert headings, make lists and convert words to **bold** and *italic* by inserting symbols such as * or #. These workshop documents were written in in Markdown. If you are viewing this on Github, click 'Raw' to see the Markdown code that produced this text.

Markdown is also code, which means that you can use repositories to keep track of your updates and changes. Wiki pages for projects or toolboxes (such as those on Github and Bitbucket) are commonly written in Markdown.

There are a variety of Markdown editors which show code and formatted text simultaneously for [Mac](https://macdown.uranusjr.com/) and [Windows](http://markdownpad.com/). You can also edit Markdown documents [in your browser](https://stackedit.io/).

Here is a great [tutorial](www.markdowntutorial.com) for learning markdown, as well as a [cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) in case you forget how to format something.



<br/>

## Collaborative writing


<br/>


## Converting across document formats (introduction to Pandoc)

Pandoc is a tool for converting documents across different file types. For example, Pandoc lets you convert your markdown document into a Microsoft Word .docx file, a LaTeX document, a pdf, or something else. There is an [impressive list](http://pandoc.org/index.html) of file types that pandoc can handle. Pandoc also has capabilities for working with a range of citation formats, for example Endnote.

You can download Pandoc [here](https://github.com/jgm/pandoc/releases/tag/1.19.2.1), and installation instructions can be found [here](http://pandoc.org/installing.html). You can even use Pandoc [in your browser](http://pandoc.org/try/) without installing it on your computer, although the browser version only converts between a limited number of file types. 

Pandoc uses the command line, which means that it does not have a graphical interface. A guide to using pandoc can be found [here](http://pandoc.org/getting-started.html). Most conversions can be done with a single command, as shown in this [list of examples](http://pandoc.org/demos.html). The list of examples contains links to the original and converted files, so you can see what your converted files will look like. 

As an example, you can convert this markdown file into a Microsoft Word .docx document by doing the following:

1. Open the command line (or terminal for Macs)
2. Navigate to the directory which contains the file that you want to convert.
3. Enter the following into the command line:

`pandoc Intro-to-Markdown-and-Pandoc.md -f markdown -t docx -s -o test-pandoc-file.docx`

The -f and -t parts tell pandoc which file types to convert between. The -o part goes before the output file name. An example of the word doc created from this markdown file is included in the workshop repository (test-pandoc-file.docx).

A handy list of commands is available in the [user guide](http://pandoc.org/MANUAL.html) or by entering `pandoc --help` into the command line.



<br/><br/>

<<< [Code Peer-Review](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Code-Peer-Review.md)						

[Back to workshop overview](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Coding%20Workshop%20DNLab.md)