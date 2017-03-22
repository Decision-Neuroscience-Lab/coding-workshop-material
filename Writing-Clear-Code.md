# Writing Clear Code

![Bad Code](images/badcodememe.png)

Some links to start out:

[MIT - Good MATLAB Programming Practices](http://www.mit.edu/~pwb/cssm/GMPP.pdf)

[Minimizing bugs in Cognitive Neuroscience programming](http://journal.frontiersin.org/article/10.3389/fpsyg.2014.01435/full)

[Writing Clear Code - Princeton University](http://introcs.cs.princeton.edu/java/11style/)

[Top MATLAB 10 Practices that make me cry](https://blogs.mathworks.com/videos/2010/03/08/top-10-matlab-code-practices-that-make-me-cry/)

[IBM - Six Ways to Write more Comprehensible Code](https://www.ibm.com/developerworks/library/l-clear-code/)

[Top 15+ Best Practices for Writing Super Readable Code](https://code.tutsplus.com/tutorials/top-15-best-practices-for-writing-super-readable-code--net-8118)

## Purpose and examples of clear/unclear code 

### Purposes:

- Clean code is easy to read

- Makes it easier to pass your project on to the next person

- Easier for yourself/others to spot an error, and debug it early.

- Allows for easier collaboration, less confusion among teammates.


### Example of unclear code:

### Example of clear code:

## Advice on writing and formatting MATLAB code

- Use long variable names with underscores (HELLO_DECISION_NEUROSCIENCE_LAB) to avoid lengthy documentation.
It is also easier for others to understand your variables and functions.

- Make good use of comments, but avoid super-obvious ones.

- Adopt a guideline for variable usage and commenting style.

- It's nice to line up equal signs, spaces, and commas; this helps a lot with spotting errors.

- Have consistent indentation and styling. Styling is a personal preference, but keeping the styling consistent
makes it easier to read.

- Keep functions small! They can be reused for other functions. It also helps make it easier to read.

- If possible, try to keep lines short by using ellipsis (...)

- Large indents can help late at night when those 2-space indents are hard to see.

Source: [MIT - Good MATLAB Programming Practices](http://www.mit.edu/~pwb/cssm/GMPP.pdf)




### Avoid variable names that are similar to function namesMATLAB has a wide variety of available functions. Some of these functions may share the same name with variables that you want to use in your code. For example, ‘path’ is a variable name that might be used to denote a file save location in a script, but is also a MATLAB function. When a MATLAB function name is used as a variable, that function will stop working in that script (which can cause unforseen problems). Wherever possible use variable names that are unlikely to have the same name as MATLAB functions.Similarly, try to avoid generic programming terms like ‘dir’ for variable names. If in doubt, enter `which ` or `help ` followed by the variable name into the command line, to see if an existing function shares the same name as your variable. 

### Create informative variable names
More generally, it is good practice to make your variable names as informative as possible. For example, rather than ‘path’ you could use the variable ‘filePath’ or ‘dataFilePath’ or ‘saveFilePath’. This helps anyone reading the code (including your future self) understand what each variable refers to without needing to see how it was defined earlier in the code. 

Another example would be replacing `maxf` with something like `maxForce` or `tstart` with `startTime`. However it is good not to make variable names too long (for example `maxForceForThisTrialInBlock1`) as they become difficult to read. The best balance is a succinct variable name that is still easily understood in the context of the code. When in doubt, always err towards longer variable names if it makes them easier to understand. ### Write informative comments
It is also good to add comments that clearly explain what each section or chunk of the code is doing. Commenting takes time while writing the code, but greatly speeds up the debugging process (and you will always need to debug code). Using informative variable names and comments also contributes to an important secondary purpose of writing code: to show how an operation or calculation is performed. Clear code can be more easily modified and is easier adapt for use in other scripts, functions or projects. 

*TODO include examples of informative comments*

### Define hard-coded variables at the beginning of the script
Wherever possible ‘hard-coded’ variables (values that are defined in the code but are often adjusted or changed) should be defined at the top of the script. This makes it easy to keep track of variables without digging through the bulk of the code in order to find them.

For example:

```
% Define instructions text parameters
instructionsText = 'Get Ready';
instructionsTextSize = 12;
instructionsTypeface = 'Arial';
instructionsTextColour = [255, 255, 255];


% Format and write the text to the screen
Screen(scrID, 'TextSize', instructionsTextSize);
Screen(scrID, 'TextFont',  instructionsTypeface);
DrawFormattedText(scrID, instructionsText, 'center', instructionsTextColour);
```### Tag end statements with their respective if/for/while commandsOne very useful trick is to attach a comment after `end` statements denoting what is being ended. For example:```if someVariable == 1
	while anotherVariable < 200		anotherVariable = anotherVariable + 1;	end % of while anotherVariableend % of if someVariable```This is particularly useful when you have a lot of nested loops (i.e. loops within loops) or `if` statements. It is also useful for detecting when you add/remove an `end` statement and the existing `end` statements don’t line up with their intended `for/while/if` statements. 

### Use whitespace
Adding spaces between parts of a line of code, or between lines of code, can make your scripts a lot easier to read. 

For example, it is useful to put spaces between variables and mathematical operators, for example:```
answer=(A+B)/1000 				answer = (A + B) / 1000
```Whitespace is also useful when writing if/while/for statements:```if variableA>variableB&&variableC>variableDif variableA > variableB && variableC > variableD```

Using commas followed by spaces is also very useful for delineating elements of a vector or input arguments for a function:

```exampleVector = [1 333 4 55 3+1 42/55 111];

exampleVector = [1, 333, 4, 55, 3+1, 42/55, 111];store_rt_data(meanRT,medianRT+1,modeRT,stdevRT/sqrt(nSubjects))store_rt_data(meanRT, medianRT + 1, modeRT, stdevRT / sqrt(nSubjects))```
You may adopt different styles of code organisation, but the main point is to think about how you can use whitespace (blank spaces, blank lines etc.) to make your code easier to understand. You can even use spaces selectively to group elements within a line of code. For example, you can group certain mathematical operations together to make an equation clearer:`A = sqrt(B+10) / mean(C-2) + D^2` 

### Further reading

If you feel particularly passionate about code formatting then you might want to read [The Elements of Matlab Style](https://www.bookdepository.com/The-Elements-of-MATLAB-Style-Richard-K-Johnson/9780521732581?ref=grid-view). This book contains a hundreds of tips for writing clearer MATLAB code. Some example tips are listed [here](http://blogs.mathworks.com/loren/2011/02/10/book-review-the-elements-of-matlab-style/).

## Lab coding standards and practices
### Variable naming
Different projects use different naming conventions for variables, structures and functions in MATLAB. For example:
`VariableName`
`variableName``variable_name``Variable_Name``Structure.VariableName``structure.variable_name``VARIABLENAME``VARIABLE_NAME`

For large projects teams usually agree on variable naming conventions to be used throughout the project. This makes the code a lot clearer and variables easier to identify. Using a consistent variable naming style also means that you don’t need to check how a variable was written each time you use it. 

Each person has their preferred variable naming style (and might use different styles in separate projects). However setting a 'lab standard' style is useful to help us to easily read other lab members' code. This will be especially useful in code reviews (so that others don't need to adjust to a new style when they read your code).The convention we will use for variables is called **lower camel**. This style uses a lower case letter to begin the first word of a variable name. Subsequent words begin with a capital letter, which looks like humps on a camel’s back. Further information can be found [here](https://en.wikipedia.org/wiki/Camel_case).For example: 
`lowerCamelCase``exampleVariableName``reactionTime`In MATLAB we will use a different naming convention for structures. The first letter of each word will be capitalised (known as **upper camel**). By doing this we can easily identify structures and variables based on how they are named. 

For Example:`Structure.lowerCamel`
`StoredData.reactionTimes`To differentiate variables and structures from function names we will use **lowercase letters and underscores** for function names.

For example:`display_stimulus(inputArg1, inputArg2)`
`record_reaction_time(trial, reactionTimeThisTrial)`Functions from toolboxes or other projects (e.g. PsychToolbox) will have different conventions for function names (PsychToolbox uses upper camel, EEGlab and DDTBOX uses lower case with underscores). This mixture of function naming conventions is unavoidable, however it is usually easy to distinguish these after some experience with MATLAB code.

Feel free to use other variable/structure/function naming conventions in your own projects if you wish. In any case (pun intended) it is useful to note your naming conventions in the script headers or in the wiki for a project or repository. When making changes to someone else's code, always remember to use the naming conventions that they have defined in their project.

Different naming conventions may work best with different programming languages. If you have a good style for R or Python please let us know or add this to the workshop wiki!

<br/><br/>

[Introduction to Git](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Introduction-to-Git.md) >>>

[Back to workshop overview](https://github.com/Decision-Neuroscience-Lab/coding-workshop-material/blob/master/Coding%20Workshop%20DNLab.md)
