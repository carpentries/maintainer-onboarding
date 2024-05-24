---
title: Communicating with Contributors
teaching: 15
exercises: 10
---

::::::::::::::::::::::::::::::::::::::: objectives

- Use The Carpentries Core Values to guide your interactions with contributors.
- Gain confidence identifying and politely declining out-of-scope contributions.
- Develop strategies to avoid demotivating contributors.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What types of contributions am I likely to encounter and how should I handle them?
- How do I make sure contributors feel valued, even if their contribution is not accepted?
- How can I direct contributors' energy to where it will be most useful?

::::::::::::::::::::::::::::::::::::::::::::::::::

## Interacting with Contributors

Maintainers represent The Carpentries on some of our most
active online spaces - our GitHub repositories. As a Maintainer,
you will often be the first point of contact for people new to The
Carpentries community.

## Where do Contributions Come From?

While anyone can contribute to The Carpentries lessons, the vast majority of contributions come from:

- Trainees who have gone through Instructor Training and are submitting a contribution as part of "checkout" to complete their Instructor certification.
- Workshop Instructors (and helpers) who have recently participated in a workshop and noticed difficulties with the materials.

Everyone who goes through The Carpentries Instructor Training program is required to [get involved](https://carpentries.github.io/instructor-training/checkout.html#getinvolved) in the Carpentries community in order to become certified, and contributing to a lesson is a popular option. We train over a thousand people each year to be Instructors, about half of whom complete the
certification process. Many of the contributions you will receive come from Instructor trainees. 

During Instructor Training, we [strongly encourage contributors](https://carpentries.github.io/instructor-training/checkout.html) to contribute to
discussion on existing PRs and issues, to submit a PR to resolve an
issue that the Maintainers have marked "help wanted", or to submit issues describing bugs or difficulties in teaching the lesson.

Keeping your repository's "help wanted" list up-to-date is a great way to maximize useful contributions. The Carpentries website
compiles [a list of all issues marked with the "help wanted" tag](https://carpentries.org/help-wanted-issues/) across all of
our official lessons. Contributors can search this list to find places where Maintainers have specifically requested help,
making it more likely that their contribution will be useful and accepted.

:::::::::::::::::::::::::::::::::::::::  challenge

## Help Wanted (5 minutes)

Locate your lesson's help wanted list.

- How many issues are currently open with that tag? How many have been closed?
- Is it clear what action is desired (i.e. what help is wanted?) for each issue marked help wanted?
- Are there any old issues that are out of date and are still marked help wanted?
- Are there any new issues that should have the help wanted tag and don't?

::::::::::::::::::::::::::::::::::::::::::::::::::

Spending some time cleaning up your lesson's help wanted list in your first few months as Maintainer will save
you and your co-Maintainers time in the long term and help ensure higher-quality contributions.

Despite our best efforts in encouraging the types of contributions listed above, you will also receive unwanted or unhelpful contributions, including:

- addition of new material covering topics outside of the scope of the lesson;
- changes to the way a topic is presented that are inconsistent with The Carpentries pedagogical model;
- changes to the technology taught in the lesson (e.g. introduction of a new plotting system);
- multiple unrelated suggestions.

These contributions may come in the form of an issue or a PR. Being open to new contributions while keeping the lessons sleek and
teachable is a difficult balancing act. It's ok to say no to a
contribution when it doesn't add anything useful to the materials,
goes beyond the scope of the lesson, or introduces unnecessary
complexity. Even when saying no, however, we want to have positive
interactions with contributors and let them know that their
involvement is valued. GitHub's OpenSource Guide on "Best Practices for Maintainers" includes a
section on ["learning to say no"](https://opensource.guide/best-practices/#learning-to-say-no). They recommend that you:

- **Thank them** for their contribution.
- **Explain why it doesn't fit** into the scope of the project, and offer clear suggestions for improvement, if you're able. Be kind, but firm.
- **Link to relevant documentation,** if you have it. If you notice repeated requests for things you don't want to accept, add them into your documentation to avoid repeating yourself.
- **Close the request.**

> Content based on [github.com/github/opensource.guide](https://github.com/github/opensource.guide) used under the [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/) license.

:::::::::::::::::::::::::::::::::::::::  challenge

## Practice Saying No (5 minutes)

The issues linked below are good examples of Maintainers saying "no" politely. Read one of these and reflect on how it uses the recommendations from GitHub's 
OpenSource Guide. If you had to respond to this issue, is there anything you would add or do differently? 

- [lc-shell - email submission: suggest adding Hello World](https://github.com/LibraryCarpentry/lc-shell/issues/143)
- [swc-git - Lesson Contribution - Additional Commands](https://github.com/swcarpentry/git-novice/issues/765)
- [swc-r-novice-inflammation - Additional exercise for "Using loops" challenge](https://github.com/swcarpentry/r-novice-inflammation/pull/168)

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::  challenge

## Motivating Language (5 minutes)

We teach Instructors to [avoid using language that can demotivate learners](https://carpentries.github.io/instructor-training/04-expertise.html#just-and-other-dismissive-language). The same principles apply in lesson maintenance. What are some words or
phrases that could have the effect of demotivating contributors? What alternatives can we use to express this meaning in a
positive and motivational way?

In the Etherpad, make a list of demotivating words/phrases and alternatives.


::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::  callout

## Checkout Contributions by Email

We allow trainees to submit feedback and suggested changes
to Data Carpentry and Library Carpentry lessons via email,
as one part of their checkout.

These emails are handled by a member of the Core Team,
who will then open an Issue on the lesson repository
on behalf of the trainee.
The Core Team will not be able to follow up on these Issues,
e.g. by opening a Pull Request
or replying to the thread with more information.
All such Issues will include a brief introductory statement
to distinguish them from contributions made directly via GitHub.
[See an example of a contribution submitted by email](https://github.com/datacarpentry/r-socialsci/issues/320).


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::: callout

## The Curriculum Team may review and merge pull requests
From time to time, members of The Carpentries Curriculum Team may review and/or merge pull requests opened on your lesson repositories.
This might happen because a change is particularly urgent (e.g. it fixes something that is broken in the lesson) or because the change is uncontroversial (e.g. a typo fix or a small improvement to wording, etc) and the Curriculum Team member happens to be looking at the lesson repository at the time.
When a member of the Core Team takes this action, it is not because that they expected one of the Maintainers to have handled the contribution sooner.
If you disagree with a pull request merged by a member of the Curriculum Team, or want to discuss changes like these with them, please get in touch!

::::::::::::::::::::::::::::::::::::::::::::::::::

## Bots and Spam

Unfortunately, The Carpentries repositories occasionally receive time-wasting contributions,
for example containing spurious changes that are not a legitimate attempt to improve the content.
(Previously seen examples have included renaming a file for no clear reason
and making unnecessary and unhelpful changes to the repository README.)
Although we generally encourage you to be thoughtful 
and to avoid demotivating community members when responding to genuine contributions,
you are welcome to close any pull requests and issues that you judge to have been opened in bad faith.
If you suspect that a spammy contribution has been made by an automated account
(for example using the interaction as a way to train and improve a bot's model for automation and communication)
you may wish to close it without any additional comment that could be used as data for the bot's training process.

In addition to closing the issue or pull request,
please [send a short message to The Carpentries team](mailto:team@carpentries.org),
including the user's username and a link to the interaction you have concerns about,
so that the Technology Team can consider blocking the user from your and other Carpentries repositories.

If you believe it is urgent that action is taken,
you may receive a response more quickly by posting to the Maintainers channel on Slack.

As well as closing the pull request or issue and informing The Carpentries team, 
you might consider taking either or both of the following steps:

1. Adding the "invalid" label to the issue/pull request
2. Reporting the issue or pull request to GitHub
   by clicking `...` at the top right of the comment box
   at the beginning of the conversation thread for the issue/pull request
   and selecting "Report content".
   This will take you to the form for reporting violations of [GitHub's terms of service](https://github.com/site/terms).

## Top Ten Tips for Managing Issues and PRs

1. **Acknowledge receipt** - Even if you won't be able to take action on an issue/PR immediately, send the contributor a quick
  message to let them know you received and appreciate their contribution. Always say thank you!
2. **Tag issues with descriptive labels** - For community-submitted issues, remember to add appropriate labels, even if you are not going to immediately take action. This shows contributors that issues are being paid attention to and encourages others to take action on issues.
3. **Include appropriate cross-references** - When putting in a PR to address an existing Issue, include a link to the Issue. GitHub will automatically add a note to the Issue linking back to the PR. This is also good practice when communicating in conversation threads on related Issues and PRs.
4. **Use the `@` symbol to tag people in a conversation** - Most people don't subscribe to all of The Carpentries repositories (there are a lot!) and will only get email alerts if their GitHub handle is tagged. This is a good way to make sure relevant people are included in the conversation. You can also use `@` to tag your Curriculum Advisory Committee. More on that later.
5. **Request reviews** for non-trivial changes. You can request a review from a fellow Maintainer or from someone else who has been active on the repository. This is another way of including relevant people in the decision-making process.
6. **Don't merge your own PRs** - Even for small PRs, it's a good idea to have a second person check for typos and formatting issues. In general, always get a second opinion before merging your own PR. This is a good time to request a review.
7. **Do edit PRs as needed** - It is OK to directly edit a contributor's PR if there are minor issues preventing it from being
  accepted. Many of our contributors are non-responsive to requests to update a PR. This is OK. If the contribution is important - make
  the minor changes and merge.
8. **Don't close an issue or PR without explaining why** - Except in the (very rare) case of spammy contributions, take a moment to
  acknowledge the contribution and explain why it won't be incorporated.
9. **Do close issues** that have gone stale, are outdated, or out of scope (after explaining why).
10. **Pay attention** to comments about accessibility and demotivating or exclusionary language.

:::::::::::::::::::::::::::::::::::::::::  callout

## How to Label Issues

To find a list of issue labels, their corresponding meanings, and when to use each,
take a look at this guide on [How to label issues](https://docs.carpentries.org/topic_folders/maintainers/github_labels.html) in The Carpentries handbook.


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: keypoints

- Valuing all contributions is one of The Carpentries Core Values.
- Not all contributions can, or should, be accepted.

::::::::::::::::::::::::::::::::::::::::::::::::::


