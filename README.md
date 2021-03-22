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

4. Create a new file called `chase.txt` and fill it with a message (in your editor). Add that file to the index, and commit it. When you enter the editor to type you commit message, press "i" to enter "INSERT" mode. Type your message. Press "ESC", then type ":wq" and press enter.
```
$ git add chase.txt
$ git commit
```

5. Instead of merging your code into main and pushing directly, you are going to push a branch and open a pull request. This is what we'll be using in the future to review your code.
```
$ git push -u origin BRANCH_NAME:BRANCH_NAME
```

6. On https://github.com/crvarner/git-lesson/branches, locate the branch you just pushed and create a pull request. Then text yo boy.
