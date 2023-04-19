---
title: Infrastructure for Lesson Maintenance
teaching: 10
exercises: 5
---

::::::::::::::::::::::::::::::::::::::: objectives

- Understand the structure of the lesson source repository --- know which elements generate the various parts of the lesson page.
- Navigate to the correct file and element to update each section, including instructor notes, setup, questions, timings, learning objectives, key points, and glossary.
- Be familiar with the various callout boxes used in Carpentries lessons and be able to use them appropriately.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What should I know about how the lessons are formatted?

::::::::::::::::::::::::::::::::::::::::::::::::::


## Lesson Infrastructure Transition

This is an exciting time for The Carpentries Lesson Infrastructure! We are in the midst of the 
official transition to a new infrastructure - [The Carpentries
Workbench](https://carpentries.github.io/workbench), which is designed to be more user friendly for
both contributors and Maintainers. All lessons will transition to using the Workbench in 
May 2023. This episode will teach you some of the most important elements of the Workbench that you will need
to interact with as a Maintainer. Full documentation can be found on 
[Introduction to The Carpentries Workbench](https://carpentries.github.io/sandpaper-docs/).

:::::::::::::::::::::::::::::::::::::::::  callout

## Important: Resolve All Open Pull Requests

In order to prepare lessons for The Workbench transtion, **all open pull requests must be merged or closed by 1 May**. 
The Carpentries Curriculum Team will be assisting
Maintainers across all of our lessons to ensure pull requests are resolved before the deadline. 

::::::::::::::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::::::::::::::::::::::  callout

## What Was "Styles"?

You may come across references to something called "Styles". Styles is the name for 
the infrastructure that was used for The Carpentries lessons from 2014 - May 2023. This 
infrastructure was managed through the [styles
repository](https://github.com/swcarpentry/styles), and documented on
the [lesson-example repository](https://carpentries.github.io/lesson-example/).

::::::::::::::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::::::::::::::::::::::  callout

## Who Maintains the Lesson Infrastructure?

Up until March 2020, the lesson infrastructure was maintained by the
[Lesson Infrastructure Committee](https://carpentries.org/lesson-infra/). The
activity of the Committee was put on hold during the COVID-19 pandemic and we are making concious
strategic decisions about how to re-form this committee ahead of May 2023.

The Lesson Infrastructure is currently maintained by the [Curriculum
Team](https://carpentries.org/core-team-projects/#curriculum-team), with the help of [Maxim
Belkin](https://github.com/maxim-belkin).


::::::::::::::::::::::::::::::::::::::::::::::::::

## Lesson configuration

The global configuration of the lesson - 
settings that affect the lesson as a whole, 
such as its title, 
the ["lesson life cycle" stage](https://cdh.carpentries.org/the-lesson-life-cycle.html) that may be displayed in the banner at the top of its pages,
and the contact information and source repository URL linked in its page footers -
are stored in the `config.yaml` file.
This file is in [YAML format](https://learnxinyminutes.com/docs/yaml/), containing configuration parameters as key-value pairs. 
Lesson Maintainers should only need to modify this file very rarely.

## Lesson homepage

The lesson homepage provides an overview of the lesson,
including any prerequisites, an introduction to the dataset used, and any other information learners will need for the lesson.
This content is built from the `index.md` file in the root folder of the lesson repository.

The Instructor view of the lesson homepage also includes a schedule showing the individual episodes included in the lesson,
and the time allotted for each. The schedule is automatically created based on information present in
the episode files.

The Learner view of the homepage includes the setup instructions for the lesson:
information about the software to install and data to download in order to be ready to follow the lesson.
This content is built from the `setup.md` file in the `learners/` folder of the lesson repository (more details later).

## Episodes

The majority of a lessons content is in its episode files. Episode files are stored in the
`episodes/` folder within your lesson repository.
Episode files are written in *Markdown* or *RMarkdown*. The essential elements of an episode
are mentioned below. For complete information about how to construct each element
of an episode file, please see [the documentation](https://carpentries.github.io/sandpaper-docs/episodes.html). 

### Episode headers

Each episode starts with a YAML header that looks like this:

```
---
title: "What is the shell?"
teaching: 5
exercises: 0
---
```

`title` sets the title of the episode, which will be displayed as a top-level heading on the webpage. `teaching` and `exercises` are values (in minutes) indicating how much time the episode is estimated to take to teach, and for learners to complete its exercises. The information stored in the YAML header is used by the lesson infrastructure to populate the schedule.


## Fenced Divs

As well as general explanatory content, episodes usually contain a number of blocks of particular types, such as Instructor notes, a list of key points, and exercises and solutions. These blocks of content are formatted to stand out from the other content on the page, and in some cases are treated differently by the lesson infrastructure (e.g. Instructor notes are hidden in the Learner View of the lesson).

These formatted blocks of content are added to episodes (and other pages in the lesson site) as _fenced divs_: chunks of content delineated ("fenced") by lines of colon `:` symbols, with the opening fence accompanied by a tag that defines the class of fenced div being created. 

For example, a fenced div belonging to the `callout` class - used to highlight a particular block of content - can be defined with:

```
::::::::::::::::::::::::::::::::::::::: callout

Some text here.

:::::::::::::::::::::::::::::::::::::::
```

::::::::::::::::::::::::::::::::::::::: callout

Some text here.

:::::::::::::::::::::::::::::::::::::::

### Questions, objectives, and keypoints

Every episode must contain one of each of the following types of fenced div: 

- Questions: Located at the top of the episode file, these are plain language questions that show learners what to expect to gain from the episode. Fenced div class: `questions`.
- Objectives: Located at the top of the episode file, objectives are specific goals that learners should be able to accomplish by the end of the episode. Fenced div class: `objectives`.
- Keypoints: Located at the end of the episode file, key points are statements of the major take-aways learners should remember from each episode. Fenced div class: `keypoints`.

Keypoints are automatically gathered from each episode and collected on the "Key Points" page of each lesson. Questions and Objectives are represented
in an "Overview" box at the top of each rendered episode page.

### Other Fenced Divs

In addition to the `callout` class shown above, 
the infrastructure supports several other classes of fenced div that,
although not essential, are often included in episodes.

Fenced divs with the tag "challenge" will render as exercises:

```
::::::::::::::::::::::::::::::::::::::: challenge

This is a challenge.

:::::::::::::::::::::::::::::::::::::::

```

::::::::::::::::::::::::::::::::::::::: challenge

This is a challenge.

:::::::::::::::::::::::::::::::::::::::

Another block with the tag "solution" can be nested inside a challenge to provide the solution to an exercise:

```
::::::::::::::::::::::::::::::::::::::: challenge

What is the solution to this exercise?

::::::::::::::::::::::::::::::::::::::::::::: solution

This is the solution to this exercise.

::::::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::

```

::::::::::::::::::::::::::::::::::::::: challenge

What is the solution to this exercise?

::::::::::::::::::::::::::::::::::::::::::::: solution

This is the solution to this exercise.

::::::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::


Callouts with the tag "instructor" will render as Instructor notes, and will only show up on the Instructor view for the lesson. 

```
::::::::::::::::::::::::::::::::::::::: instructor

This is an Instructor note.

:::::::::::::::::::::::::::::::::::::::

```

::::::::::::::::::::::::::::::::::::::: instructor

This is an Instructor note.

:::::::::::::::::::::::::::::::::::::::

In addition to showing up in-line in the Instructor view, callouts with the "instructor" tag are gathered to a separate "Instructor Notes" page. 


:::::::::::::::::::::::::::::::::::::::  challenge

## Scavenger Hunt (5 minutes)

Identify the file and lines of the file that control the following output for The Carpentries 
[Instructor Training lesson](https://carpentries.github.io/instructor-training/).
Add the file name and copy the relevant lines to the Etherpad.

- Questions (for episode 1)
- Timings (for episode 1)
- Objectives (for episode 1)
- Key points (for episode 1)
- Instructor notes (for all episodes)
- Setup instructions
- Glossary
  

::::::::::::::::::::::::::::::::::::::::::::::::::

## Other repository contents

Most lesson content is stored in `index.md` and the files within the `episodes/` folder,
but the lesson repository also contains source files in other folders:

- the `instructors/` and `learners/` folders contain more Markdown and/or R Markdown files that will be presented as accompanying pages in the Instructor and Learner views of the lesson, respectively.
  - For example, the `instructors/` folder contains the source file for the Instructor Notes page, which - in addition to collating the inline Instructor Notes inlcuded in the episodes of a lesson - can contain general guidance for Instructors.
  - The `learners/` folder contains `setup.md`, the source file for the setup instructions that will appear on the landing page of the lesson in the Learner view.
- the `profiles/` folder contains a source file that can be used to provide learner profiles for the lesson: a way to describe its target audience.
- the `site/` folder exists to store the built version of the lesson site, and should not be modified directly.
- the `.github/` folder contains the GitHub Actions workflows that tell GitHub's systems how to build the lesson site from the source files in the `main` branch of the repository. These workflows will be regularly updated by automated pull requests, and **Maintainers should not modify the contents of this folder directly**.

::::::::::::::::::::::::::::::::::::::::::::::::: callout

## For R Markdown Lessons Only

Lesson repositories set up to build from R Markdown source files also contain 
the `.Rbuildignore` file and `renv/` folder.
These provide the configuration required for the interpretation and conversion of R Markdown source files in the lesson repository.

:::::::::::::::::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::::::::::::::: callout

## Non-source files

The other repository contents not covered elsewhere in this episode are:

- `.editorconfig` and `.gitignore` are files that help people work with lesson repositories on their local system.
- other files with upper-case names (`AUTHORS`, `LICENSE.md`, etc) are "repository-internal" files i.e. they are most relevant to the lesson as an open source repository, rather than as a website. 

Although these repository files may be occasionally updated, Maintainers can mostly ignore them and focus on the source files for the lesson itself.

:::::::::::::::::::::::::::::::::::::::::::::::::

### Full Infrastructure Documentation

For a step-by-step guide to how the lessons are structured, and what syntax to use to add code
chunks, exercises, and other elements, please read the
[Introduction to The Carpentries Workbench](https://carpentries.github.io/sandpaper-docs/).

:::::::::::::::::::::::::::::::::::::::: keypoints

- The Carpentries lessons share a consistent style, which is controlled by [The Carpentries Workbench](https://carpentries.github.io/workbench) and documented in the [Introduction to The Carpentries Workbench](https://carpentries.github.io/sandpaper-docs/).

::::::::::::::::::::::::::::::::::::::::::::::::::


