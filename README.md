# Git Overview

# Introduction

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. In simple terms, It's a content manager. It allows to manage and keep track of your code. If the project is broken by any means, you can rollback to a stable or previous version or to fix specific bugs.

## Installation

Installing git differ on most os. I will give the ones that I already test. So let's go :

### Windows

First, you must download the windows installer git. 
You can install on those website [Official Website : git-scm](https://git-scm.com/). Other Option : [gitforwindows](https://gitforwindows.org/).

### Linux

On linux, most everything can be done on the terminal. Git Installation included. 

#### On Debian based systems

`# sudo apt-get install git`

#### On Red Hat based systems

`# sudo dnf install git`

#### On Arch based systems

`# sudo pacman -S git`

After installation, check :
`# git --version or git` 

Result :
`git version 2.36.1`

The latter shows a list of possible with the CLI Tool.

# Let's Start

## Create a local repository

First create a directory on your machine : 

```
# mkdir <whatever-name-you-want>
# cd <whatever-name-you-want>
```

Init your repository : 
` # git init`

After that, it will create the default branch for your local repo.



Now lets create our new file.

`# touch README.md`

Write any content in your file.



Now you can see the status of your local repo : 

`# git status`



CL

``` 
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```



It will advise you to add your modified or created file for this to be commited : 

`# git add README.md `



After you can commit the file :

`# git commit -m "Task : Create .md file" `



CL 

``` 
[master ad4bb8c] Task : Create .md file
 1 file changed, 106 insertions(+)
 mode change 100644 => 100755 README.md
```

 



Now let's configure your local Git : 

- First : Your information 

``` 
$ git config user.name "Jax Jagger"
$ git config user.email "jj@example.com"
```

You can also specify your identity by supplying your name and email address
to the GIT_AUTHOR_NAME and GIT_AUTHOR_EMAIL environment
variables respectively.

You can choose the editor of your choice. Set a new variable for GIT_EDITOR.



You can see the registry of your local repo with :

`$ git log`

See the new status of the repo

`$ git status`




