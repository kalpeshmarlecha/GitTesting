GitTesting
==========

This is just a testing folder to get started

How to rebase:
==========

To avoid all the confusion, bring the remote branch where you would want to rebase to your local.

```
git checkout master
git pull origin master // origin OR remote, u can decide
git rebase master
```

Resolve the conflicts only by adding files and the continuing

```
git rebase --continue
```

Finally push your changes to the branch and then finally to the remote
If your changes aren't pushed as expected, you can force push if you think your changes are correctly done
```
git push origin mergeOnboard -f
```



If not, you can also force push changes on your remote to bring the branches in sync
To force a branch to come to a particular commit, use this command
```
git reset --hard 18f5e39ea29ed44a56ca60d41b29d7d28ecbdbb2
```

Bring the latest changes from other branches and then force push, if you think you want to push these changes on remote
```
git push origin mergeOnboard -f
```


Just in case for reference:
https://stackoverflow.com/questions/7929369/how-to-rebase-local-branch-with-remote-master
https://blog.algolia.com/master-git-rebase/ -- Didnt read yet
