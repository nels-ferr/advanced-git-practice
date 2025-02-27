<img src="https://raw.githubusercontent.com/LCSB-BioCore/basic-git-practice/master/assets/img/r3-training-logo.png" height="150px"/>

# Advanced git course - Practice repository

First, fork and clone this practice repository.

Add a remote to the upstream repository:
```bash
$ cd advanced-git-practice
$ git remote add upstream git@github.com:LCSB-BioCore/advanced-git-practice.git
$ git fetch upstream
```

Then, create a separate branch from the develop branch:
```bash
$ git checkout -b myBranch upstream/develop
```

Add your name file in the `attendees` directory:

When you are done editing your file, add the file to the stage and commit it:
```bash
$ git add attendees/myName.md
$ git commit -m "Edit the content of the subpage myName.md"
```

Once you are done committing, you can push your branch to your fork:
```
$ git push origin myBranch
```

## Open a pull request

If you now browse to your fork, you can open a pull request and submit it for review.

:warning: Please make sure to select `develop` as the target branch.

:warning: Watch out for comments from the reviewer! If there are things to be changed, change the files locally, commit,
and then push again. The pull request will update automatically.

Once the pull request has been accepted, you will be able to see your page online! :tada:
