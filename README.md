# git-lesson

1. Open your terminal and `cd` to your "workspace" where all of your project folders are kept. Clone the repository into your workspace with `git clone`. You now have a complete copy of my online repository. You can see w/ `ls` that it only has one file so far.
```
% git clone https://github.com/crvarner/git-lesson.git
% cd git-lesson
% ls
```

2. Next, create a file called `chase.txt` and write me a message. This is an "untracked" file that git currently doesn't know anything about. You can see the status of your working directory w/ `git status`
```
% git status
```

3. Stage that file to be committed, and check its status again.
```
% git add chase.txt
% git status
```

4. Before committing, check the log to see any previous commits w/ `git log`. You should see 2 commits from me: the "initial commit", and another from me adding instructions to README.md. Commit your staged changes with `git commit`.
```
% git log
% git commit
```

5. `git commit` will bring up a prompt for you to enter a commit message. Enter a meaningful description of the changes included in this commit. Here, you have added the file `chase.txt`. Once committed, check `git log` again. You should see your commit message.
```
% git log
```

6. Finally, you will use `git push` to publish your changes to the "upstream" repository.
```
% git push
```
