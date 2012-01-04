!SLIDE commandline small
# Fancy Log w/ Graph #

    $ git log --date-order --graph --decorate --pretty=oneline --abbrev-commit
    * a2f480d (HEAD, origin/master, master) fix missing SourceResetButton autoload
    * afc0c39 (tag: staging_20111213223105) more fixes for overseer
    *   6c6578e Merge branch 'master' of github.com:CentaurTechnology/newreg
    |\  
    * | 7b1eef3 improvements to overseer
    | * 1f1c9ac resque worker machine shifts
    |/  
    * a21ddb0 fix typo in coverage-aware cleaning code
    * 2c403ec (tag: staging_20111208175710) minor tweaks to out of work email
    * 51a8f2b (tag: staging_20111208004955) Usable out of work email
    *   946916c Merge branch 'production'
    |\  
    | * 0e67998 (tag: production_20111207190059, tag: production_20111207183546) switch production ruby/bundle paths
    | *   1f8cdbb Merge branch 'master' into production

!SLIDE commandline
# What do I need to merge? #

    $ git log --oneline production..master
    a2f480d fix missing SourceResetButton autoload
    afc0c39 more fixes for overseer
    6c6578e Merge branch 'master' of github.com:CentaurTechnology/newreg
    7b1eef3 improvements to overseer
    1f1c9ac resque worker machine shifts
