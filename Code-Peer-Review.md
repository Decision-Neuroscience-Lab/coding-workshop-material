## Code Peer-Review

### What is code review?

Code review is a peer-review process for code, with many of the same benefits as peer-review of an academic manuscript. One or more people go through a script or section of code and provide feedback about:

1. Possible bugs/errors
2. Sections that are unclear or difficult to understand
3. Possible improvements or options for extending the code

The primary author of the code and the reviewer(s) usually sit down together and first discuss the structure and purpose of the code. The reviewers then look through the code independently from the author. Reviewers usually make notes and/or leave comments in the code, which are then discussed online or in-person. The primary author of the code can then choose to make or reject changes suggested by the reviewer(s). 

There are multiple benefits of this process. The author gets valuable feedback; others may spot bugs which are difficult to find if you are the one who originally wrote the code. Reviewers get a glimpse of how other people write and structure their programs, and often learn new approaches or methods that are relevant to their own work. Sharing knowledge among collaborators also trains more people to solve (and help with) a wide variety of problems, and reduces the [bus factor](https://en.wikipedia.org/wiki/Bus_factor). 

### Why do we need code reviews in science?

People always make [at least some mistakes](http://ivory.idyll.org/blog/automated-testing-and-research-software.html) when writing code. Professional programmers have long acknowledged this fact of life;  finding and fixing bugs (debugging) is considered an essential part of writing software. If someone tells you that they don't make mistakes when coding then 1.) don't believe them and 2.) do NOT use their code for your own work. It is much more likely that they simply have not been able to identify the bugs/mistakes in their code, or have not bothered to look closely enough.    

The most insidious bugs are those that affect your experiment or results, but still allow your code to run. These small bugs can sometimes have devastating consequences. Here is [a rather extreme example](http://boscoh.com/protein/a-sign-a-flipped-structure-and-a-scientific-flameout-of-epic-proportions.html) of a simple bug heavily influencing the direction of an academic field, and ultimately leading to the retraction of several papers in Nature and Science. As another example, some researchers (known to one of the authors of this workshop) lost over 50 EEG datasets because of one number entered incorrectly into the stimulus presentation script. Dan F similarly lost two datasets the first time he programmed an experiment in PsychToolbox due to six cells in an excel spreadsheet being copied incorrectly.

The point here is not that we should be terrified of writing code, but that we need to put measures in place to minimise the number of errors in our own software. We researchers are in a particularly tricky position; most of our software is written in-house (and is not seen/evaluated by the wider community) and by non-professional programmers. Code review is one practice that we can adopt to improve the quality of our own code. It also forces us to organise our code in a way that other people (and our future selves) can understand what the code is doing. This is very useful when we have to rerun an analysis for that pesky manuscript reviewer 2, and when someone (probably you) inevitably re-uses a chunk of your code for use in their own data analyses.

In addition, here is [a paper](https://arxiv.org/pdf/1210.0530v1.pdf) that lists some other approaches to finding and fixing bugs in your code. And here is [another one](http://journal.frontiersin.org/article/10.3389/fpsyg.2014.01435/full) written for cognitive neuroscientists.

### Protocols and guidelines

Here is [a great guide](https://alexgaynor.net/2013/sep/26/effective-code-review/) for doing code reviews.

### Establishing a peer-review process




Links to advice on code peer-review (temporary, decide if we want to include)

http://blog.regehr.org/archives/1153

https://github.com/thoughtbot/guides/tree/master/code-review

https://smartbear.com/learn/code-review/best-practices-for-peer-code-review/

https://www.atlassian.com/agile/code-reviews

https://www.ibm.com/developerworks/rational/library/11-proven-practices-for-peer-review/

## Navigation

<<< [Introduction to Git](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Writing-Clear-Code.md)
				
[Introduction to Markdown and Pandoc](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Intro%20to%20Markdown%20and%20Pandoc.md) >>>	

[Back to workshop overview](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Coding%20Workshop%20DNLab.md)