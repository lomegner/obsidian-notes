we have a pull request where we have completed a feature on our branch and now wants to merge it to the master, we ask for a pull request from a team lead to review our code, after they mentioned our mistakes in our files and we changed them, then they can submit our pull request and merge it, when they make a merge, when we pull in our local repository the newly created merged commit has the main branch (if we pull in main/master ) and the origin/master in it.

for checking the comments on our code navigate to pull requests->files changed
for creating pull requests click `new pull request`, base should be `main` and compare should be the branch you want to merge. 

git remote prune origin= sometimes in the GitHub like after the pull request process we delete the remote branch (the local remains) but the remote tracking branch remains in our machine, this command helps us to remove those remote tracking branches from our machine.

so when we're finished completing a feature and now it's turn to be part of project and merged to the master we pull request.

when working on a project either private or open source, always create your branch to work on.