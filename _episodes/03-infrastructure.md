---
title: "Infrastructure for Lesson Maintenance"
teaching: 30
exercises: 25
questions:
- "How will I interact with my fellow Maintainers?"
- "What is the overall curriculum development process and what is my role in it?"
- "What is the overall lesson release process and what is my role in it?"
- "How does my lesson fit into the overall curriculum?"
- "What kinds of changes do I have the authority to make?"
- "Who should I talk to about bigger-scale changes?"
- "What should I know about how the lessons are formatted?"
- "How do I preview changes?"
- "What terminology is used to describe the lessons?"
- "What files are involved in the lesson and what do they do?"
- "How are the lesson styles maintained?"
objectives:
- "Become comfortable rendering local previews of Carpentry lessons."
- "Describe the relationship between your lesson and the styles repository."
- "Describe how the lesson release process works for your lesson."
- "Identify interdependencies between your lesson and other lessons it will be taught with."
- "Identify types of changes that you can implement alone, in collaboration with your Lesson Team, and after consultation with other community members."
- "Determine how you and your co-Maintainers will communicate and how you will divide responsibilities for your lesson."
- "If a Curriculum Advisory Committee exists for your lesson, describe their responsibilities and how to contact them."
keypoints:
- "First key point."
---

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

## Curriculum Development Process

The Carpentry community is still developing and testing our process
for development of new lessons. Your involvement with this process
(and making modifications to this process) will depend on the lesson
you are a Maintainer for. Some lessons have been around for a while
and are quite mature and stable, while others are newer and are still in
active development. You can check the status of our lesson rosters on
[Software-Carpentry.org/lessons](https://software-carpentry.org/lessons/),  
[DataCarpentry.org/lessons](https://datacarpentry.org/lessons/) and
[LibraryCarpentry.org/lessons](https://librarycarpentry.org/lessons/).

If your lesson is in active development, you can expect to see a lot
of changes to your repo in the near future. Data Carpentry holds an
Issue Bonanza, followed by a Bug BBQ, for each of the lessons in
active development, to prepare those lessons for publication.

| Lesson Development Stage | Description |
| ---  | --- |
| Preparation | Maintainers and staff make organizational changes to prepare for community contributions. This can include bringing in a new template, changing lesson or episode order, fixing broken formatting, and ensuring data accessibility. The purpose of this stage is to ensure that contributors aren't hindered by bad organization or formatting. |
| Issue Bonanza | Community members are invited to submit issues for problems they see in the materials. Issues can range from typos or broken links to larger content-related problems.|
| Interim | Between the Issue Bonanza and Bug BBQ, Maintainers and staff go through existing issues, organizing and consolidating contributions. The purpose of this stage is to organize the community contributions so that the follow-up for each issue is clear and there aren't duplicated or contradicting issues. |
| Bug BBQ | Community members are invited to submit PRs to fix problems that were identified during the Issue Bonanza (or new issues that they identified).|
| Clean-up | Immediately after the Bug BBQ, Maintainers and staff finish merging PRs, submit PRs for any unresolved issues, and go through the [lesson release checklist]() to ensure that everything is ready for publication.|
| Publication | Staff submit the repository files to Zenodo and generate a DOI for the lesson release. |

The timeline for each of these stages differs between different lessons, as this is still a work in progress. Although not all
Maintainers are expected to be involved with the full process, it
is important to have at least one Maintainer from each Lesson Team
involved in each stage to make sure the process runs smoothly.

## Lesson Release Process
If your lesson is in a mature state, your level of involvement in the
lesson development process will be less intense than that described
above. The mature SWC and DC lessons go through a new lesson release
every six months. At this point, the lessons go through clean-up
(including resolving old issues and PRs) and are submitted to Zotero
to create a new DOI for that version.

[FIXME: ask Raniere for some text here about what Maintainers do during lesson release.]

## Interconnectedness

Even our "mature" and "stable" lessons are continuously changing.
Although the types of changes that these lessons undergo are more
minor than the types of changes that happen in a lesson under
active development, it's important to keep in mind that even minor
changes can have larger impacts. A change in one episode of a lesson
can affect later episodes in that lesson, for example by removing an
example that introduces a concept that is needed later in the lesson.
A change in your lesson can also impact later lessons in your
curriculum. It's a good idea to be familiar with all of the lessons
in your curriculum, so that you know what concepts learners are
coming into contact with in the lessons before yours and what
concepts your lesson is their first exposure to (a later lesson may
be depending on you to introduce that concept).

This interconnectedness is sometimes more obvious in the Data Carpentry
lessons, where all of the lessons deal with a single dataset, but it is also
a feature of some of the Software Carpentry lessons. For example, the
[Version Control with Git](http://swcarpentry.github.io/git-novice/) lesson
is taught on the command line. It depends on the [Unix Shell](http://swcarpentry.github.io/shell-novice/) lesson to introduce concepts like
hierarchical directory structure, flags/options, file manipulation with nano, and
specific Bash commands like `ls`, `cat`, `cd` and others.

> ## Identify Your Interconnections (15 min)
> You will be placed in a breakout group with members of your Curricular Team.
> Spend about XX minutes identifying concepts, terms, and commands that are
> introduced in one lesson and used in later lessons. Make a list of the ways
> in which your lessons are interconnected in the Etherpad.
{: .challenge}

> ## Exercise
> With another member of your Lesson Team, look through the files
> in your lesson's GitHub repo. Identify at least one point where
> formatting does not match that specified in the [Lesson Example](http://swcarpentry.github.io/lesson-example/)
> and put in a PR to correct the formatting.
> > ## Hint
> > Common issues include syntax highlighting,
> > failing to include time estimates for exercises, and keyboard key
> > styling.
> {: .solution}
{: .challenge}

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

The template for Carpentry lessons is managed through the [styles repository](https://github.com/swcarpentry/styles), which is
maintained by [Raniere Silva](https://github.com/rgaiacs) in
coordination with the Lesson Infrastructure Subcommittee. If you
are interested in being involved, please contact Raniere.

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

The overall Maintainer team communicates via our [mailing list](https://carpentries.topicbox.com/groups/maintainers).
Please make sure you are signed up, as this is the primary
communication channel for all Maintainer-related information. We also
have monthly meetings to discuss topics relevant to the
Maintainer community. You can find the times for these meetings
on the
[community calendar](https://carpentries.org/community/#community-events)
and on the [Maintainer Etherpad](http://pad.software-carpentry.org/maintainers).

It is important to stay in touch with your Lesson Team.
All Lesson Teams work
differently, and you will need to find a communication style and
distribution of work that works for you. We recommend that, at
a minimum, your team meets by video-conference once a quarter to
set priorities and deal with existing concerns.

There are several decisions that your Lesson Team will need to make
about how you will work together. Here are some issues you should
consider:

* Who will be responsible for what?
* How often will we each work on the lesson?
* What are our expectations for our repo in terms of response time,
turn-around time, issue tagging, etc.

> ## Make a List (10 min)
> With your break-out group, discuss the points above and
> add to this list. What are other things that you want to
> communicate about with your Lesson Team?
{: .challenge}

> ## Follow-up Homework
> Get in touch with your Lesson Team to schedule an initial
> meeting. At this meeting, be sure to discuss the issues in the list
> generated above. Communicating by email can also help to set the
> stage for your initial meeting and clarify any of these items
> after the meeting.
{: .challenge}


> ## Minute Cards (5 min)
> Have Maintainer Onboarding participants fill out Minute Cards to gain feedback on the session.
{: .challenge}
