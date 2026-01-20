### Git fetch vs pull

Git fetch:

Git fetch command only downloads new data from a remote repository
It doesn't integrate any of these new data into your working files

Command: git fetch origin
        git fetch -all ---> Tries to merge remote chnages with your local ones.


Git Pull:

Git pulls updates the currennt HEAD branch with the latest changes from the remote server
Downloads new data and integrate it with the current working files

Command: git pull origin master
