# Advanced Git Cheat Sheet

| Command | Explanation & Link |
| ------- | ------- |
| git commit -a | [Stages files automatically](https://git-scm.com/docs/git-commit#Documentation/git-commit.txt---all) |
| git log -p | [Produces patch text](https://git-scm.com/docs/git-log#_generating_patch_text_with_p) |
| git show | [Shows various objects](https://git-scm.com/docs/git-show) |
| git diff | [Is similar to the Linux `diff` command, and can show the differences in various commits](https://git-scm.com/docs/git-diff) |
| git diff --staged | [An alias to --cached, this will show all staged files compared to the named commit](https://git-scm.com/docs/git-diff) |
| git add -p | [Allows a user to interactively review patches to add to the current commit](https://git-scm.com/docs/git-add) |
| git mv | [Similar to the Linux `mv` command, this moves a file](https://git-scm.com/docs/git-mv)
| git rm | [Similar to the Linux `rm` command, this deletes, or removes a file](https://git-scm.com/docs/git-rm) |

[Git cheat sheat](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)

# Git Revert Cheat sheet

[git checkout](https://git-scm.com/docs/git-checkout) is effectively used to switch branches.

[git reset](https://git-scm.com/docs/git-reset#_examples) basically resets the repo, throwing away some changes. It’s somewhat difficult to understand, so reading the examples in the documentation may be a bit more useful.

There are some other useful articles online, which discuss more aggressive approaches to [resetting the repo](https://jwiegley.github.io/git-from-the-bottom-up/3-Reset/4-doing-a-hard-reset.html).

[git commit --amend](https://git-scm.com/docs/git-commit#Documentation/git-commit.txt---amend) is used to make changes to commits after-the-fact, which can be useful for making notes about a given commit.

[git revert](https://git-scm.com/docs/git-revert) makes a new commit which effectively rolls back a previous commit. It’s a bit like an undo command.

There are a few ways you can rollback commits in Git.

There are some interesting considerations about how git object data is stored, such as the usage of sha-1.

# Git Branches and Merging Cheat Sheet

| Command | Explanation & Link |
| ------- | ------- |
| git branch | [Used to manage branches](https://git-scm.com/docs/git-branch) |
| git branch <name> | [Creates the branch](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging) |
| git branch -d <name> | [Deletes the branch](https://git-scm.com/docs/git-branch#Documentation/git-branch.txt--D) |
| git branch -D <name> | [Forcibly deletes the branch](https://git-scm.com/docs/git-branch#Documentation/git-branch.txt--D) |
| git checkout <branch> | [Switches to a branch](https://git-scm.com/docs/git-checkout) |
| git checkout -b <branch> | Creates a new branch and [switches to it](https://git-scm.com/docs/git-checkout#Documentation/git-checkout.txt--bltnewbranchgt). |
| git merge <branch> | [Merge joins branches together](https://git-scm.com/docs/git-merge) |
| git merge --abort | If there are merge conflicts (meaning files are incompatible), --abort can be used to abort the merge action. |
| git log --graph --oneline | [This shows a summarized view of the commit history for a repo.](https://git-scm.com/book/en/v2/Git-Basics-Viewing-the-Commit-History) |

# Git Remotes Cheat-sheet
| Command | Explanation & Link |
| ------- | ------- |
| git remote  | [Lists remote repos](https://git-scm.com/docs/git-remote) |
| git remote -v | [List remote repos verbosely](https://git-scm.com/docs/git-remote#Documentation/git-remote.txt--v) |
| git remote show <name> | [Describes a single remote repo](https://git-scm.com/docs/git-remote#Documentation/git-remote.txt-emshowem) |
| git remote update | [Fetches the most up-to-date objects](https://git-scm.com/docs/git-remote#Documentation/git-remote.txt-emupdateem) |
| git fetch | [Downloads specific objects](https://git-scm.com/docs/git-fetch) |
| git branch -r | [Lists remote branches](https://git-scm.com/docs/git-branch#Documentation/git-branch.txt--r) can be combined with other branch arguments to manage remote branches |
