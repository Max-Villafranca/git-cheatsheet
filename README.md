## Setting up Git and SSH

* system  -all users
* global  -single user all repositories
* local   -single user single repository

`ls -al ~/.ssh` Checks if existing SSH keys are present.

`ssh-keygen -t ed25519 -C "your_email@example.com"` Create SSH keys.

`eval "$(ssh-agent -s)"` Start ssh-agent.

`ssh-add ~/.ssh/id_ed25519` Add SSH private key to the ssh-agent.

`git config --global user.name "name"`

`git config --global user.email "name@email.com"`

`git config --global core.editor "code --wait"`

`git ls-files` Shows files in staging area (index).

## Working with Git

`git commit -am` Stages and commits in one step.

`git status -s` Short status.

`git mv "old name" "new name"` Renames files both on the working dir and staging area.

<br><picture><img width=500 src="https://user-images.githubusercontent.com/18624609/222594799-df7648d7-38b5-41b5-8085-326079b194ea.png"></picture>

## Fixing common mistakes

