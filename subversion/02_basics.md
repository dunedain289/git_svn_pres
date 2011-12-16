!SLIDE
# SVN Basics #

!SLIDE commandline
# Initial working copy setup #

    $ svn checkout <url>

!SLIDE commandline
# Getting latest changes #

    $ svn update

    U    mobdispatcher/pli.tab
    A    mobdispatcher/cJSON.c
    U    mobdispatcher/mtf_dispatcher.c
    U    mobdispatcher/Makefile
    U    archcov/archcov.cc
    U    archcov/archcov.h
    U    debug/debug.m4
    U    debug/debug.c
    D    spd/chiron.make

!SLIDE commandline
# Checking edit status #

    $ svn status

    ?      cscope.out
    ?      tmp
    M      Makefile
    D      fpudispatcher/acc_readmem.c
    A      fpudispatcher/newfile.c

!SLIDE commandline
# Committing #

    $ svn commit

Will open your $EDITOR for a message.

!SLIDE commandline
# Branching #

    $ svn copy <trunk URL> <branch URL>

## SVN branches are just copies ##

!SLIDE commandline
# Merging #

Tracking trunk:

    $ svn merge <trunk URL>

Integrating into trunk:

    $ svn merge --reintegrate <branch URL>

## Don't use branch after reintegration ##

!SLIDE commandline
# Handling conflicts #

    $ svn resolved <filename>

When more than 1 person edits the same section of a file,
SVN doesn't know how to merge.

It leaves .mine, .theirs, .r389, files for use in
resolving.

Also leaves markers in file: `<<<<< r1`.
