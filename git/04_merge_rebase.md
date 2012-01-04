!SLIDE bullets
# Merge vs. Rebase #

Similar result, different history in repo.

Merge creates merge commits with 2 parents.

Rebase replays one branch's commits on top of another. Results in a
linear history, even if it didn't actually happen that way.

!SLIDE center
# Merge #

![merge](merge.png)

!SLIDE center
# Rebase #

![rebase](rebase.png)

!SLIDE bullets
# WARNING #

# REBASE CHANGES HISTORY #

Don't do this if you've pushed (shared) the commits you're rebasing.

If you do, you'll cause **lots of pain** for others when they pull!
