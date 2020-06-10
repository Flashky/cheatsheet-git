# cheatsheet-git

#### Delete local commits

Delete last commit:

```
git reset --hard HEAD^
```

Delete last N commits:

```
git reset --hard HEAD~<<NUMBER_OF_COMMITS>>
```

Therefore with 2 commits:

```
git reset --hard HEAD~2
```

#### Delete already pushed commits

Grab the commit you want to delete and type this command locally:

```
git push <<REMOTE_HERE>> +><COMMIT_ID_HERE>>^:<<BRANCH_NAME_HERE>>
```

Example:

```
git push origin +8b39c8271b84b1c2a8bf827706451aee973f0680^:master
```

#### Change user and email for commits

Globally:

```
git config --global user.name <<YOUR_NAME_HERE>>
git config --global user.email <<YOUR_EMAIL_HERE>>
```

Locally:

```
git config user.name <<YOUR_NAME_HERE>>
git config user.email <<YOUR_EMAIL_HERE>>
```

#### Ammend the user and mail of the last commit

```
git commit --amend --author "YOUR_NAME_HERE <YOUR_EMAIL_HERE>"
```

Example:

```
git commit --amend --author "AwesomeUser <awesomeuser@gmail.com>"
```

