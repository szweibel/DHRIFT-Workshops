---
title: How to Use DHRIFT
cover title: How to Use DHRIFT
description: "This workshop is designed for those who are interested in learning and teaching with DHRIFT, including those who want to create and customize their own DHRIFT site, those who would like to write their own workshops to publish with the DHRIFT platform, and for workshop facilitators and developers who would like to make use of DHRIFT’s minimal computing environment to create their own DH curricula." 

programming_language: 'jupyter'

learning objectives:
    - Understand the basic features and affordances of the DHRIFT platform to create and manage curricula
    - Learn how to write and publish workshops with the DHRIFT platform
    - Learn how to create and customize a DHRIFT site
    - Learn how to clone and modify an existing DHRIFT instance
    - Learn how to use the wizard to create an institute based on your community’s needs

estimated time:
    - 3 hours

authors:
    - 'Zachary Lloyd'
    - 'Lisa Rhody'
    - 'Stephen Zweibel'
    - 'Leanne Fan'

facilitators:
    - 'Zachary Lloyd'
    - 'Lisa Rhody'
    - 'Stephen Zweibel'
    - 'Leanne Fan'
---

# Introduction

Welcome to DHRIFT!

During this workshop, you will learn about the DHRIFT platform, including its directory of available workshops, interactive features, and pedagogical philosophy. You will learn to build your own DHRIFT website for a mock institute, including modifying and customizing existing DHRIFT content. By creating DHRIFT sites, you will also learn about DHRIFT’s underlying technologies: how workshop markdown files are created, ingested, and displayed, how they are stored and processed through GitHub actions, and how institute leaders can use the platform's wizard to build an institute based on your community’s needs.

__Quick Links:__

This workshop is meant as a starting point for utilizing the DHRIFT platform. We also encourage you to visit and bookmark other resources, such as:

- The extended documentation and reference guides: TODO: link to docs

- The DHRIFT GitHub repository: [DHRIFT GitHub](https://github.com/DHRI-Curriculum/DHRIFT)

- The DHRIFT informational website, which provides more information about the DHRIFT project, its team, and news/updates: [DHRIFT Website](https://dhrift.org)

# Learning with DHRIFT

Let's begin by exploring what DHRIFT is and how you can use it to learn digital humanities concepts.

## What is DHRIFT?

To start with, DHRIFT is the platform you are currently using to access this workshop!

To be more specific, DHRIFT (Digital Humanities Resource Infrastructure for Teaching Technology) is an open educational resource (OER) and publication platform for digital humanities (DH) workshops. Designed by humanities scholars for humanities scholars, DHRIFT provides a minimal computing, accessibility-aware, and interactive environment for teaching fundamental DH concepts. 

The platform includes a core set of more than 10 reviewed and tested workshops that have been developed and tested during two NEH-funded, week-long institutes, called the Digital Humanities Research Institutes (DHRI). Workshop topics range from learning the basics of Python, JavaScript, and R to conducting research through text analysis, data wrangling, and mapping. You can see the full list of workshops on the workshops page, accessible from the header menu or [by clicking here](https://app.dhrift.org/workshops/?instUser=dhri-curriculum&instRepo=dhrift-site-template&user=dhri-curriculum&repo=workshops). 

DHRIFT’s core workshops are always accessible from and usable on our website; however, its flexible framework also allows users to build their own customized, static DHRIFT sites and tailor them for a variety of situations, such as teaching an undergraduate or graduate class, hosting a week-long skills institute, or organizing a series of professional development workshops. DHRIFT facilitates an instructor or organizations’ ability to reproduce, adapt, and publish DH workshops with interactive, learner-focused features. All workshop content is accessible in the browser, avoiding the need for learners to install software or set up complex computing environments.

## Underlying Technologies

DHRIFT is built on a few key technologies that make it easy to create, manage, and publish DH workshops. These technologies include:

- **GitHub**: DHRIFT uses GitHub to store and manage workshop content. Each workshop is stored in a GitHub repository, which contains the workshop’s markdown files, images, and other assets. GitHub also provides version control, so you can track changes to your workshop content over time. 

- **Markdown**: DHRIFT uses Markdown to write workshop content. Markdown is a lightweight markup language that is easy to read and write. It allows you to format text, add images, and create links without having to write HTML.

- **YAML**: DHRIFT uses YAML to configure workshop metadata. YAML is a human-readable data serialization format that is easy to read and write. It allows you to specify metadata such as the workshop title, author, and description.

- **React**: DHRIFT’s frontend is built with React, a JavaScript library for building user interfaces. React allows us to create interactive, responsive, and accessible interfaces for our workshops.

- **WebAssembly**: DHRIFT uses WebAssembly to run code snippets in the browser. WebAssembly is a low-level programming language that is designed to run fast and efficiently in web browsers. It allows us to incorporate code editors in a secure and sandboxed environment so that learners can immediately see the results of their code.

- **GitHub Actions**: DHRIFT uses GitHub Actions to automate the process of building and deploying workshop content. When you make changes to your workshop content, GitHub Actions will automatically build and deploy the changes to your DHRIFT site.

We'll be exploring these technologies in more detail throughout the workshop, so don't worry if you're not familiar with them yet!

## The Learning Experience

DHRIFT is designed to be an interactive and engaging platform for learning digital humanities concepts. Let's explore some of the features and affordances of the DHRIFT platform, including interactive quizzes, challenges, and code editors. We'll also discuss how DHRIFT workshops are structured and how you can navigate and interact with them.

It should be noted that DHRIFT can be used in a variety of settings, including remote, in-person, and self-instructional modalities. The platform is designed to be accessible to learners of all backgrounds and skill levels, from beginners to more advanced users. Whether you're new to digital humanities or an experienced practitioner, DHRIFT has something to offer you.

Let's dive into the platform and see what it has to offer!

## Using the DHRIFT Platform

If you have made it this far, you have already become familiarized with the standard DHRIFT workshop format. 

Each workshop has a front page that provides the workshop’s description, learning objectives, estimated time, authors, workshop facilitators, ethical considerations, and more. To begin a workshop, simply click the Start Workshop button under the main description or below the workshop's additional details.

![DHRIFT Workshop Front Page](ws-frontpage.png)

Each individual workshop is divided into sections and subsections. You can navigate between sections by using the back and forward buttons in the navigation bar below each section. You can also access the table of contents for each workshop by clicking on the Workshop Overview button in the top-right corner of the screen.

![DHRIFT Workshop Navigation](ws-overview.png)

Workshop content can take many forms: text, images, code snippets, interactive exercises and quizzes, and more. Let's explore some of these features.

## Quizzes

DHRIFT workshops may include quizzes to test your knowledge and understanding of the material. Quizzes can take many forms, including multiple-choice, true/false, and short answer questions.

A common quiz type you'll encounter in our core curriculum is the multiple-choice question, which looks like this:

### Evaluation

What front-end technology does DHRIFT use to build its user interfaces?

<Quiz>
- React*
- Angular
- Vue
- Ember
</Quiz>

To answer a multiple-choice question, simply click on the answer you think is correct and hit the Check My Answer button. If you choose the correct answer, you will be congratulated by a Correct! message. If you choose the incorrect answer, you will prompted to try again.

## Challenges

DHRIFT workshops may also include challenges to test your skills and understanding of the material. Like quizzes, challenges can take many forms, including coding exercises, short answer questions, and more.

While we will always provide a solution to the challenge, we encourage folks to try the challenge on their own first before looking at the solution. Therefore, we initially hide a solution and provide a button to reveal it, like so:

### Challenge

Where are DHRIFT workshops stored?

### Solution

<Secret>
In a GitHub repository.
</Secret>

To reveal the solution to the challenge, simply click on the Reveal button.

## Interactive Code Editors

DHRIFT workshops may also include interactive code editors that allow you to write and run code directly in your browser. These code editors are powered by WebAssembly, which allows you to run code snippets in a secure and sandboxed environment.

For demonstration purposes, this workshop includes a JupyterLite notebook that allows you to write and run multiple coding languages. To use the notebook, simply click the Open Code Editor button near the top-right corner of the screen. This will open the code editor in a slide-out panel on the right-hand side of the page.

Let's try running a simple Python code snippet. Click the Open Code Editor button to open the Jupyter code editor, then create a new Python file by clicking the Python (Pyodide) button. If it prompts you to choose a kernel, select Python(Pyodide).

Next, type the following code into the first cell of the notebook:

```python
print("Hello, world!")
```

When finished, press <kbd>shift<kbd> + <kbd>enter</kbd> to execute the code. The output of the code will then be displayed below.

### Resizing and Closing the Code Editor

You can also resize the width of the code editor by dragging the left-hand side frame of the editor window. This allows you to see more or less of the code editor, depending on your needs.

To close the code editor, simply click the Close Code Editor button at the top of the code editor panel.

## Additional Code Editors

DHRIFT workshops may also include code editors for other programming languages, such as JavaScript, R, and more. These code editors work in a similar way to the Jupyter notebook editor, allowing you to write and run code directly in your browser. Currently, there is support for the following:

### Python and Jupyter Notebooks

You have already seen the JupyterLite notebook in action. DHRIFT also supports a standard Python editor, which allows you to write and run Python code in a basic script-style code editor.

![Python Code Editor](python-editor.png)

In addition, DHRIFT also provides a dedicated REPL (Read-Eval-Print Loop) for Python, which allows you to write and run simple Python commands.

![Python REPL](python-repl.png)

### JavaScript

DHRIFT supports a JavaScript code editor, which allow you to write and run JavaScript code directly in your browser. JavaScript is a popular programming language for building interactive web applications, games, and more.

![JavaScript Code Editor](js-editor.png)

### R

DHRIFT supports an R code editor, which allow you to write and run R code directly in your browser. R is a popular programming language for statistical computing and data analysis.

TODO: image of R editor

### Command Line

DHRIFT supports command line code editors, which allow you to run shell commands directly in your browser. This is useful for working with files, directories, and other system-related tasks. _Note that the command line editor is an emulated terminal and will not have access to your local file system._

![Command Line Editor](cl-editor.png)

### HTML and CSS

DHRIFT supports HTML and CSS code editors, which allow you to write and style web pages directly in your browser. HTML is a markup language for creating web pages, while CSS is a stylesheet language for styling web pages.

TODO: image of HTML and CSS editor

## Downloading Workshop Materials

DHRIFT workshops may also include downloadable materials, such as PDFs, slides, datasets, and more. These materials are typically provided to help you follow along with the workshop content, complete exercises, and refer back to the material later.

Here's an example of how downloadable materials might be presented in a workshop:

### Downloadable and Importable Materials

TODO: add download button with something

TODO: add import button with something  

## Glossary

Often, DHRIFT workshops will use specific terms or concepts that may be unfamiliar. In this case, we provide a Key Terms section that defines and explains these terms, like so:

<Keywords>
- DHRIFT
DHRIFT (Digital Humanities Resource Infrastructure for Teaching Technology) is an open educational resource (OER) and publication platform for DH workshops. Designed by humanities scholars for humanities scholars, DHRIFT provides a minimal computing, accessibility-aware, and interactive environment for teaching fundamental DH concepts.

- Markdown
Each workshop is created using Markdown, a lightweight markup language that is easy to read and write. Markdown allows you to format text, add images, and create links without having to write HTML.
</Keywords>

 To access the full glossary of key terms for DHRIFT workshops, you can click on the Glossary button in the header section of the site.

![Glossary](glossary.png)

## Workshop Completion

Each workshop typically ends with a Theory to Practice section, which provides an opportunity to apply what you have learned in the workshop to a real-world scenario. This section may include case studies, projects, or reflection exercises.

![Theory to Practice](theory-to-practice.png)

In general, these sections are intended to offer learners a chance to extend their understanding beyond the workshop and apply their new skills and knowledge in practical ways. For instance, you might be asked to analyze a dataset, create a visualization, or build a simple web application based on the concepts you have learned in the workshop.

# Teaching with DHRIFT

### Pedagogical Philosophy

DHRIFT is designed with a learner-focused pedagogical philosophy that emphasizes accessibility, interactivity, and engagement. The platform has been developed in conversation with an extensive community of DH graduate students, faculty, administrators, librarians, curators, and independent scholars, and our advisory board is drawn from a cross section of DH practitioners at institutional types such as community colleges, liberal arts colleges, regional colleges, and Historically Black Colleges and Universities (HBCUs). By engaging with this diverse community, we have been able to develop a platform that meets the needs of a wide range of learners and instructors.

Additionally, DHRIFT values the principles of open education and open access. All workshop content on the platform is freely available to anyone who wishes to use it, and all workshops are licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. This means that you are free to use, share, and adapt the content for non-commercial purposes, as long as you provide attribution to the original authors and share any derivative works under the same license.

## Workshop Philosophy

Our curricula reflect the pedagogical values of humanities instruction, drawing from years of feedback and iteration. Both textual and visual in design, workshops attempt to accommodate different learning styles. By embedding a technical interface in the curricula, DHRIFT streamlines the learning environment for both instructors and learners and reduces confusion caused by context switching. DHRIFT workshops emphasize practical coding through a humanities lens, providing learners tools to extend their skills into new domains relevant to their research.

DHRIFT workshops are also designed to be accessible to learners with disabilities. The platform is built with accessibility in mind, following best practices for web accessibility and usability. DHRIFT workshops are designed to be screen reader-friendly, keyboard navigable, and color contrast compliant.

Let's look at some best practices for teaching with DHRIFT.

## Best Practices

When teaching with DHRIFT, there are a few best practices you can follow to ensure a positive and engaging learning experience for your students. Here are some tips to keep in mind:

- **Set Clear Learning Objectives**: Clearly present the learning objectives for each workshop and communicate them to your students at the outset. This will help students understand what they will be learning and why it is important.
- **Provide Context**: Provide context for the material you are teaching and explain how it relates to the broader areas of research students might be interested in. Additionally, consider ethical considerations and implications of the material you are teaching.
- **Encourage Active Learning**: Encourage students to actively engage with the material by asking questions, participating in discussions, and completing exercises. This will help reinforce their learning and make the material more memorable.
- **Use a Variety of Teaching Methods**: Use a variety of teaching methods to keep students engaged and accommodate different learning styles. This could include different forms of group work in which students attempt to solve a problem together, or individual work in which students complete a task on their own.
- **Provide Feedback**: Provide feedback to students on their progress as the workshop unfolds. This could include feedback on quizzes, challenges, and exercises, as well as general feedback on their understanding of the material. Reiterate key concepts to bolster understanding.

While DHRIFT tries to accommodate these best practices in terms of its design and content, it is, as always, up to the instructor to ensure that these practices are implemented effectively in the classroom.

## Using a Pre-Existing Resource

Although you can create your own workshops from scratch, we also encourage you to explore and utilize the existing DHRIFT workshops available on the platform. These workshops have been developed and tested by experienced DH practitioners and educators and cover a wide range of topics and skill levels. By using these pre-existing resources, you can save time and effort in developing your own workshops and benefit from the expertise of the wider DH community.

Depending on your needs and your students' experience, it is generally a good idea to start with the basics and build up to more advanced topics. Looking at the "Prerequisites" section of a workshop can help you determine if the workshop is appropriate for your students' skill level. For example, you might wish to have students work through the Command Line workshop before moving on to the Python workshop, as the former provides a foundation for the latter.

If you are teaching a live session using a workshop from the platform, you might also suggest that students work through the workshop on their own before the session, so that they can come prepared with questions and be ready to engage with the material in a more meaningful way.

## Scaffolding a Workshop

When teaching with DHRIFT, you may want to scaffold your session to guide students through the material in a structured and logical way. Scaffolding involves breaking down the material into manageable chunks and providing support and guidance to help students progress through the material. 

The platform itself is designed to scaffold the learning experience, with workshops divided into sections and subsections that guide students through the material step by step. Still, it is a good idea as an instructor to work through the material yourself and identify which sections might be more challenging for students and where additional support might be needed. 

## Teaching and Community Engagement

Additionally, DHRIFT is committed to fostering a community of practice around digital humanities pedagogy. We encourage instructors, learners, and developers to engage with the platform, share their experiences, and contribute to the ongoing development of the platform. We welcome feedback, suggestions, and contributions from the community and are always looking for ways to improve the platform and make it more useful for our users.

Furthermore, we invite users to create and share with us their own workshops, curricula, and institutes. By contributing to the wider curricula available to learners, you can help build a rich and diverse collection of resources that benefit the wider DH community.

On that note, let's move on to the next section, where you will learn how to create and modify DHRIFT sites to host your own workshops and digital research institutes.

# Creating and Modifying DHRIFT Sites

In this section, you will learn how to create and modify DHRIFT sites to host your own workshops and digital research institutes. You will learn how to use the DHRIFT wizard to create a sample institute based on your community’s needs and how to customize your DHRIFT site to display your own branding and content.

Our wizard is meant to be a tool that allows you to create a new DHRIFT site with a few simple steps. You will be able to choose workshops from among our core curriculum, customize your site with your institute name, logo, and more, and generate a new standalone DHRIFT site that you can further customize to suit your preferences. 

Let's get started!

## We're Off to See the Wizard!

Let's use the wizard to create a new DHRIFT site. The wizard is a simple form that will guide you through the process of setting up your site, choosing workshops, and customizing your site's appearance.

### How Does the Wizard Work?

Once you have completed the form and submitted your choices, the wizard will generate a new DHRIFT site for you based on your selections. The site will include the workshops you chose, along with your institute name, logo, and other customizations. It will automatically deploy your site to a new GitHub repository under your username, which you can then further customize and publish.

### Accessing the Wizard

TODO: To access the wizard, you can click on the Create New Institute button in the header menu. This will take you to the wizard page, where you can begin setting up your new DHRIFT site. (?) 

Although the wizard is meant to be fairly self-explanatory, this workshop will walk through the form together to explain each option and how it will affect your site.

## Walking Through the Wizard

Let's walk through the wizard together to create a new DHRIFT site. We'll go step by step through the form, explaining each option and how it will affect your site.


# Creating New DHRIFT Workshops

So far, you have seen how to navigate and interact with existing DHRIFT workshops on the platform, including using the wizard to set up your own DHRIFT site and repository with options from among our core curriculum.

However, DHRIFT is also meant to be a platform for easily creating and publishing your own workshops, so you can better meet the needs of your particular audience or institution. In this section, then, you will learn how to create your own workshops to publish with the DHRIFT platform. You'll learn how to write workshop markdown files, configure workshop metadata using YAML, add images and other assets, and incorporate interactive features like quizzes, challenges, and code editors.

Let's get started!

## Getting Started

To create a new workshop, you will need to follow a few general key steps:

1. Create a new GitHub repository to house your workshops (or use an existing one)
2. Configure your workshop metadata using YAML
3. Write your workshop content in Markdown
4. Add images, downloads (e.g., datasets) and other assets to your workshop, if needed
5. Incorporate interactive features like quizzes, challenges, and code editors, if desired
6. Build and deploy your workshop using GitHub Actions

Depending on what you want to achieve with your workshop, you may need to follow additional steps or best practices. We'll cover these in more detail as we go along.

### Additional Resources

Keep in mind that we have provided a template workshop that you can use as a starting point for creating your own workshops. The template workshop includes examples of how to structure your workshop content, configure your workshop metadata, and incorporate interactive features. You can find the template workshop here:  TODO: link to template workshop, or maybe just a download for the md file?

We also have a detailed style guide on how to write workshops for the DHRIFT platform. While this guide is meant to be a reference for those wishing to publish workshops with the wider DHRIFT community, it can also be useful for those creating their own workshops for personal or professional use. You can access the style guide here: TODO: link to style guide

## Setting up Your Workshop Repository

The first step in creating a new workshop is to set up a GitHub repository to house your workshop content. You can create a new repository from scratch or use an existing repository if you prefer. 

Considering we have already set up a DHRIFT site and repository using the wizard, we can simply use that repository to house our new workshop and subsequently add it to the available workshops on our site.

In general, you should be aware that the DHRIFT platform generates workshops by pointing to a specific repository that contains your workshop files. 

For instance, in the following URL: https://app.dhrift.org/inst/?instUser=dhri-curriculum&instRepo=dhrift-site-template

...the `instUser` parameter specifies the GitHub user or organization that owns the repository, and the `instRepo` parameter specifies the name of the repository. You can use these parameters to point to your own repository and display your workshops on your DHRIFT site. DHRIFT will automatically detect the workshops (markdown files) in your repository and display them on the workshops page.

## Configuring Workshop Metadata

Once you have set up your workshop repository, you will want to create a new markdown file for your workshop. You can name this file anything you like, but it is a good idea to use a descriptive name that reflects the content of your workshop. For example, if you are creating a workshop on Python programming, you might name your file `intro-to-python.md`.

You can create and edit markdown files locally using a text editor like [Visual Studio Code](https://code.visualstudio.com/) or utilize the Jupyter Notebook code editor here in the browser (just save and download your files to your local file system). Make sure to save your file with the `.md` extension. If you are using the built-in code editor, you'll notice that there is a markdown option when creating a new file.

The first thing you will need to do in your workshop markdown file is configure your workshop metadata using [YAML](https://yaml.org/)." In terms of your workshop, the YAML language allows you to specify metadata such as the workshop title, author, description, learning objectives, estimated time, and more.

Here is an example of a simple YAML configuration for an Intro to Python workshop:

```yaml
---
title: Introduction to Python
cover title: Introduction to Python
description: "This workshop is designed for beginners who want to learn the basics of Python programming. By the end of this workshop, you will be able to write simple Python programs, work with variables, and use control structures like loops and conditionals."

programming_language: 'python'

learning objectives:
    - Understand the basic syntax and structure of Python
    - Learn how to work with variables and data types
    - Understand control structures like loops and conditionals

estimated time:
    - 2 hours

authors: 
    - 'Jimmy Pesto'
    - 'Bob Belcher'

facilitators:
    - 'Jimmy Pesto'

ethical considerations:
    - "Learners should be aware of the potential ethical implications of using Python for data analysis and machine learning. For example, it is important to consider issues of bias, privacy, and security when working with data in Python."

---
```

First, you'll notice the three dashes at the beginning and end of the YAML configuration. This is a standard way to indicate the start and end of a YAML document. You will always want to enclose your metadata in these dashes at the start of your markdown file.

The metadata will comprise the information to display on your workshop's front page. Here's a breakdown of the metadata fields shown above:

- `title` specifies the title of the workshop, which will be displayed on the workshop's front page.
- `cover title` specifies the title of the workshop that will be displayed in the image gallery of all workshops. Unless it is a very long title that may not display well in terms of the image, it is often the same as the title.
- `description` provides a brief overview of the workshop content and objectives.
- `programming_language` specifies which code editor to use for the workshop (e.g., Python, Jupyter, JavaScript, R, command line, etc). See below for a list of supported programming languages and the associated metadata field.
- `learning objectives` lists the main learning objectives of the workshop.
- `estimated time` specifies the estimated time needed to complete the workshop.
- `authors` lists the authors of the workshop.
- `facilitators` lists the facilitators, or instructors, of the workshop.

These are, at bare minimum, the fields you will likely want to include in your workshop metadata. However, it should be noted that the only truly required fields are `title`, `cover title`, and `description`. The other fields are optional but highly recommended for providing a complete and informative workshop experience.

You can also add additional metadata fields as needed for your workshop. For example, you might want to include a list of prerequisites, projects, additional resources or tutorials, etc. You can follow the same format as the `ethical considerations` field shown above for these additional fields, e.g.,

```yaml
prerequisites:
    - "No prior programming experience is required."
    - "A basic understanding of computer science concepts is helpful but not necessary."
```

### Supported Programming Languages

You can include the other code editors supported by DHRIFT in the `programming_language` field. Here is a list of supported programming languages and their associated metadata fields:

- Python: `'python'`
- Jupyter Notebooks: `'jupyter'`
- JavaScript: `'javascript'`
- R: `'r'`
- Command Line: `'command_line'`
- HTML and CSS: `'html_css'`

It will be up to you to decide which code editor (if any) is most appropriate for your workshop content.

## Writing Workshop Content

Once you have set up your workshop repository and YAML, you can start writing your workshop content in markdown. Markdown is a lightweight markup language that is fairly straightforward to read and write, once you understand the basic syntax. It allows you to format text, add images, and create links without having to write HTML (although it supports many basic HTML features such as text styling and table creation as well).

DHRIFT uses standard markdown syntax for formatting text, including headings, lists, links, images, and more. You can find a comprehensive guide to standard markdown syntax here: [Markdown Syntax Guide](https://www.markdownguide.org/basic-syntax/).

Beyond that, DHRIFT also includes a few custom markdown extensions that allow you to include interactive features like quizzes, challenges, and code editors in your workshop content. We'll cover these extensions in more detail in the following sections.

### General Structure

A typical DHRIFT workshop is divided into sections and subsections, each with its own content. You will want to separate your content into logical sections that follow the flow you envision for your workshop. For major sections, you can use level 1 markdown headings (`#`), and for subsections, you can use level 2 headings (`##`). For instance, in this workshop, we have used level 1 headings for major over-arching sections like "Introduction to DHRIFT" and level 2 headings for subsections like "What is DHRIFT?", "Underlying Technologies", etc. In general, note that both level 1 and level 2 headings will create a new page. DHRIFT will then automatically generate a table of contents for your workshop based on the headings you use.

For the most part, you can structure your workshop content as you see fit, but it is generally a good idea to follow a pedagogically conscientious progression from introduction to conclusion. Separating out your content effectively can help learners navigate through the material more easily and tackle the lessons in digestible chunks.

Here is an example of how you might structure the beginning of a workshop using markdown headings:

```markdown
# Introduction

This section provides a short introduction to the workshop. 

## Overview

This subsection provides an overview of the workshop and what learners can expect to gain from it.

## Learning Objectives

This subsection lists the main learning objectives of the workshop.

# Getting Started

This creates a new main section for the workshop.

## Setting up Your Environment

This subsection covers how to set up the necessary tools and resources to follow along with the workshop.

### Installing Python

This (sub)subsection provides instructions on how to install Python on your computer.

## Writing Your First Program

This subsection introduces learners to the basics of programming and writing their first program.

### Hello, World!

This (sub)subsection covers how to write a simple "Hello, world!" program in Python.
```

As you can see, we are utilizing level 1 headings for major sections like "Introduction" and "Getting Started" and level 2 headings for subsections like "Overview", "Learning Objectives", "Setting up Your Environment", etc. This structure helps to organize the content and make it easier for learners to follow along. 

Furthermore, we are using level 3 headings for additional (sub)subsections like "Installing Python" and "Hello, World!" to further break down the content. Note that level 3 headings will be displayed _on the same page_ as the level 1 or 2 heading they are nested under, and will not appear in the table of contents. This can be useful for breaking down content into smaller, more manageable sections without cluttering the table of contents or creating new pages.

## Adding Images

In addition to text content, you can also add images to your workshop. Images can help illustrate concepts, provide visual interest, and make your workshop more engaging.

To add an image to your workshop, you can use standard markdown syntax for images. Here is an example:

```markdown
![Alt text](path/to/image.jpg)
```

In this syntax, `Alt text` is the alternative text for the image, which is displayed if the image fails to load (this should also comprise a short description of the image for accessibility purposes). `path/to/image.jpg` is the path to the image file in your repository. Typically, you will want to store your images in a subdirectory of your repository, such as `images/`, to keep your files organized. Even better would be to store the images in a designated folder for the workshop, e.g., `images/your-workshop`. Just make sure your folder title follows the _exact_ name of your workshop so DHRIFT knows where to look for it. You can also use a URL to an external image if needed.

## Code Snippets and Info Boxes

### Code Snippets

DHRIFT workshops may also include inline code snippets to demonstrate programming concepts, provide examples, and guide learners through exercises. You can include code snippets in your workshop using standard markdown syntax for code blocks. 

To create something like the following:

```python
print("Hello, world!")
```

...you can use three backticks ````(```)```` to start and end the code block, followed by the language identifier (e.g., `python`) to specify the language of the code snippet.

In this example, `python` specifies the language of the code snippet, which helps DHRIFT format the code block correctly. You can replace `python` with other supported languages like `javascript`, `html`, `console`, etc., as needed. 

### Info Boxes

To create an info box with additional information or tips that stands out from the rest of your text, like the following...

<Info>
This is an info box with additional information or tips for learners.
</Info>

...you can use the following custom markdown syntax:

```markdown
<Info>
This is an info box with additional information or tips for learners.
</Info>
```

In this example, the `<Info>` tag creates an info box with the enclosed text. This can be useful for highlighting important information, providing additional context, or offering tips and suggestions to learners.

## Incorporating Interactive Features

DHRIFT workshops can include a variety of interactive features to engage learners and reinforce learning. 

### Quizzes

To create a quiz, you can use the following custom markdown syntax:

```markdown
### Evaluation

What front-end technology does DHRIFT use to build its user interfaces?

<Quiz>
- React*
- Angular
- Vue
- Ember
</Quiz>
```

In this example, the (optional heading) `Evaluation` section introduces a multiple-choice quiz question, and the `<Quiz>` tag creates the interactive quiz. Learners can select an answer from the list, and DHRIFT will provide feedback on whether the answer is correct or incorrect. To specify a correct answer (or answers), mark it with an asterisk (`*`).

### Challenges

To create a challenge with a solution that you can show/hide, you can use the following custom markdown syntax:

```markdown
### Challenge

Where are DHRIFT workshops stored?

### Solution

<Secret>
In a GitHub repository.
</Secret>
```

In this example, the (optional heading) `Challenge` section poses a question or problem, and the `<Secret>` tag creates a hidden solution that learners can reveal by clicking a button. This allows learners to attempt the challenge on their own before checking the solution.

## Key Terms

DHRIFT workshops may also include a section of key terms to define and explain unfamiliar concepts. You can include a key terms section in your workshop using the following custom markdown syntax:

```markdown
<Keywords>
- DHRIFT
DHRIFT (Digital Humanities Resource Infrastructure for Teaching Technology) is an open educational resource (OER) and publication platform for DH workshops. Designed by humanities scholars for humanities scholars, DHRIFT provides a minimal computing, accessibility-aware, and interactive environment for teaching fundamental DH concepts.
- Markdown
Each workshop is created using Markdown, a lightweight markup language that is easy to read and write. Markdown allows you to format text, add images, and create links without having to write HTML.
</Keywords>
```

In this example, the `<Keywords>` tag creates a section of key terms, and each term is defined with a bullet point list. This section can help learners understand and remember important concepts from the workshop.

## Adding Your Workshop to Your DHRIFT Site

Once you have reached a point where you are satisfied with your workshop content, you can add your workshop to your DHRIFT site. To do this, you will need to push or upload your workshop markdown file to your GitHub repository. DHRIFT will automatically detect the new workshop file and display it on your site.

To ensure that your workshop is displayed correctly, keep in mind these checks:

- Check that your workshop metadata is correctly configured in the YAML front matter.
- Make sure your workshop markdown files are correctly formatted and free of syntactical errors.
- Prepare all necessary assets (images, downloads, etc.) to be placed in designated folders in your repository.

If everything looks good, there are a few ways you can add your workshop to your repository. If you are familiar with Git and GitHub, you can push your changes directly to your repository using Git commands. 

For instance, you can add your files to the staging area, commit your changes, and push them to your repository using the following commands:

```bash
git add -A
git commit -m "Add new workshop"
git push
```

[VSCode](https://code.visualstudio.com/) also has a built-in Git interface that you can use to stage, commit, and push your changes.

If you are less familiar with Git or are not using VSCode, you can also use the GitHub web interface to upload your files directly to your repository. Simply navigate to your repository on GitHub, click the "Add file" button, and select "Upload files" to add your workshop markdown file. Make sure you are also adding any images or other assets to the correct folders in your repository.

### Reviewing Your Workshop

To see your workshop in action, you can navigate to your DHRIFT site and check the workshops page. Your new workshop should appear in the list of available workshops, and you should be able to click on it to view the workshop content. Make sure your DHRIFT site is pointed to the correct repository and branch where your workshop files are stored (please see the "Setting up Your Workshop Repository" section if you need a refresher on how to point to your repo).

# Forking and Cloning the DHRIFT Platform

The DHRIFT team encourages not only that you create your own workshops but also that you contribute to the wider DHRIFT community by suggesting changes, improvements, and new features to the platform itself. One way to do this is by forking and cloning the DHRIFT platform and modifying it to suit your needs.

In this section, then, you will be shown how to fork and clone the DHRIFT platform for your own uses. You will learn some basics about the DHRIFT platform and repository, fork the repository to create a copy in your GitHub account, and modify the platform in a variety of ways. You will also learn to suggest changes to the DHRIFT platform and contribute to the wider DHRIFT community.

Let's get started!

## Forking vs. Cloning

Before we begin, it is important to understand the difference between forking and cloning a repository, as you will be doing both.

- **Forking**: Forking a repository creates a copy of the repository in your GitHub account, which you can then publish as your own site. Any changes you make to the forked repository will not affect the original repository. Forking is typically used when you want to suggest changes back to the owners of the original repository.

- **Cloning**: Cloning a repository creates a copy of a repository on your local machine, which you can then modify and push back to the cloned repository. Cloning is typically used when you want to work on a project locally and make changes to the source repository.

In other words, forking is used to create a remote copy of a repository on GitHub, while cloning is used to create a copy of a repository on your local machine. In this section, you will be forking the DHRIFT repository to create a copy in your GitHub account and then cloning the forked repository to work on it locally. This process can allow you to submit pull requests to the original DHRIFT repository and potentially contribute changes to its development.

## Forking the Repository

To fork your own copy of the DHRIFT platform, you can follow these steps:

1. Navigate to DHRIFT's current development repository on GitHub: [DHRIFT GitHub](https://github.com/DHRI-Curriculum/DHRIFT)
2. Click the "Fork" button in the top-right corner of the repository page. This will create a copy of the repository in your GitHub account.
3. Navigate to your forked repository on GitHub. You should see a copy of the DHRIFT repository in your account.

Now that you have forked the DHRIFT repository, you can clone it to your local machine and start making changes to the platform.

## Cloning the Repository

As mentioned earlier, cloning a repository creates a copy of the repository on your local machine, which you can then modify and push back to the cloned repository. To clone your forked DHRIFT repository to your machine, you can follow these steps:

1. Copy the URL of your forked repository. You can find the URL by clicking the green "Code" button on your repository page and copying the HTTPS or SSH URL.
2. Open a terminal or command prompt on your local machine.
3. Use the `git clone` command to clone the repository. Replace `URL` with the URL of your forked repository:

```bash
git clone URL
```

4. Change into the cloned repository directory:

```bash
cd DHRIFT
```

Now you have a local copy of the DHRIFT platform on your machine that you can modify and work with.

<Info>
If you are not familiar with Bash or the command line, you can also simply click the "Download ZIP" button on your forked repository page to download a ZIP file of the repository to your local machine. You can then extract the ZIP file and work with the repository in your file explorer.
</Info>

## Modifying the Platform

DHRIFT's platform is built with React, a JavaScript library for building user interfaces. This means that you can modify the appearance and content of your DHRIFT site by editing the React components that make up the site. You can also customize the site by adding new components, changing the HTML/CSS styling, and updating the markdown content.

<Info>
If you are unfamiliar with React, we would recommend starting with the [React documentation](https://react.dev/learn) to get a sense of how React works and how you can use it to build user interfaces.
</Info>

If you take a look at the DHRIFT repository you forked, you will see a number of directories and files that make up the platform. 

### Components

One of the main directories you will likely be working with is `/components`. This directory contains many of the React components that make up the DHRIFT site, including the code editors, the header, footer, and institute schedules, and the workshops. You can modify these components to change the appearance and functionality of the site. For instance, if you inspect the `WorkshopPieces` folder, you will see the custom markdown components that render the workshop content, including custom components like quizzes, challenges, info boxes, and more.

### Styles

The `/styles` directory contains the CSS files that style the DHRIFT platform. You can modify these files to change the appearance of the site, including colors, fonts, spacing, and more. For instance, you might want to update the color scheme of the site to match your institute's branding.


