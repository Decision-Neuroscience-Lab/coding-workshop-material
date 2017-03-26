## 3. Code Review

### What is code review?

Code review is a peer-review process for code, with many of the same benefits as peer-review of an academic manuscript. One or more people go through a script or section of code and provide feedback about:

1. Possible bugs/errors
2. Sections that are unclear or difficult to understand
3. Possible improvements or options for extending the code

A popular code review protocol usually proceeds as follows: the primary author of the code and the reviewer(s) usually sit down together and first discuss the structure and purpose of the code. The reviewers then look through the code independently from the author. Reviewers usually make notes and/or leave comments in the code, which are then discussed online or in-person. The primary author of the code can then choose to make or reject changes suggested by the reviewer(s). 

There are multiple benefits of this process. The author gets valuable feedback; others may spot bugs that may be missed by the code's primary author(s). Reviewers get a glimpse of how other people write and structure their programs, and often learn new approaches or methods that are relevant to their own work. Sharing knowledge among collaborators also trains more people to solve (and help with) a wide variety of problems, and raises the [bus factor](https://en.wikipedia.org/wiki/Bus_factor). 

### Why do we need code reviews in science?

People always make at least some mistakes when writing code. Professional programmers have long acknowledged this fact of life;  finding and fixing bugs (debugging) is considered an essential part of writing software. If someone tells you that they don't make mistakes when coding then 1.) don't believe them and 2.) do NOT use their code for your own work. It is much more likely that they simply have not been able to identify the bugs/mistakes in their code, or have not bothered to look closely enough.    

Broadly speaking, there are two types of bugs that are commonly encountered. The first category of bugs crash your code and require fixing before you can run your scripts. However, the most insidious bugs are those in the second category, which affect your experiment or results but still allow your code to run. These small bugs can sometimes have devastating consequences. Here is [a rather extreme example](http://boscoh.com/protein/a-sign-a-flipped-structure-and-a-scientific-flameout-of-epic-proportions.html) of a simple bug heavily influencing the direction of an academic field, and ultimately leading to the retraction of several papers in Nature and Science. As another example, some researchers (known to one of the authors of this workshop) lost 50+ EEG datasets because of one number entered incorrectly into a stimulus presentation script. Dan F similarly lost two datasets the first time he programmed an experiment in PsychToolbox, due to six cells in an excel spreadsheet being copied incorrectly.

The point here is not that we should be terrified of writing code, but that we need to put measures in place to minimise the number of errors in our own software. We researchers are in a particularly tricky position; most of our software is written in-house (and is not seen/evaluated by the wider community) and is written by non-professional programmers. Code review is one practice that we can adopt to improve the quality of our own code. It also forces us to organise our code in a way that other people (and our future selves) can understand what the code is doing. This is very useful when we have to rerun an analysis for manuscript reviewer 2, or when someone inevitably re-uses a chunk of your code in their own data analysis scripts.

Code review is one of many tools used for debugging code. Here is [a paper](https://arxiv.org/pdf/1210.0530v1.pdf) that lists some other approaches to finding and fixing bugs in your code. And here is [another one](http://journal.frontiersin.org/article/10.3389/fpsyg.2014.01435/full) written for cognitive neuroscientists.

### Protocol and guidelines

Here is a draft protocol for code reviews. This is a working draft and should be modified as we learn about better methods. To date there is not much information on code reviews in academic settings, so for now we must rely on trial-and-error.  

We can proceed as follows:

1. The code's primary author(s) **finish a complete version** of their code that runs without crashing, and includes informative comments explaining what the code does. Please do not give code that doesn't run to a reviewer, unless the goal of the code review is to find out why your script is crashing.

2. An author **approaches a potential reviewer** and asks them to review. When choosing someone to review your code it is good to ask a person that is doing a similar project or analysis technique. This allows the reviewer to see how others design experiments or analyses in their field of research. However, reviewers with different areas of expertise can also be good, as it can broaden reviewers' knowledge of experimental paradigms and data analysis techniques. 

3. The reviewer is given access to the Git repository containing the code to be reviewed and **makes a new branch**. This branch should be called something like 'danf-code-review'. Make sure to branch off of the most recent version of the code. 

4. The reviewer **makes notes, and makes changes/inserts comments in the code**. For example, comments could be included that ask for further explanation/clarification or suggest an improvement. Reviewer comments should be prefaced by a keyword, so that the code author(s) can easily locate them using the search function. For example, you could preface each comment with DANF_COMMENT. Try to write informative comments and explain the reasons why you have made each suggestion.

5. The reviewer **submits a pull request** to merge their reviewed version back into the master or working branch. Notes and feedback on the code can be summarised in the pull request description. Changes to the code will be highlighted in the summary of changes on Github/Bitbucket. The reviewer's suggested changes could be merged into master branch (or a separate working branch) at the author's discretion. However, the reviewer should never approve their own pull request; the code author ultimately decides what will (or will not) be done to the code. Author and reviewer may also meet and discuss any features of the code or recommended changes. 

6. (recommended step) the author **buys the reviewer at least one coffee** or beverage of choice, and probably should treat the reviewer to lunch for reviewing longer pieces of code. Code review is a laborious process, so be thankful for the reviewer's time!


<br/>

This is the basic structure of the proposed code review. Below are some links that contain advice for effective review, mostly written for teams of professional programmers:

<https://alexgaynor.net/2013/sep/26/effective-code-review/>

<http://blog.regehr.org/archives/1153>

<https://github.com/thoughtbot/guides/tree/master/code-review>

<https://smartbear.com/learn/code-review/best-practices-for-peer-code-review/>

<https://www.atlassian.com/agile/code-reviews>

<https://www.ibm.com/developerworks/rational/library/11-proven-practices-for-peer-review/>

## Navigation

<<< [Introduction to Git](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Writing-Clear-Code.md)
				
[Introduction to Markdown and Pandoc](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Intro%20to%20Markdown%20and%20Pandoc.md) >>>	

[Back to workshop overview](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Coding%20Workshop%20DNLab.md)