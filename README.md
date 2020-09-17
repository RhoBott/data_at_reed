d\&r update
================

yall\! \!\!\!

this is a GitHub repository that will help us manage an update to the
[Data at Reed](data-at-reed) site. specifically, the information at
\[Analyzing & Visualizing Data \> R tutorials\]\!

ideally, we can point people who come into the mLab to that site to help
address common issues. unfortunately, Nothing Has Happened to those
pages for a good bit of time and, as a result, they don’t reflect the
kinds of issues we see most often now.

so uhhh they need updating\! sweet.

all of the files that the site actually runs off of (is that how you say
that? idk web stuff) are held in something called a Content Management
System, which is kinda scary. Leila and I are able to pull the files out
of there and put them back in, but we’d rather not, like, *work in
there*.

okay, so that’s where Git comes in. it’s my sense that everyone has done
a little git, maybe not a ton of Git. various levels of Comfy are fine.

## git: tl;dr

this is a *repository*–it’s kind of like a folder on Google Drive.
however many people we want can have access to it, except…

changes to any documents happen in really discrete steps called
*commits*. commits can be as long (i’ll draft this README in one) or as
short (i.e. fix a typo, see later) as you want.

right now, you’re probably looking at the `main` *branch*. branches
allow you to “branch off” (\~make a copy of) a repository, make changes
by adding as many commits as you want, and then *pull requesting* back
in (something along the lines of “can i plz merge my changes into the
real thing??”) to the `main` branch.

doing each of those things for the first time can be scary, and i’ll try
to make the first go at doing each as cozy as possible. if you’d
appreciate more than, say, a sentence of explanation on each of this, i
highly recommend Jenny Bryan’s book [*Happy Git With
R*](https://happygitwithr.com/).

## workflow

#### getting set up

okokok let’s get to it\!

you’ll first want to close this repo to an rstudio project. [HGwR
Chapter 15.2](https://happygitwithr.com/new-github-first.html#new-rstudio-project-via-git-clone)
might be helpful if you haven’t done this before.

alright, you have a project in RStudio now. sweet.

now, groove back to GitHub (look\! you’re here\!) you’ll want to branch
off of `main` by clicking the down arrow beside `main` in the top left
corner, type the new name of your repo (something goofy\!), and press
Enter.

<img src="readme_figs/branch.png" width="50%" />
