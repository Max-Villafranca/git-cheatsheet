## Setting up Git, SSH and GitHub

* system  -all users
* global  -single user all repositories
* local   -single user single repository

`ssh -T git@github.com` Test SSH connection. [Check fingerprint.](https://docs.github.com/en/authentication/) 

`ls -al ~/.ssh` Checks if existing SSH keys are present.

`ssh-keygen -t ed25519 -C "your_email@example.com"` Create SSH keys.

`eval "$(ssh-agent -s)"` Start ssh-agent.

`ssh-add ~/.ssh/id_ed25519` Add SSH private key to the ssh-agent.

`git config --global user.name "name"`

`git config --global user.email "name@email.com"`

`git config --global core.editor "code --wait"`

`git clone <URL>` Clones remote repository.

`git init` Creates new local repository.

`git remote -v` Shows short names and URLs of the remote servers.

`git remote add <shortname> <url>` Add remote repository.


## Working with Git

`git fetch <remote>` Downloads changes from the remote repository.

`git pull <remote>` Same as `git fetch` and `git merge` combined.

`git commit -am` Stages and commits in one step.

`git ls-files` Shows files in staging area (index).

`git status -s` Short status.

`git push <remote> <branch>` Pushes changes to remote repository.

`git mv "old name" "new name"` Renames files both on the working dir and staging area.

<br><picture><img width=500 src="https://user-images.githubusercontent.com/18624609/222594799-df7648d7-38b5-41b5-8085-326079b194ea.png"></picture>

<br><picture><img width=500 src="https://miro.medium.com/max/1200/1*tjrF1ff5UjVNclwwe_GREg.png"></picture>


## Fixing common mistakes

Read the [book](https://git-scm.com/book/en/v2).