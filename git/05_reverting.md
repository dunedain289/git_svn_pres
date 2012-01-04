!SLIDE commandline
# Reverting 1 file #

    $ git checkout -- <filename>

Pulls a file fresh from the last commit.

!SLIDE commandline
# Reverting everything #

    $ git reset --hard HEAD

Blows away **ALL CHANGES** since your last commit.

Also unstages everything.

!SLIDE commandline
# Undoing a commit with a new commit #

    $ git revert <bad commit>

This creates a new commit that undoes the changes in the bad commit -
always safe.

!SLIDE commandline
# Throwing away commits #

    $ git reset --hard <commit-ish to go back to>

This doesn't actually remove the commits from the db, but they're hard
to get to after this.

!SLIDE commandline
# Trying a merge again #

    $ git reset --hard HEAD^

Resets your branch to it's previous commit (before the merge), so you
can try again or wait for the merge.
