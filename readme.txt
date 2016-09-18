# TUTORIAL FOR SETTING UP TERMINAL ON MAC

# edit the default profile for bash scripts
nano ~/.bash_profile # opens up the nano editor and the bash_profile for edit

# after done type ^O and ENTER to save the file and ^X to exit

# Script content:

# Configures command prompt to show: user@hostname:working directory >
export PS1=“\u@\h:\w >”
# renames the list command to show colours and a / on directory
alias ls=“ls -GF”
# change path to drive with script source files
cd /Volumes/LANGARA/ssf




# Setting up git to open Sublime Text
# find Sublime text executable sbl
ls /Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin

# Configure the path to find Sublime Text
export PATH=$PATH:/Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin
export EDITOR='subl -w'

# Configure git to use Sublime Text editor
git config —global core.editor subl

#  Initialize the git repository inside the directory of the repository
git init 

# Check status of files: git status
# Add file to staging area: git add <filename>
# Remove file from staging area: git rm --cached <filename>
# Add changes to file in staging area: git add <filename>
# Show staged files for next commit: git diff --staged
# Commit files on staging area: git commit
# Send files to server on github from destiny to origin: git push srv-fss master
# Get files from server on github: git fetch srv-ssf or git pull srv-ssf
