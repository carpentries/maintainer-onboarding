---
title: "Communicating with Curriculum Advisors"
teaching: 10
exercises: 15
questions:
- "How does my lesson fit into the overall curriculum?"
- "What kinds of changes do I have the authority to make?"
- "Who should I talk to about larger-scale changes?"
objectives:
- "Describe who has authority, and responsibility, to make different types of decisions." 
- "Gain confidence in merging simple PRs independently." 
- "Identify which PRs need review and know how to contact other Maintainers for PRs that need review." 
- "Know when and how to contact Curriculum Advisors."
keypoints:
- ""
---

To include: 
- CAC consultation rubric (undergoing RFC now, add after August 23)
- What is a CAC, what do these groups do, who is on the CAC for my curriculum? 
- When will CACs become active again?
- Communication pathways for contacting appropriate CAC


> ## Exercise
> Match the issue with the correct strategy for resolving it. (Erin find real examples)
> - Needs elevation to CAC
> - Simple fix by a single Maintainer without review
> - Put in a PR and wait for another Maintainer to review
> - Raise the issue for conversation at Maintainer co-working corral or on email list
{: .challenge}


## Types of Changes

A common question from Maintainers is whether they have the authority to implement certain
types of changes and who should be involved in the decision-making process. Roughly
speaking, we can break down types of changes into three main categories:

- **Typos and minor wording changes**
    These can be implemented immediately after review by a single Maintainer.

- **Introduction of new material to a lesson**
    A decision to implement these changes (or not) should be made by at least two members of the Lesson Team. The first
    Maintainer to review the change leaves a comment indicating whether it should be approved (we often use the comment "LGTM"
    (looks good to me) to indicate approval). The second Maintainer to review can either merge (if both have approved the
    changes) or suggest revisions. Or, if they disagree with the spirit of the change, they should leave a comment explaining
    why, and allow some time for the contributor, the first approver, or anyone else to respond before closing the PR.

- **Large-scale changes to the structure of the lesson**
    Examples of this would be changing from base R to tidyverse for teaching R, changing from ggplot to matplotlib for plotting
    in Python, or introduction of new tools like a different variant caller for the Data Carpentry Genomics lesson.
    A decision of this scale
    should involve a broader conversation with the community.

Some lessons have a [Curriculum Advisory Committee](https://docs.carpentries.org/topic_folders/lesson_development/lesson_development_roles.html#curriculum-advisory-committee).
These Committees are responsible for guiding the overall direction
of the curriculum, including any proposed large-scale changes. As of May 2021, the Curriculum Advisory Committees are
on hiatus and are scheduled to be reintroduced in September 2021. While Curriculum Advisors are on hiatus, and for
lessons without a Curriculum Advisory Committee, decisions about large-scale changes to the lessons are made via conversations
in GitHub
repos, on The Carpentries [TopicBox lists](https://carpentries.topicbox.com/), and other communication channels.

> ## Exploring Issues (15-20 min)
> You will be placed in a breakout group with members of your Lesson Team.
> Open the GitHub repo for your lesson and navigate to the `Issues` tab.
>
> **First**, select an issue that has been open for less than 6 months with your group and decide which of the above categories it fits into.
> Add a comment describing your group's suggested action/follow-up on at least one issue.
> Be sure to tag any involved parties.
>
> **Next**, with your breakout group, select one PR or Issue that has been
> open for > 6 months. Read the comments and discuss what the problem
> is (i.e. why hasn't the PR been merged). Draft a response to the
> PR/Issue in the Etherpad. If you're comfortable doing so, add your
> response to the conversation and tag the other Maintainers for the lesson.
{: .challenge}
