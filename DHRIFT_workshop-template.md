---
title: This is the title
cover title: short title!
description: A description of the workshop.

programming_language: "choices are: jupyter, python, javascript, computer (for command line), or none"

learning objectives:
    - Understand what Python is and, in general terms, what it can do.
    - Run Python programs, both by interacting directly with the interpreter and by preparing and running scripts.
    - Distinguish among five core data types—integers, floats, strings, booleans, and lists.
    - Become familiar with core programming concepts, including variables, loops, and conditionals.
    - Engage with error output and use the internet and documentation to independently research language features.
    - Learn how to find and import code from external sources to solve more complex problems.

estimated time:
    - 3 - 4 hours

# has to be formatted like this!
prerequisites: 
    - command line: 
        description: Introduction to the Command Line (Required) This workshop makes reference to concepts from the Command Line workshop, and having basic knowledge about how to use the command line will be central for anyone who wants to learn about programming with Python.
        required: true
    - data ethics: 
        description: Data Ethics (Recommended) This workshop will give you a basis for thinking through the ethical considerations of your programming projects.
        recommended: true

instructors: 
    - 'Stephen Zweibel'
    - 'Leanne Fan'

authors:
    - 'Kalle Westerling'
    - 'Di Yoong'
    - 'Lisa Rhody'
    - 'Jojo Karlin'
    - 'Stephen Zweibel'
    - 'Patrick Smyth'

editors:
    - 'Di Yoong'
    - 'Lisa Rhody' 
    - 'Stephen Zweibel'

readings:
    - Want to learn programming, but not convinced that the Python language is the right language? Check out [Five Reasons Why Learning Python Is The Best Decision](https://medium.com/datadriveninvestor/)
    - "Some concrete ideas for how to use Python: [What Can I Do With Python?](https://realpython.com/what-can-i-do-with-python/)"

ethical considerations:
    - Python works by reducing data to portable units and presenting them in a way that prioritizes readability. These units are known as "data types" and include strings (words/letters), integers (numbers), booleans (true or false statements), and lists (groups of strings). The python grammar, which dictates how python statements ought to be ordered, values simplicity, efficiency, and concision. You can read more about Python values at [the Zen of Python](https://www.python.org/dev/peps/pep-0020/).
    - As we learn about the Python data types and grammar, keep in mind that working within any digital format requires making seemingly neutral choices that carry ethical consequences. When using python, be aware of the ways the ways that data is transformed into computable form. What choices are you making about your data? What is being included, and what is left out? What are reductions and assumptions necessary to encode your data? If you are more interested in thinking further about data types and our choices in relation to data, you should have a look at our [Data Literacies workshop](https://www.github.com/DHRI-Curriculum/data-literacies).

projects:
# Title and then description and link
    - The NEH Impact Index:
        description: Built by former Digital Fellow Patrick Smyth, The NEH Impact Index makes visible the distribution of funds by National Endowment for the Humanities across the United States. The website uses python to map projects, communities, and cultural institutions who have received NEH support. You can check out the code on Github.
        link: http://www.nehimpact.org/about
    - Mapping Arts NYC: 
        description: Mapping Arts NYC, created in 2019 by the Graduate Center’s Data for Public Good fellows, “is a project that explores the geography and representation of arts and culture in New York City over time.” It includes a number of Python scripts written to clean and make sense of all the data.
        link: http://gcdiprojects.org/MappingArtsNYC/
        
resources:
    - Digital Fellows’ Python Cheat Sheet: 
        description: See the Digital Fellows’ Python Cheat Sheet for handy commands that we cover in this workshop.
        link: https://curriculum.dhinstitutes.org/shortcuts/workshop/python

---

<!---
README: This workshop is a template for creating new workshops. Please read the instructions carefully.

General instructions for editing this template:
1) Duplicate this file (to avoid overwriting it) and rename/save it to the name of the workshop you are creating. Save the file as a Markdown file (`.md`) in the `workshops` folder, with hyphens to indicate spaces.
2) Edit the YAML front matter at the top of the file to include the correct information for your workshop (see more about that below).
3) Edit the content of the workshop with your lessons.

YAML Metadata:

Everything above this comment section (the YAML) constitutes the metadata of your workshop, which will populate the front page. It must be placed at the very top of your workshop file, beginning and ending with the three hyphens ---. Everything below (starting with #) is the actual content of your workshop. 

For the metadata, you should typically include some or all of the following:
- The title, and an excerpt (description) that will be displayed on the front page
- The learning objectives, which should be a list of bullet points
- The estimated time it will take to complete the workshop
- The dependencies, which should be a list of workshops that are required or recommended to complete this workshop
- The authors, which should be a list of the current and past authors of the workshop (if applicable)
- The editors, which should be a list of the current and past editors of the workshop (if applicable)
- The readings, which should be a list of readings that are relevant to the workshop
- The ethical considerations, which should be a list of ethical considerations that are relevant to the workshop
- The projects, which should be a list of projects that use the skills you'll learn in this workshop
- The resources, which should be a list of resources that are relevant to the workshop
- The goals, which should be a list of goals that are relevant to the workshop

The metadata you are currently seeing above is just an example, which you can use as a template for your own workshop. Make sure to follow the syntax exactly (or you will likely create errors), and to modify/delete any metadata that is not relevant to your workshop.
---> 

# Page 1

Welcome to my workshop! This is the first page (the first lesson).

<!--- Each h1 and h2 markdown header (the #) indicates the beginning of a new page. Use them to structure lessons in your workshops. --->

To add a lesson, simply type your lesson content below the header. You can use typical markdown styles to format your text.

There are several components you can incorporate into your lessons, including:

1. The Python REPL: You can embed the Python REPL into your lessons by using the following tag:

<PythonREPL/>

2. A download button: If you have files you'd like the participant to download, you can add a download button to your lessons with the appropriate files by using the following syntax:

<Download files='your_file1.csv, your_file2.md'>

Here, `your_file1` and `your_file2` are the two files to download (you can add as many as you'd like, just separate them with commas). The break tag at the end is just to add some space after the button. NOTE: You must include copies of the files indicated in the `uploads` folder.

3. An info box: Use <Info> to highlight interesting additional information.

<Info>
Here's an interesting aside! 
</Info>

3. A way to link internally to other workshops.

<Link workshop='python' page='56'>`Objects in Python`</Link>

This is necessary when linking to another workshop page. 'workshop' is the workshop file name, and the 'page' can be found in the URL query string, for instance:   `?user=dhri-curriculum&repo=workshops&file=command-line&**page=15**&instUser=dhri-curriculum&instRepo=dhrift-site-template` 

<!--- Most workshop lessons should include some form of a challenge, a solution, and an evaluation. See below for an example of each. --->

## Challenge

It's a good idea to include challenges in your workshop to help participants practice what they've learned.

## Solution

Provide a solution to the challenge.

## Evaluation

This is an evaluation, which you can utilize in the form of a quiz. For the syntax, see the example question and quiz below:

What are the characteristics of the REPL? Select all that apply.

<Quiz>
- The REPL has a prompt that begins with `$`.
- The REPL has a prompt that begins with `>>>`.*
- The REPL and the terminal are the same thing.
- The REPL can be used to evaluate mathematical expressions like `2 + 2`.*
</Quiz>

<!--- For quizzes, each list item in the <Quiz> tags is a potential answer. To indicate correct answers, place an asterisk at the end. --->

<!-- Each section end should have a collection of key words related to the lesson, like so: -->
<Keywords>
- keyword 1
definition 1

- keyword 2
definition 2
</Keywords>

<!--- Keywords are a good way to reinforce the key concepts of the lesson. Definitions cannot be multiple paragraphs. --->

# Section 2

This is the second section (the second lesson) of the workshop. Provide as many pages as you'd like.

# Section 3

# Section 4

# Section etc.
