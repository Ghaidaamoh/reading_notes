
## By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.


$ cd example

$ git remote -v

remote1 https://github.com/remote1/example (fetch)

remote1 https://github.com/remote1/example (push)

remote2 https://github.com/remote2/example (fetch)

remote2 https://github.com/remote2/example (push)

remote3 https://github.com/remote3/example (fetch)

remote3 https://github.com/remote3/example (push)
Adding Remotes
To create a new remote Git repository with a short name, use the following format:

git remote add shortname url
Example:

$ git remote

origin

$ git remote add js https://github.com/janesmith/project1

$ git remote -v

origin https://github.com/johndoe/project1 (fetch)

origin https://github.com/johndoe/project1 (push)

js     https://github.com/janesmith/project1 (fetch)

js     https://github.com/janesmith/project1 (push)
This addition of these remote and short names allows you to use shortnames for Git collaboration.

**Fetching**
Fetching entails pulling data that you don’t have from a remote project.

Here is the command format:

git fetch [remote-name]


__Cloned Repositories__

For cloned repositories, use the command git fetch origin to pull down any new changes that were pushed to the server since you cloned or last fetched from it.


**Pushing**
To push your changes “upstream” for sharing, you would use the following git push command format:

git push [remote-name][branch-name]
Example:

$ git push origin master
*This command pushes committed changes from your local “master” branch upstream to the “origin” server.

Note: You can only successfully push changes upstream if you have write access for the server from which you cloned, and if someone else has not pushed changes upstream that you haven’t pulled yet. If a collaborator pushed changes upstream after you had cloned, your push will not be successful. You will have to pull new changes and merge them with your branch before you can successfully push your changes upstream.

Renaming/Removing Remotes
Rename

To rename a remote’s short name, use the git remote rename command.

Example:

$ git remote rename js jane

$ git remote

origin

jane
*In the example above, we can see that the remote’s short name has been changed from js to Jane. The command git remote lists our existing remotes, which jane is now one of. The rename action also alters names of remote branches: js/master would change to jane/master.

Remove

To remove a remote for whatever reason (e.g., a contributor has left the team, the server has moved), simply use the git remote rm command:

Example:

$ git remote rm jane

$ git remote

origin
NOTE: Reminder: “origin” is simply the default remote name when you use the git clone command.

Undoing Actions
Git has mechanisms for undoing certain actions.

Commit Mistakes
You can use the –amend command when you need to alter a commit message or forgot to add some files.

$ git commit --amend
In the example above, you can use this command to easily change your commit message, if no changes were made since the newest commit.

$ git commit -m “my first commit”

$ git add example_file

$ git commit --amend
In the above example, a forgotten file is added to a commit.

Unstaging a File
$ git reset HEAD index.html

Unstaged changes after reset:

M index.html
Above, we see that the git reset HEAD command unstaged the index.html file.

NOTE: When git reset --hard is used, Git overwrites all changes in the working directory, permanently destroying any uncommitted changes.

Undo a Committed Snapshot
To undo changes resulting from a particular commit, use the git revert command. This command appends a new commit that undoes changes introduced by a specific commit. This prevents Git from losing history.

$ git commit -m "Example Commit"

$ git revert HEAD
*In the example above, a new commit gets appended and rolls back changes from a specific commit.

Unmodifying a File
To have a file return to its state when you last committed, utilize the git checkout command.


**Branching**
Almost every type of Version Control System incorporates branching. By creating branches of a central repository, collaborators are able to work on a project simultaneously via multiple branches, without affecting this main repository.
=======
## By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.


$ cd example

$ git remote -v

remote1 https://github.com/remote1/example (fetch)

remote1 https://github.com/remote1/example (push)

remote2 https://github.com/remote2/example (fetch)

remote2 https://github.com/remote2/example (push)

remote3 https://github.com/remote3/example (fetch)

remote3 https://github.com/remote3/example (push)
Adding Remotes
To create a new remote Git repository with a short name, use the following format:

git remote add shortname url
Example:

$ git remote

origin

$ git remote add js https://github.com/janesmith/project1

$ git remote -v

origin https://github.com/johndoe/project1 (fetch)

origin https://github.com/johndoe/project1 (push)

js     https://github.com/janesmith/project1 (fetch)

js     https://github.com/janesmith/project1 (push)
This addition of these remote and short names allows you to use shortnames for Git collaboration.

**Fetching**
Fetching entails pulling data that you don’t have from a remote project.

Here is the command format:

git fetch [remote-name]


__Cloned Repositories__

For cloned repositories, use the command git fetch origin to pull down any new changes that were pushed to the server since you cloned or last fetched from it.


**Pushing**
To push your changes “upstream” for sharing, you would use the following git push command format:

git push [remote-name][branch-name]
Example:

$ git push origin master
*This command pushes committed changes from your local “master” branch upstream to the “origin” server.

Note: You can only successfully push changes upstream if you have write access for the server from which you cloned, and if someone else has not pushed changes upstream that you haven’t pulled yet. If a collaborator pushed changes upstream after you had cloned, your push will not be successful. You will have to pull new changes and merge them with your branch before you can successfully push your changes upstream.

Renaming/Removing Remotes
Rename

To rename a remote’s short name, use the git remote rename command.

Example:

$ git remote rename js jane

$ git remote

origin

jane
*In the example above, we can see that the remote’s short name has been changed from js to Jane. The command git remote lists our existing remotes, which jane is now one of. The rename action also alters names of remote branches: js/master would change to jane/master.

Remove

To remove a remote for whatever reason (e.g., a contributor has left the team, the server has moved), simply use the git remote rm command:

Example:

$ git remote rm jane

$ git remote

origin
NOTE: Reminder: “origin” is simply the default remote name when you use the git clone command.

Undoing Actions
Git has mechanisms for undoing certain actions.

Commit Mistakes
You can use the –amend command when you need to alter a commit message or forgot to add some files.

$ git commit --amend
In the example above, you can use this command to easily change your commit message, if no changes were made since the newest commit.

$ git commit -m “my first commit”

$ git add example_file

$ git commit --amend
In the above example, a forgotten file is added to a commit.

Unstaging a File
$ git reset HEAD index.html

Unstaged changes after reset:

M index.html
Above, we see that the git reset HEAD command unstaged the index.html file.

NOTE: When git reset --hard is used, Git overwrites all changes in the working directory, permanently destroying any uncommitted changes.

Undo a Committed Snapshot
To undo changes resulting from a particular commit, use the git revert command. This command appends a new commit that undoes changes introduced by a specific commit. This prevents Git from losing history.

$ git commit -m "Example Commit"

$ git revert HEAD
*In the example above, a new commit gets appended and rolls back changes from a specific commit.

Unmodifying a File
To have a file return to its state when you last committed, utilize the git checkout command.


**Branching**
Almost every type of Version Control System incorporates branching. By creating branches of a central repository, collaborators are able to work on a project simultaneously via multiple branches, without affecting this main repository.

