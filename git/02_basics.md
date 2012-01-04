!SLIDE title
# Git Basics #

!SLIDE commandline
# Initial working copy setup #

    $ git init .

    $ git clone <url>

!SLIDE commandline
# Getting latest changes #

Simple:

    $ git pull

Details:

    $ git fetch origin
    $ git merge origin/master


!SLIDE commandline small
# Checking edit status #

    $ git status
    # On branch master
    # Changes to be committed:
    #   (use "git reset HEAD <file>..." to unstage)

    #    new file:   git/graph.png

    # Changes not staged for commit:
    #   (use "git add <file>..." to update what will be committed)
    #   (use "git checkout -- <file>..." to discard changes in working directory)

    #    modified:   git/01_intro.md
    #    modified:   subversion/01_intro.md

    # Untracked files:
    #   (use "git add <file>..." to include in what will be committed)

    #    git/02_basics.md


!SLIDE commandline
# Committing #

Will open your $EDITOR for a message.

    $ git add <files>
    $ git commit

OR

    $ git commit -a

!SLIDE commandline
# Branching #

    $ git checkout -b <new branchname>

OR

    $ git branch <new branchname>
    $ git checkout <new branchname>

## Git branches are just pointers (super cheap!!!) ##

!SLIDE commandline
# Merging #

    $ git merge <other branch>

    $ git rebase <other branch>

!SLIDE commandline
# Handling conflicts #

    $ git add <fixed file>
    $ git commit

When more than 1 person edits the same section of a file,
Git doesn't know how to merge.

It leaves .mine, .theirs, .base files for use in
resolving.

Also leaves markers in file: `<<<<<`, `======`, `>>>>>>`.

!SLIDE commandline
# Sharing #

    $ git push
    $ git push <remote> <local branch>:<remote branch>
