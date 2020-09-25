d&r update
================

yall! !!!

this is a GitHub repository that will help us manage and update to the [Data at Reed](data-at-reed) site. specifically, the information at \[Analyzing & Visualizing Data &gt; R tutorials\]!

ideally, we can point people who come into the mLab to that site to help address common issues. unfortunately, Nothing Has Happened to those pages for a good bit of time and, as a result, they don’t reflect the kinds of issues we see most often now.

so uhhh they need updating! sweet.

all of the files that the site actually runs off of (is that how you say that? idk web stuff) are held in something called a Content Management System, which is kinda scary. Leila and I are able to pull the files out of there and put them back in, but we'd rather not, like, *work in there*.

okay, so that's where Git comes in. it's my sense that everyone has done a little git, maybe not a ton of Git. various levels of Comfy are fine.

git: tl;dr
----------

this is a *repository*--it's kind of like a folder on Google Drive. however many people we want can have access to it, except...

changes to any documents happen in really discrete steps called *commits*. commits can be as long (i'll draft this README in one) or as short (i.e. fix a typo, see later) as you want.

right now, you're probably looking at the `main` *branch*. branches allow you to "branch off" (~make a copy of) a repository, make changes by adding as many commits as you want, and then *pull requesting* back in (something along the lines of "can i plz merge my changes into the real thing??") to the `main` branch.

doing each of those things for the first time can be scary, and i'll try to make the first go at doing each as cozy as possible. if you'd appreciate more than, say, a sentence of explanation on each of this, i highly recommend Jenny Bryan's book [*Happy Git With R*](https://happygitwithr.com/).

workflow
--------

#### getting set up

okokok let's get to it!

you'll first want to clone this repo to an rstudio project. [HGwR Chapter 15.2](https://happygitwithr.com/new-github-first.html#new-rstudio-project-via-git-clone) is very helpful if you haven't done this before.

alright, you have a project in RStudio now. sweet.

now, groove back to GitHub (look! you're here!) you'll want to branch off of `main` by clicking the down arrow beside `main` in the top left corner, type the new name of your repo (something goofy!), and press Enter.

<img src="readme_figs/branch.png" width="50%" />

now, navigate back to RStudio. look for the "Git" tab in the top right of your screen, and then click the "Pull" (little blue downward-facing arrow) button. it might look something like this:

<img src="readme_figs/git_pane.png" width="50%" />

#### branching off

as of now, you're probably still on the `main` branch. see where it says `main` in the top right corner of that screenshot? click the down arrow directly to it's right and select your new branch:

<img src="readme_figs/select_branch.png" width="50%" />

woop woop woop! almost there!

now, while reading through this document, you might have noticed a typo. (i'm not saying i intentionally placed any--i just make a lot of typos!) there might have also been a step that needed additional clarification for you.

find some spot in this README to make a small edit, make the edit in `README.Rmd`, and then knit to `README.md`. nice.

now, navigate back to the Git pane, check the boxes beside `README.Rmd` and `README.md` (they should be blue now), and press "commit".

<img src="readme_figs/commit.png" width="50%" />

you should be brought to a new window that looks something like this:

<img src="readme_figs/commit_2.png" width="100%" />

in the top right box, you can see that i've written a *commit message*. this will let the rest of us know what you're doing in a commit, and also helps to bring our collaboration workflow much closer to the documents we're actually working on.

i dropped the text `#1` into that commit message. GitHub is smart enough to know that, when i do that, i'm linking to an issue or pull request. (an aside: if i had written `closes #1`, then, when i push that commit, the issue will be automatically closed! slick!)

eventually, we'll have issues open about specific documents (or sections of documents) we're working on. it'll be helpful to know what changes are relevant to what sections of what documents.

okay whatever whatever whatever so write your message to note what you changed, and make sure to link to issue 1 by writing `(#1)` somewhere in your commit message.

now go ahead and press the "Commit" button below your message and then press the "Push" button (the green up arrow.) if you go back to GitHub and navigate to your new branch, you should see your newest commit!

okay okay okay last step! all we need to do now is try to merge our changes back in to the `main` branch.

#### making a PR

while i'm writing this, i just branched off to a branch called `pull-requesting`. i want to merge the changes i'm making now back into `main`.

so i commit, push, and go to look at GitHub. you might see some sort of note along the lines of:

<img src="readme_figs/pr1.png" width="100%" />

if you don't, that's fine! on the top menu, navigate over to "Pull requests". again, you might see the little yellow box. if not, nbd. i clicked "New pull request":

<img src="readme_figs/pr2.png" width="100%" />

this "Comparing changes" window will summarize the changes you made, and ask you to choose what gets pull-requested to what (see those `base:` and `compare:` boxes in the top left of the below screenshot?)

you'll want to change the `compare:` box so that they look like

`[base: main] <- [compare: your branch's name]`

<img src="readme_figs/pr3.png" width="100%" />

now, click "Create pull request"!

<img src="readme_figs/pr4.png" width="100%" />

aaaand once you've written a message, click "Create pull request" again!

you're done!!! woop woop woop!

#### whaaat now

when i see the email from your PR, i'll glance at it quickly and then merge it to `main`. in practice, we will all have the necessary permissions to merge each other's changes.

that's all for now. :-)

in the coming weeks, Leila and I will add all of the necessary files from the site's source and we can get to work on them. more on that workflow to come!

some thoughts:

-   as we work on this project, i highly recommend **every time you open up this project in RStudio, pull!** press the lil feller that is the blue down arrow! this will help prevent...
-   merge conflicts. hopefully we'll have a chance to get grooving a little bit before we come across one, but tl;dr -- two people make changes to the same thing, and Git is like "ahhHHHhHHhH WHAt R U doin?!?!" we'll cross that bridge when we come to it. or maybe i'll write something up beforehand. if not, Happy Git With R [comes in clutch](https://happygitwithr.com/push-rejected.html), as usual.
-   Git can be kind of an uphill battle while you're getting started. especially at first, the *why not just Google Docs?* energy can be strong. **response 1:** it gets better, i promise! **answer 2:** [HGwR, per usual](https://happygitwithr.com/big-picture.html)
-   i appreciate yall. stoked to get started up on this!
