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
  
  



