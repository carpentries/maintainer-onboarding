---
title: "Curricular Aspects of Lesson Maintenance"
teaching: 20
exercises: 35
questions:
- "What is the overall curriculum development process and what is my role in it?"
- "What is the overall lesson release process and what is my role in it?"
- "How does my lesson fit into the overall curriculum?"
- "What kinds of changes do I have the authority to make?"
- "Who should I talk to about bigger-scale changes?"
objectives:
- "Describe how the lesson release process works for your lesson."
- "Identify interdependencies between your lesson and other lessons it will be taught with."
- "Identify types of changes that you can implement alone, in collaboration with your Lesson Team, and after consultation with other community members."
- "If a Curriculum Advisory Committee exists for your lesson, describe their responsibilities and how to contact them."
keypoints:
- "First key point."
---

Some introductory text.

## Curriculum Development Process

The Carpentry community is still developing and testing our process
for development of new lessons. Your involvement with this process
(and making modifications to this process) will depend on the lesson
you are a Maintainer for. Some lessons have been around for a while
and are quite mature and stable, while others are newer and are still in
active development. As of December 2017, the status of each of the
Software and Data Carpentry lessons is:

| Lesson  | Status |
| --------------- | ------ |
| all SWC lessons | mature |
| DC Ecology lessons | mature |
| DC Genomics R | in active development |
| all other DC Genomics lessons | mature |
| DC Geospatial lessons | in active development |
| DC Social Sciences lessons | in active development |

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
| Publication | Staff submit the repository files to Zotero and generate a DOI for the lesson release. |

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

## Types of Changes

A common question from Maintainers is whether they have the authority to implement certain
types of changes and who should be involved in the decision-making process. Roughly
speaking, we can break down types of changes into three main categories:

- **Typos and minor wording changes**
    These can be implemented immediately after review by a single Maintainer.

- **Introduction of new material to a lesson**
    A decision to implement these changes (or not) should be made by at least two members of the Lesson Team. The first Maintainer to review the change leaves a comment indicating whether it should be approved (we often use the comment "LGTM" (looks good to me) to indicate approval). The second Maintainer to review can either merge (if both have approved the changes) or suggest revisions. Or, if they disagree with the spirit of the change, they should leave a comment explaining why, and allow some time for the contributor, the first approver, or anyone else to respond before closing the PR.

- **Large-scale changes to the structure of the lesson**
    Examples of this would be changing from base R to tidyverse for teaching R, changing from ggplot to matplotlib for plotting in Python, or introduction of new tools like a different variant caller for the Genomics lesson. A decision of this scale should involve a broader conversation with the community.

Some Data Carpentry curricula (Genomics, Social Sciences, and Geospatial) have a Curriculum
Advisory Committee. These Committees meet every six months to discuss the overall direction
of the curriculum, including any proposed large-scale changes.

Software Carpentry lessons do not have this Curriculum Advisory Committee structure.
Decisions about large-scale changes to the lessons are made via conversations in GitHub
repos, the [Discuss list-serv](http://lists.software-carpentry.org/listinfo/discuss), and other communication channels. This process may be
changing in the future with the restructuring of the Carpentries.

> ## Exploring Issues (20 min)
> You will be placed in a breakout group with members of your Lesson Team. Open the GitHub
> repo for your lesson and navigate to the `Issues` tab. Starting with the oldest issue
> that is less than 6 months old, discuss each issue with your group and decide which of
> the above categories it fits into. Add a comment describing your group's suggested
> action/follow-up on the issue. Be sure to tag any involved parties. It's ok if you
> don't get through all of your group's issues! Some lessons have a lot of issues.
{: .challenge}

Some group discussion to end.






