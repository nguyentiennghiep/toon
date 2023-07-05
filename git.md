# Setup for new PC 

_updated 2023/02/14_ 
 
## Git setup
  ```
  $ git config --global user.name "Your name here"
  $ git config --global user.email "your_email@example.com"
  ```
  
### Setup ssh key 
  1. Setup SSH key Link (https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

# Git Submodule

## Setup for new project
  ```
  $ git submodule init 
  $ git submodule add {git-repo} 
  ```

## Clone from existing repo 
  ```
  $ git submodule init 
  $ git submodule update
  ```
  
## Update the submodule when pull the parent
  ```
  $ git fetch --all
  ##this pull for the parent
  $ git pull  
  ##This is required for the submodule
  $ git submodule update  
  ```
  
# Git stash
## Git stash include new file 
  ```
  $ git stash --include-untracked -m "Message for remember"
  ##Using flag --include-untracked to stash new file 
  $ git stash list  
  ##show stash list to view stash want to pop
  $ git stash@{0}
  ##pop the stash you want
  ```
# Git trick 
## Check changed file 
  ```
    Check numbers of files changed
    git diff origin/develop --name-only | wc -l
    Check numbers of *.spec.ts* files changed
    git diff origin/develop --name-only | grep '\.spec\.ts' | wc -l
  ```

  



