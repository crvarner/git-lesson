# git-lesson #2: Pull Requests

1. Double check that you are on the main branch and pull down the latest version of this README from github
```
$ git checkout main
$ git pull
```

2. OPTIONAL: list your existing local branches and delete any old development branches (i.e. not `main`) to cleanup your local repo
```
$ git branch
$ git branch --delete BRANCH_TO_DELETE
```

3. Create a branch for your development and check it out
```
$ git branch BRANCH_NAME
$ git checkout BRANCH_NAME
```

4. Create a new file called `chase.txt` and fill it with a message (in your editor). Add that file to the index, and commit it. When you enter the editor to type your commit message, press "i" to enter INSERT mode. Type your message. Press "ESC" to exit INSERT mode. Type ":wq" (stands for "write quit") and press enter. The editor that git opens for entering commit messages is called `vi`. Feel free to google it if you want to learn more. It is a very handy tool to know how to use, as it is installed by default on almost all unix (mac or linux) OS's. You will almost certainly use it to edit files on remote servers at some point in your career.
```
$ git add chase.txt
$ git commit
```

5. Instead of merging your code into main and pushing, you are going to push a branch to the remote repo and open a pull request. This is what we'll be using in the future to review your code. First, list your branches (using the `-vv` flag for extra verboseness). Then push your code, using `-u REMOTE_NAME BRANCH_NAME` to set the upstream branch. In this case, REMOTE_NAME is `origin` and BRANCH_NAME is whatever you named your local branch. Finally, list your branches (again verbosely with `-vv`). You should see that your local branch now "tracks" a remote branch on origin (indicated by `[origin/branch_name]`).
```
$ git branch -vv
$ git push -u origin BRANCH_NAME
$ git branch -vv
```

6. On https://github.com/crvarner/git-lesson/branches, locate the branch you just pushed and create a pull request.

7. Text ya boy!
