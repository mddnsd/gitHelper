# Git helper

This readme file can explain you the basics of git

## First git repository

*Before start you should create remote git account. For example on github.com*

**Every git-command starts with the word 'git'**

1. git init. Initializing of local git repository. 

Create a folder on local storage, open it with git bash and use 'git init' command there.

```
git init
```

2. git config. Changes your git configuration.

Use command git config (--global) user.name/user.email to set your credentials for remote repository.

```
git config (--global) user.name: <your user name>
git config (--global) user.email: "<your email>"
```

3. git add. Collecting changes in your repository before commit

In your git repository create/change/delete any files, then use 'git add .' command. '.' is used here to add all the changes from repository. You can add any specific file with 'git add <fileName>'

```
git add <fileName> (--all)
```

4. git commit. Commits your changes.

To commit your changes use 'git commit'. You should add some explanation after '-m'.

```
git commit -m '<your commet about commit>'
```

5. git remote. Before pushing your commits into remote repository you should add it.

To add link to remote repository you should use 'git remote add'.

```
git remote add origin <link to your remote repository>
```

6. ssh-keygen. Adding ssh-key to authorize in remote repository (this step requiered only if you have no shh-key and it is not set in your git account)

[Here you can find good instruction to do it](https://inchoo.net/dev-talk/how-to-generate-ssh-keys-for-git-authorization/)

7. git push. Puhes local changes to remote git repository.

For the first push command you need '-u' flag.

```
git push (-u) origin <name of your branch>
```

## Other usefull commands

- git log. Shows you your commits.

- git status. Shows you current changes in your repository.

## Usefull theory

### Hash.

Hash is a commit ID. You can use 'git log' command to see it. It is the main identifier of commit. Also can be called as "Fingerprint". Every commit has ist own uniq hash.

### Git log

Git log shows you your commits history, where you can find hash, author, date and message of commit.

```
commit e83c5163316f89bfbde7d9ab23ca2e25604af290
Author: Linus Torvalds <torvalds@linux-foundation.org>
Date:   Thu Apr 7 15:13:13 2005 -0700

    Initial revision of "git", the information manager from hell
```

You can additionaly use '--oneline' to get shorter info of commits in one line. It shows only part of the hash and message. The part of the hash is still uniq.

```
e83c5 Initial revision of "git", the information manager from hell
```

If you having issue with automaticly quiting log viewing, you should yse the 'Q' button.

### Head

Head file is one of the .git folder service files. It has a refer to the last commit. With every commit this file updates and gets the newest commit refer. You can use 'HEAD' instead of hash of commits.

### File statuses

There are some statuses of files in repository: untracked, tracked, staged and modified.

untracked - untracked files, which are new in repository. Git is not tracking their changes.

staged - staged files, which have changes but they are added into commit with 'git add' command. (These files are tracked)

modified - modified files, which are different from latest commited versions of them. (These files are tracked)

tracked - tracked files, which changes is tracked by git.

### git status

git status shows you statuses of repository files (can see them upper).