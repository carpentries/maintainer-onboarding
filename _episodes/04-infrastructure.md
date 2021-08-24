---
title: "Infrastructure for Lesson Maintenance"
teaching: 30
exercises: 25
questions:
- "What files are involved in the lesson and what do they do?"
- "How are the lesson styles maintained?"
- "What should I know about how the lessons are formatted?"
- "How do I preview changes?"
objectives:
- "Understand the structure of the lesson template - know which elements generate the various parts of the lesson page." 
- "Navigate to the correct file and element to update each section - including instructor notes, setup, questions, timings, learning objectives, key points, and glossary."
- "Be familiar with the various callout boxes uses in The Carpentries lesson template and be able to use them appropriately." 
- "Locally preview your lesson to test changes."
keypoints:
- ""
---

How to handle images - where to put the files and how to link to them.
Locally preview your lesson to test changes. 
Make in-line comments and suggestions on a PR. Accept suggestions and commit directly to the PR. 
Use appropriate tags on issues. 
Monitor and keep up to date the help-wanted list.
Be aware that the lesson template is nearing a new release. Decide whether you want to be involved in beta testing or wait for official release. 

Rubric for when to use the help-wanted tag. 
Information on other common issue tags.
Different callout boxes used in our lessons and when to use them. 

> ## Exercise
> Review items marked help-wanted on your repository. Remove the tag where it is no longer relevant. Add the tag to things where it is relevant. 
{: .challenge}


> ## Exercise
> Identify the file and lines of the file that control the following output for your lesson. Add the file name and copy the relevant lines 
> (or just add line numbers?) to the Etherpad. 
> - Instructor notes
> - Setup instructions
> - Questions
> - Timings
> - Learning objectives
> - Key points 
> - Glossary
{: .challenge}

Edit nested challenge blocks / solutions. 
Write a challenge block with solution and proper code formatting. 






> ## Preparatory Homework
> Please read the [Lesson Example](http://swcarpentry.github.io/lesson-example/) before our meeting this week.
> The Lesson Example includes information about all the formatting
> you are likely to see in your lesson, as well as instructions
> on how to locally render changes. If you are not maintaining an
> R lesson, you can skip the episode on `Using RMarkdown`. Please
> come prepared to discuss any questions you have about formatting.
{: .prereq}

> ## Preparatory Homework (optional)
> Follow the [instructions for installing Jekyll](https://carpentries.github.io/lesson-example/setup#jekyll-setup-for-lesson-development) and its dependencies.
> Then clone a copy of your lesson repository to your local computer. For example:
>
> ~~~
> $ git clone https://github.com/carpentries/maintainer-onboarding.git
> ~~~
> {: .language-bash}
>
> Navigate to your cloned copy of the repository and preview it
> locally using:
>
> ~~~
> $ make serve
> ~~~
> {: .language-bash}
>
> You should see output that ends with something like:
>
> ~~~
> Server address: http://127.0.0.1:4000
> Server running... press ctrl-c to stop.
> ~~~
> {: .output}
>
> Enter the server address into your web browser to see your local
> website.
>
> If this doesn't work for you, don't worry! We're going to be
> troubleshooting together in breakout groups.
{: .prereq}


## Previewing Changes and Rendering locally

Even for small changes, it is always a good idea to preview changes
to make sure that everything is formatted correctly. There are
(at least) two different ways to do this.

If you are making changes to a single file, you can use
the `Preview changes` tab at the top of the GitHub file editor. This
will show you a simplified version of how GitHub is parsing the
Markdown file. This is useful for checking to see if line breaks are
in the right places, if lists are rendering correctly, and
to make sure that the figures are displaying. However, since this
will not show you the fully rendered webpage for the lesson, it is
not sufficient for checking that blockquotes and code blocks are
rendering properly.

For more complex changes (or changes to multiple files), the safer
option is to make the changes locally, render the full webpage, and then
push those changes back up to GitHub. This requires Jekyll to be
installed and for you to have a local clone of the repository you
are modifying.

> ## Exercise
> In breakout groups, make sure everyone has a local rendering of the
> repo working. Troubleshoot together. Once everyone has a local
> rendering, have one person screenshare, make a change to one of the
> repository files, and visually confirm that the change has occurred
> in the locally rendered webpage. Continue until everyone has
> screenshared.
{: .challenge}

## Style Maintenance

The template for Carpentries lessons is managed through the [styles
repository](https://github.com/swcarpentry/styles), which is maintained by the
[Lesson Infrastructure Committee](https://carpentries.org/lesson-infra/). The
activity of the Committee was put on hold during the COVID-19 pandemic but is
set to resume in the second half of 2021. In the meantime, the [Curriculum
Team](https://carpentries.org/core-team-projects/#curriculum-team), with the
help of [Maxim Belkin](https://github.com/maxim-belkin), has been maintaining
this repository.

## Interacting with Your Fellow Maintainers

As a Maintainer, you will be part of an overlapping set of teams.
From smallest to largest, these include:

* **Your Lesson Team** - the Maintainers who work with you on your lesson (a single GitHub repository).
* **Your Curricular Team** - Maintainers who work on your lesson and other lessons taught in the same workshop.
* **Your Technology Team** - Maintainers who work on other lessons that teach the same tool.
* **The full Maintainer Team** - all Carpentry Maintainers.

> ## Find Your Technology Team!
>
> For our exercises today, we will be working with your Technology
> Team. In the Etherpad, next to your name, write the name of your
> lesson (including whether it is a DC or SWC lesson). Identify your
> group number and put it next to your name:
>
> 1) R Maintainers
> 2) Python Maintainers
> 3) SQL Maintainers
> 4) Unix / Git / and other Maintainers
{: .challenge}

