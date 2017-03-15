#Decision Neuroscience Lab – Getting Started#

Written by Dan F 070317

Last updated by Dan F 150317

Welcome to the Decision Neuroscience Lab! Here is a quick guide to installing the software and learning the coding practices/standards that we will use in the lab. Links to further information and helpful resources are also included. 

Many of these programs or workflows may be new to you, and it will take some time to master all of these pieces of software. However even a rough understanding of these programs will help you manage your code more effectively, and will allow us to work together to quickly develop experimental paradigms and analyses. 

If you get stuck please first look up the problem on the internet. Other members of the Change of Mind team might also be able to help if you cannot find a satisfactory answer on the web. If you find a resource that is especially useful (e.g. for Git, MATLAB or something else) then please share it around or send it to me. I’ll be creating a wiki for the lab based on this guide, so any suggested improvements and extra resources are much appreciated! 


Here we go:

1.	Get a copy of MATLAB for your computer, or find a workstation that has MATLAB installed. Ideally we want to use the most recent versions of MATLAB (2015 or 2016), but anything from 2013b onwards should be okay. The university of Melbourne supplies licenses for students and staff. A [guide for installing MATLAB](https://github.com/resbaz/lessons/blob/master/matlab/unimelb_matlab_install.md) is provided by Research Bazaar. 

Their [Github page](https://github.com/resbaz) also has a lot of helpful tutorials spanning a range of commonly-used programming languages.  

For those with a psychology background I would recommend the book [MATLAB for Behavioural Scientists](http://cw.routledge.com/textbooks/matlab/) for learning MATLAB, which also teach you how to create stimuli and experiment programs.

I would also highly recommend the book [Visual Psychophysics](https://mitpress.mit.edu/books/visual-psychophysics), which includes code for creating a wide range of visual stimuli, as well as creating psychophysical models (e.g. using signal detection theory). This book also contains a lot of information about the appropriate hardware and software for psychophysics research, which will be useful for designing our experiments. 

2. Create a Github account. This will allow you to be added to the Decision Neuroscience Lab group and contribute to code for experiments and analyses. You can do this at [github.com](https://github.com). 

Some great resources for learning Git are listed below (thanks to Cheng for providing these!) By using Git you can manage your code and track the changes that have been made (which is especially useful if you accidentally ‘break’ a program and need to go back to an earlier version). 

[Getting started/hello world activity](https://guides.github.com/activities/hello-world/)

[Github guides and tutorials](https://guides.github.com/)

[Video on using Git commands](https://www.youtube.com/watch?v=0fKg7e37bQE)

Here are some guides that show how using Git can be a powerful way to collaboratively develop code:

[Github introduction to flow](https://guides.github.com/introduction/flow/)

[Github comparing workflows](https://www.atlassian.com/git/tutorials/comparing-workflows) 

Here is a [tutorial](https://guides.github.com/activities/forking/) showing how you can also copy entire repositories to your own account, for when you want to make your own versions of experiments or analysis code.

When first using Git I would recommend making some test repositories (see the ‘hello world’ tutorial above) and playing around with different commands to see what they do. This might be easier once you install a Git program on your computer (see step 4). 

Also, Github offers [free private repositories](https://education.github.com/pack) for all students, so that you can upload your own code and protect it from prying eyes.

3.	Get added to a team in the Decision Neuroscience Lab organisation. This is an account which hosts code for completed and in-progress projects. Ask Daniel F or Will and they will add you to the organisation. The organisation Github page can be found [here](https://github.com/Decision-Neuroscience-Lab).

4.	Download and install an application that interfaces with Git. Which program you use depends on your personal preferences. Some popular programs are [SourceTree](www.sourcetreeapp.com/) and [TortoiseGit](https://tortoisegit.org/) (but please send me recommendations of other good alternatives). For this project I would recommend SourceTree as it is relatively easy to learn. 

A tutorial for SourceTree can be found [here](https://github.com/GSoft-SharePoint/Dynamite/wiki/Getting-started-with-SourceTree,-Git-and-git-flow). 


5.	Copy or ‘clone’ the online project repository to your own computer. This creates a copy of all of the project code on your own computer. A guide for doing this in SourceTree can be found [here](https://confluence.atlassian.com/sourcetreekb/clone-a-repository-into-sourcetree-780870050.html). The Simon Task project repository (which we will use to initially develop our experiments) can be found [here](https://github.com/Decision-Neuroscience-Lab/Simon-Task). 

6.	Download and install PsychToolbox version 3 (optional). This is a set of MATLAB functions for designing and running experiments. Installing this program will allow you to test and debug your experiment programs on your own computer. Everyone who will be coding the experimental paradigms will want to install PsychToolbox. Instructions for installing PsychToolbox can be found [here](http://psychtoolbox.org/download/). 

Peter Scarfe has a lot of excellent examples and [tutorials](http://peterscarfe.com/ptbtutorials.html) for creating experiments that present visual stimuli. Alternatively the book [Matlab for Behavioural Scientists](http://cw.routledge.com/textbooks/matlab/) has a section dedicated to using PsychToolbox . 

For a more advanced example of an experiment using PsychToolbox, I have uploaded a script (DF_example_experiment.m) to the ‘Simon Task’ repository. This code will not run (as it requires several additional image and data files) but provides some examples of how PsychToolbox commands can be used to calibrate the screen, get the monitor refresh rate and tightly control stimulus presentation timing.

7.	Learn the standards and coding practices for the project. Please see the document ‘DNLab Coding Practices and Tips’ for information on how to format your code and how to format MATLAB variables, structures and functions. Using a consistent format is very important when collaborating as a team, as it allows each person to easily see where changes have been made, and quickly interpret what these changes mean. If you have any suggestions for formatting (or have your own code organisation tips) please let me (Dan F) know so that I can add them to the document. 

If you feel particularly passionate about code formatting then you might want to read [The Elements of Matlab Style](https://www.bookdepository.com/The-Elements-of-MATLAB-Style-Richard-K-Johnson/9780521732581?ref=grid-view). This book contains a hundreds of tips for writing clearer MATLAB code. Some example tips are listed [here](http://blogs.mathworks.com/loren/2011/02/10/book-review-the-elements-of-matlab-style/).
 


After completing these steps you will be ready to contribute to the Change of Mind project code. Make sure to check the Github pages often as we will be constantly adding new resources and code updates! 


**Extra - Using Markdown and Pandoc**
The collaborative coding approach developed in Github can also be extended to the writing process, which may be useful for you and your collaborators. Here we will go through a writing-as-coding approch using the langauge Markdown. 

There are a number of text editors that work with markdown. Two simple editors that are freely-available are [Textwrangler](http://www.barebones.com/products/textwrangler/) (windows/mac) and [Macdown](https://macdown.uranusjr.com/) (macs only).

A guide to commonly-used Markdown formatting options is provided [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). 
