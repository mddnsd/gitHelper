# Git helper

This readme file can explain you the basics of git

## First git repository

**Every git-command starts with the word 'git'**

1. git init. Initializing of local git repository. 

Create a folder on local storage, open it with git bash and use 'git init' command there.

```
git init
```

2. git add. Collecting changes in your repository before commit

In your git repository create/change/delete any files, then use 'git add .' command. '.' is used here to add all the changes from repository. You can add any specific file with 'git add <fileName>'

```
git add <fileName> (--all)
```

3. git commit. Commits your changes.

To commit your changes use 'git commit'. You should add some explanation after '-m'.

```
git commit -m '<your commet about commit>'
```

4. git remote. Before pushing your commits into remote repository you should add it.

To add link to remote repository you should use 'git remote add'.

```
git remote add origin <link to your remote repository>
```

5. ssh-keygen. Adding ssh-key to authorize in remote repository (this step requiered only if you have no shh-key and it is not set in your git account)

[Here you can find good instruction to do it](https://inchoo.net/dev-talk/how-to-generate-ssh-keys-for-git-authorization/)

6. git push. Puhes local changes to remote git repository.

For the first push command you need '-u' flag.

```
git push (-u) origin <name of your branch>
```

## Other usefull commands

- git log. Shows you your commits.

- git status. Shows you current changes in your repository.

