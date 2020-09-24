d\&r update
================

yall\! \!\!\!

this is a GitHub repository that will help us manage an update to the
[Data at Reed](data-at-reed) site. specifically, the information at
\[Analyzing & Visualizing Data \> R tutorials\]\! ideally, we can point
people who come into the mLab to that site to help address common
issues.

## what now?

Leila and I have added all of the previous files in the `old_docs`
folder, and an outline of what the new content could look like below.
Each header is a single document, and below it are some packages and
functionality that we’ll discuss what they do, maybe give an example,
link out to resources that are maintained by authors and collaborators
and *how* to do it, and probably not much more. Each of the new
documents are in `content`, and have corresponding issues linked to the
work that happens on them.

## a new outline

### R at Reed

The RStudio Server & `thesisdown`

### Getting Started

Installing R & RStudio, some terminology, and `palmerpenguins`

### Loading Data

`readr`, `readxl`, `googlesheets4`, `rvest`

### Data Wrangling

`tibble`, `tidyr`, `dplyr`

### Presentation & Visualization

`ggplot2`, `kable`, RMarkdown

### More Resources

Learning more & getting connected (links to the free online textbook,
our hours in the MLab?)

## keeping-in-mind-things

We’ll be using `palmerpenguins` to demonstrate important functions,
instead of `iris`\! Here’s some
[documentation](https://allisonhorst.github.io/palmerpenguins/articles/intro.html)
for `palmerpenguins`, and some info on [why we’re not using
iris](https://www.meganstodel.com/posts/no-to-iris/).

We want people to not only get the information they need, but also to
know where to look if our examples don’t completely answer their
questions (teach a man to fish?). So\! As much as possible, we’ll link
out to other resources (like the Happy Git with R resource Simon linked
to, or tidyverse cheatsheets) so that folks get used to using the
documentation that’s already out there\! Not trying to reinvent the
wheel\!

Workflow-wise, editing the documents will look something like:

  - Check for outstanding (i.e. unmerged) pull requests
  - Make a new branch off of `main`
  - Work on a document, tagging the issue for the relevant document in
    your commit messages
  - At the end of a work session, pull request back to `main`

All of us have permission to merge pull requests\! At the start of your
work sessions on here, check to see if there are any open pull requests.
If so, take a look over your collaborators’ changes, discuss/make edits
on the PR, and (possibly) merge their changes back into `main`.
