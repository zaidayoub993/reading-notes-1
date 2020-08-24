Git stores data in a file system made up of snapshots. Each time you save a changed you will get a new version of the project. Because of the necessary found in local resources Git relies on local operations. Git will track the changes applied to any file or directory to minimize the possibility of damage to files such as lost data. Files in Git can reside in three main states: committed which means data is securely stored in a local database, modified which means the file has been changed but not committed to the database.

After installed Git, there are some steps should perform and completed once on any machine. An inherent Git tool called git config allows the setting of configuration variables that control aspects of Git’s operation and look. After installing Git, users should immediately set the user name and email address, which will be used for every Git commit.
Type the following into Terminal or Command Line:
git config --global user.name "Jane Smith"
git config --global user.email "example@email.com"
To confirm that you have the correct settings, enter the following command:
git config --global user.name (should return Jane Smith)
git config --global user.email (should return example@email.com)


To start tracking repository files, perform an initial commit by typing the following:
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”

You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:
$ git clone https://github.com/test


The local Git repository has three components:
Working Directory: The actual files reside here.
Index: The area used for staging
Head: Points to the most recent commit
Tracked: files can be modified, unmodified, or staged; they were part of the most recent file snapshot.
Untracked: files were not in the last snapshot and do not currently reside in the staging area.

To determine the state of files, utilize the git status command.
Track one file only by using the following format: git add filename.
Track all files in a repository by using the following command: $ git add *
To commit a snapshot of all modifications to tracked files in the working directory use $ git commit -a
To push changes from the local “master” branch to the remote repository named “origin” use $ git push origin master

