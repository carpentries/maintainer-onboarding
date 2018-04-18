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

Start with a group discussion about the questions?

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
> repository files, and visually confirm that the change has occurred
> in the locally rendered webpage. Continue until everyone has
> screenshared.
{: .challenge}

## Configuring and Sync Forks

Forks are often used in open source development on GitHub 
to make changes to a project without affecting the original repository. 
You must first configure a remote that points to the upstream repository in Git.
Then, you can sync and fetch updates from or 
submit changes to the original repository with pull requests. 

To **configure a remote** for a fork, follow these commands:

~~~
$ git remote -v
$ git git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git
$ git merge upstream/gh-pages
~~~
{: .bash}

To **sync a fork** of a repository to keep it up-to-date 
with the upstream repository, follow these commands:

~~~
$ git fetch upstream
$ git checkout gh-pages
$ git merge upstream/gh-pages
~~~
{: .bash}

Note, this is different from the typical git workflow 
where master is the typical branch. 
You carn read more about [configuring a remote fork here](https://help.github.com/articles/configuring-a-remote-for-a-fork/) and [syncing a fork here](https://help.github.com/articles/syncing-a-fork/).


## Style Maintenance

The template for Carpentry lessons is managed through the [styles repository](https://github.com/swcarpentry/styles), which is
maintained by [Raniere Silva](https://github.com/rgaiacs) in
coordination with the Lesson Infrastructure Subcommittee. If you
are interested in being involved, please contact Raniere.

