#If you create a remote repository directly in Website, it by default takes "MAIN" as the branch. 
#When you pull the contents of this repository into a local repository, the branch HEAD will be set to use branch "MASTER"
#We can change this branch "MASTER" to "MAIN" by the following steps

git branch -m master main

Run the following command which creates a branch called ‘main’ using the history from ‘master’. 
Using the argument -m will transfer all of the commit history on the ‘master’ branch to your new ‘main’ branch so nothing gets lost.


git symbolic-ref refs/remotes/origin/HEAD refs/remotes/origin/main

At this stage if ‘master’ was your default branch you cannot remove it without first changing HEAD, the pointer to the current branch reference.


git branch -a

To see the change in branch and see any other branch not in use.
