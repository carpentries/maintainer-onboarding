---
title: Infrastructure for Lesson Maintenance
teaching: 30
exercises: 30
---

## Maintainers and Forked Repositories

::::::::::::::::::::::::::::::::::::::: objectives

- Understand the structure of the lesson source repository---know which elements generate the various parts of the lesson page.
- Navigate to the correct file and element to update each section---including instructor notes, setup, questions, timings, learning objectives, key points, and glossary.
- Be familiar with the various callout boxes used in Carpentries lessons and be able to use them appropriately.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What should I know about how the lessons are formatted?

::::::::::::::::::::::::::::::::::::::::::::::::::


## The Carpentries Lesson Infrastructure

This is an exciting time for The Carpentries Lesson Infrastructure! We are in the midst of the 
official transition to a new infrastrucutre - [The Carpentries
Workbench](https://carpentries.github.io/workbench), which is designed to be more user friendly for
both contributors and Maintainers. All lessons will transition to using the workbench in 
May 2023. This section will teach you some of the most important elements of The Workbench that you will need
to interact with as a Maintainer. Full documentation can be found on [The Carpentries Workbench](https://carpentries.github.io/workbench/).

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

### Lesson homepage

The lesson homepage is built from the `index.md` file and provides an overview of the lesson,
including any prerequisites, an introduction to the dataset used, and any other information learners will need for the lesson.

The Instructor view of the lesson homepage also includes a schedule showing the individual episodes included in the lesson,
and the time allotted for each. The schedule is automatically created based on information present in
the episode files.

### Episodes

The majority of a lessons content is in its episode files. Episode files are stored in the
`_episodes/` folder within your lesson repo (or in `_episodes_rmd/` for lessons written in R).
Episode file names must start with a two-digit identifier number (e.g. `01`) followed by a short
descriptive name, separated by a dash (`-`). For example `02-loop.md`, `03-lists.md`. The numeric
identifier is used to place your episode files in the correct sequence within the lesson. Episode
files are written in *Markdown* or *RMarkdown*.

#### Episode headers

Each episode starts with a YAML header that looks something like this:

```
---
title: "What is the shell?"
teaching: 5
exercises: 0
---
```

The information stored in the YAML header is used by the lesson infrastructure to populate the schedule.

#### Questions, objectives, and keypoints

Each episode must contain one each of the following types of callouts: 

- Questions: Located at the top of the episode file, these are plain language questions that show learners what to expect to gain from the episode.
- Objectives: Located at the top of the episode file, objectives are specific goals that learners should be able to accomplish by the end of the episode.
- Keypoints: Located at the end of the episode file, key points are statements of the major take-aways learners should remember from each episode. 

Keypoints are automatically gathered from each episode and collected on the "Key Points" page of each lesson. Questions and Objectives are represented
in an "Overview" box at the top of each rendered episode page.

#### Instructor notes



:::::::::::::::::::::::::::::::::::::::  challenge

## Scavenger Hunt (5 minutes)

Identify the file and lines of the file that control the following output for The Carpentries 
[Instructor Training lesson](https://carpentries.github.io/instructor-training/).
Add the file name and copy the relevant lines to the Etherpad.

- Questions (for episode 1)
- Timings (for episode 1)
- Objectives (for episode 1)
- Key points (for episode 1)
- Instructor notes
- Setup instructions
- Glossary
  

::::::::::::::::::::::::::::::::::::::::::::::::::

For a step-by-step guide to how the lessons are structured, and what syntax to use to add code
chunks, exercises, and other elements, please read the [technological introductions
chapter](https://cdh.carpentries.org/technological-introductions.html) of The Carpentries Curriculum
Development Handbook.

:::::::::::::::::::::::::::::::::::::::: keypoints

- Make a branch to create a pull request.
- The Carpentries lessons share a consistent style, which is controlled by [styles](https://github.com/carpentries/styles) and documented in the [lesson-example](https://carpentries.github.io/lesson-example/)

::::::::::::::::::::::::::::::::::::::::::::::::::


