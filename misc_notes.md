# Misc Notes #

## Generating lists of files that use SDL ## Generate a list of files that
refer to SDL with:

    cd ~jenkins/jobs find . -mindepth 3 -maxdepth 3 -type d | grep workspace \
    | grep -v lib | egrep -v "artifacts|output|temp" | sort \ | xargs grep
    -rns "SDL" 


vim: set filetype=markdown shiftwidth=2 tabstop=2 
