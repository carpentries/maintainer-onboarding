---
title: "Communicating with Contributors"
teaching: 15
exercises: 15
questions:
- "What types of contributions am I likely to encounter and how should I handle them?"
- "How do I make sure contributors feel valued, even if their contribution is not accepted?"
- "How can I direct contributors' energy to where it would be most useful?"
objectives:
- "Use The Carpentries Core Values to guide your interactions with contributors."
- "Gain confidence identifying and politely declining out-of-scope contributions."
- "Develop strategies to avoid demotivating contributors."
keypoints:
- "Valuing all contributions is one of The Carpentries Core Values."
- "Not all contributions can, or should, be accepted."
---

## Interacting with Contributors

Maintainers represent The Carpentries on some of our most
active online spaces - our GitHub repositories. As a Maintainer,
you will often be the first point of contact for people new to The
Carpentries community.

Igor Steinmacher, a computer scientist who researches
retention of open source contributors, provides [a set of
recommendations](http://wsl.softwarelivre.org/2015/0002/fostering-freelibre-open-source-software-community-formation:-guidelines-for-communities-to-support-newcomers-onboarding-wsl-2015.pdf) based on his research on how to reduce barriers to
new contributors becoming part of your community. While some of these
are more specific to software projects, some are very applicable to
our (or any) community:

* Answer quickly
* Be kind and make newcomers feel part of the team
* Set expectations and needs early
* Point newcomers to easy tasks
* Keep the issue list clean and triaged
* Dismiss or identify outdated information
* Create a live FAQ section

> ## How Are We Doing?
> How do you feel the Carpentry community does overall in meeting these recommendations? Are there particular areas of strength
> or places where there is room for improvement?
{: .challenge}

## Where do Contributions Come From? 

While anyone can contribute to The Carpentries lessons, the  vast majority of contributions come from:

- Trainees who have gone through Instructor Training and are submitting a contribution as part of "checkout" to complete their Instructor certification. 
- Workshop Instructors (and helpers) who have recently participated in a workshop and noticed difficulties with the materials. 

Everyone who goes through The Carpentries Instructor Training program is required to contribute to a Carpentries lesson
(or other resource) in order to become certified. We train over a thousand people each year to be Instructors, about half of whom complete the
certification process. A large proportion of the contributions you will receive come from Instructor trainees. 

During Instructor Training, we [strongly encourage contributors](https://carpentries.github.io/instructor-training/20-checkout/) to contribute to
discussion on existing PRs and issues, to submit a PR to resolve an
issue that the Maintainers have marked "help-wanted", or to submit issues describing bugs or difficulties in teaching the lesson. 

Despite our best efforts in encouraging these types of contributions, you will also receive unwanted or unhelpful contribtions, including:
- addition of new material covering topics outside of the scope of the lesson
- changes to the way a topic is presented that are inconsistent with The Carpentries pedagogical model
- other examples?

These contributions may come in the form of an issue or a PR. It is important to recognize the effort of contributors, and be respectful, even if their contribution will not be merged. 

Many of the contributions you will receive are from Intructor trainees. Others will be from Instructors who are 
preparing to teach or have recently taught a workshop and noticed things that didn’t work as well as expected. 

It is OK (and more than OK) to directly edit a contributor’s PR if there are minor issues preventing it from being accepted. 
Many of our contributors are non-responsive to requests to update a PR. This is OK. If the contribution is important - make the minor changes 
and merge. If it is not helpful - leave a short and polite explanation of why it won’t be accepted and either ask for edits or close. 

Do not summarily close an issue or PR without commenting. Especially if the contributor is actively engaged and appears to be acting in good faith, 
do not close the issue/PR. This can be very discouraging. 
Ok to close if an issue has gone stale (define?) or if the issue or PR is out of scope (after explaining it is out of scope). 




> ## Discussion (10 min)
> In breakout groups, discuss any of the following questions based on your pre-readings. Please make sure you are taking notes in the Etherpad:
> * How can you balance saying no and being inclusive? What practices can help with this?
> * How might the factors discussed in the Motivation and Demotivation episode of Instructor Training influence the way we interact with contributors?
> * How might the contributing guidelines influence how a contributor contributes to your lesson? How can you use them effectively as a Maintainer?
> * How might you implement the suggestions in “Learning to Say No” as a Maintainer?
> This discussion should take around 10 minutes.
>
> > ## Solution
> > * Teach Most Useful First - we can (and should) politely turn down contributions that take the material out of the scope of the novice learner or that involve unnecessary and distracting technical detail.
> > * Actual Time - everything will probably take longer for learners than it does for you. Limit new additions to the materials and encourage cutting material where needed.
> > * Things You Shouldn't Do in a Workshop - these are also things we shouldn't do in a PR or Issue conversation.
> > * Imposter Syndrome - be encouraging to new contributors, even if they make a formatting mistake.
> > * Accessibility - take seriously any comments a contributor makes about accessibility issues.
> > * Inclusivity - avoid unnecessary use of gendered pronouns and other exclusive language.
> {: .solution}
{: .challenge}

> ## Checkout Contributions by Email
>
> The Carpentries Lesson Programs have expanded to include
> curricula that do not teach Git and GitHub,
> and our [checkout process for new Instructors](https://carpentries.github.io/instructor-training/checkout/index.html#part-1-submit-a-small-contribution-to-a-lesson-or-glossary)
> has changed to acknowledge this.
> We allow trainees to submit feedback and suggested changes
> to Library and Data Carpentry lessons via email,
> as one part of their checkout.
> These emails are handled by a member of the Core Team,
> who will then open an Issue on the lesson repository
> on behalf of the trainee.
> The Core Team will not be able to follow up on these Issues,
> e.g. by opening a Pull Request
> or replying to the thread with more information.
> All such Issues will include a brief introductory statement
> to distinguish them from contributions made directly via GitHub.
> [See an example of a contribution submitted by email](https://github.com/datacarpentry/r-socialsci/issues/320).
>
{: .callout }

When interacting with contributors, whether new or old, we want to
be sure to embody [The Carpentries values](https://carpentries.org/values/) around communication and teaching
and learning. Part of doing so includes communicating appropriately on Github.

## GitHub Etiquette and Processes

In addition to formal [contributor guidelines](https://github.com/carpentries/maintainer-onboarding/blob/gh-pages/CONTRIBUTING.md), The Carpentries have a set of community norms for working with
GitHub. These include:

* **Including appropriate cross-references:**
    If putting in a PR to address an existing Issue, include a link to the Issue. GitHub will automatically add a note to the Issue linking back to the PR. This is also good practice when communicating in conversation threads on related Issues and PRs.

* **Using the `@` symbol to tag people in a conversation:**
    Most people don't subscribe to all of The Carpentries repositories (there are a lot!) and will only get email alerts if their GitHub handle is tagged. This is a good way to make sure relevant people are included in the conversation.

* **Requesting reviews:**
    You can request a review from a fellow Maintainer or from someone else who has been active on the repository. This is another way of including relevant people in the decision-making process.

* **Not merging your own PRs:**
    Even for small PRs, it's a good idea to have a second pair of eyes to check for typos and formatting issues. In general, always get a second opinion before merging your own PR. This is a good time to request a review.

* **Tagging issues with descriptive labels:**
    For community-submitted issues, remember to add appropriate labels, even if you are not going to immediately take action. This shows contributors that issues are being paid attention to and encourages others to take action on issues.

> ## How to Label Issues
> To find a list of issue labels, their corresponding meanings, and when to use each,
> take a look at this guide on [How to label issues](https://docs.carpentries.org/topic_folders/maintainers/github_labels.html) in The Carpentries handbook.
> The guide also includes instructions on how to populate a Github repository with these issues.
{: .callout}

Being open to new contributions while keeping the lessons sleek and
teachable is a difficult balancing act. It's ok to say no to a
contribution when it doesn't add anything useful to the materials,
goes beyond the scope of the lesson, or introduces unnecessary
complexity. Even when saying no, however, we want to have positive
interactions with contributors and let them know that their
involvement is valued. GitHub's [OpenSource Guide for Maintainers](https://opensource.guide/best-practices/#learning-to-say-no)
has an excellent discussion on learning to say no.

> ## Lesson Maintenance Demo, pt 1 (5 min)
> We will demonstrate briefly how one might respond to a (sample) issue on a lesson.
> At what points during the demo did we use proper Github etiquette? What could have been improved?
{: .challenge}

> ## Lesson Maintenance Demo, pt 2 (5 min)
> We will demonstrate again how one might respond to a (sample) issue on a lesson.
> At what points during the demo did we use proper Github etiquette? What could have been improved?
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
