---
title: "Technical Aspects of Lesson Maintenance"
teaching: 30
exercises: 25
questions:
- "What should I know about how the lessons are formatted?"
- "How do I preview changes?"
- "What terminology is used to describe the lessons?"
- "What files are involved in the lesson and what do they do?"
- "How are the lesson styles maintained?"
objectives:
- "Become comfortable rendering local previews of Carpentry lessons."
- "Describe the relationship between your lesson and the styles repository."
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
{: .challenge}

Start with group discussion about questions?

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

## Previwing Changes and Rendering locally

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
option is to make changes locally, render the full webpage, and then
push those changes back up to GitHub. This requires Jekyll to be
installed and for you to have a local clone of the repository you 
are modifying.

> ## Preparatory Homework
> Follow the [instructions for installing Jekyll](http://swcarpentry.github.io/lesson-example/setup#optional-jekyll-setup-for-lesson-development) and its dependencies.
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
{: .challenge}

> ## Exercise
> In breakout groups, make sure everyone has a local rendering of the
> repo working. Troubleshoot together. Once everyone has a local 
> rendering, have one person screenshare, make a change to one of the
> repository files, and visually confirm that the change has occured
> in the locally rendered webpage. Continue until everyone has 
> screenshared.
{: .challenge}

## Style Maintenance

Section about how lesson styles are maintained. Include information
about Lesson Infrastructure Subcommittee and their mailing list. 

