# **ACTIVITY 1**
## Configuration
1. **a. What are the commands to configure your user.name and your user.email?**
* This is a code fence. git config --global user.name "Your Name"
* This is a code fence. git config --global user.email "your_email@example.com"
1. **b. Should this be configured globally or in your repo? Why or why not?**
* It is typically recommended this be configured globally, as it simplifies a developers setup and ensures consistency accross multiple projects. The developers identity is easily and clearly associated with all of the work they put in. 
2. **How do you configure the core editor for git?**
* This is a code fence. git config --global core.editor "<editor_command>"
3. **How do you view your global config and your local (for the repo) config?**
* Global git config: git config --global --list
* Local git config: git config --list

## Working With a Local Repo
4. **What are the steps to create a new local repo via the CLI?**
* This is a code fence. echo "# 'REPO NAME'" >> README.md
* This is a code fence. git init
* This is a code fence. git add README.md
* This is a code fence. git commit -m "first commit"
* This is a code fence. git branch -M main
* This is a code fence. git remote add origin 'URL to Github Repo'
* This is a code fence. git push -u origin main
5. **a. How do you clone a repo?** 
* This is a code fence. git clone 'URL to Github Repo
5. **b. What's the difference between cloning and creating a new repo from scratch?**
*  When cloning a repo, you put the already created repo onto your local machine. This includes its history and all of the changes made. When creating a new repo from scratch, the developer is starting with a clean slate, so to speak, to begin a new project.
5. **c. Practice cloning a public repo from somewhere.**
* I have done this at least once during this class.
6. **How do you look at the status of your repo? What information does this give you?**
* This is a code fence. git status
* This command displays the status of the working directing and the staging area. It will display what changes have been staged, which ones have not, and which files are not being tracked by git.
7. **How do you stage changes to your local repo in prepartion for a commit?**
* This is a code fence. git add -A
8. **How do you commit changes to your local repo?**
* Once the changes are staged, you would use "git commit -m 'commit message'"
9. **Include an example of a file that will allow you to "ignore" files in your repo. What kinds of files should not be part of your version control?**
* In order to "ignore" files in your repo, and .gitignore file needs to be created. An example of a .gitignore file I found at https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#_ignoring is as follows:  
<p># ignore all .a files<br>
*.a<br>  
# but do track lib.a, even though you're ignoring .a files above<br>
!lib.a<br>
# only ignore the TODO file in the current directory, not subdir/TODO<br>
/TODO<br>
# ignore all files in any directory named build<br>
build/<br>
# ignore doc/notes.txt, but not doc/server/arch.txt<br>
doc/*.txt<br>
# ignore all .pdf files in the doc/ directory and any of its subdirectories<br>
doc/**/*.pdf<p>

* Files that should not be included as part of a developers version control include the following:
<p>files that contain sensitive data, such as passwords<br>
files that are generated during the build process, such as log files or temporary files<br>
files that are too large and exceed the maximum size limit for Github, which according to docs.github.com is 100MiB(Mebibyte)<br>
any files that contain local machine specific confogurations or any local ID configurations<p>

10. **When files are under version control, you can't delete them using the OS commands. How do you delete files using git?**
* To delete files using git, you would use the command "git rm" followed by the name of the file. For example, if I were to delete the current file I am working on, I would use the command "git rm Assignment3.md".

## Working With a Remote
11. **How do you view the remote repo that is associated with your local repo?**
* Entering the command "git remote -v" allows you to see the URL associated with the local repo. Output from this command would looke like the following:
<p> origin  git@github.com:OWNER/REPOSITORY.git (fetch)<br>
 origin  git@github.com:OWNER/REPOSITORY.git (push)<p>
 
 12. **What is the function of the git fetch command?**
 *  The "git fetch" command retrieves updates from the remote repo for the developer to inspect before merging them with the current local repo. This command does not change any of the files on the local repo and allows the developer to inspect the changes and choose which changes to merge with the local repo.
 13. **What is the difference between fetch and pull. Practice using both and show the results.**
 * Fetch retrieves updates from the remote repo without merging any of them with the current local repo. Pull automatically merges any updated on the remote repo with the current local repo.
 14. **Make some changes in your repo and using the command line to sync those changes with your remote repo. Show the results.**
 * Image is stored in the Screenshots  folder as "TerminalSyncResults.png".

 ## Branches
 15. **How do you view the local and the remote branches for your repositories?**
 * To see a list of local branches, a developer would use the command "git branch". The current branch will be marked with an asterisk.
 * To see the remote branches, a developer would use the command "git branch -r".
 * To see both remote and local branches at the same time, a developer would use the command "git brand -a".
 16. **View the local branches and create a new branch. Look again. Show before and after.**
 * Screenshots of before and adding a new branch are in the Screenshots folder.
 17. **What are different ways to switch to a new branch?**
 * In order to switch to a different branch, a developer can use one of two commands. The first command, which is the newer one, is "git switch 'branch name'". The second way, which is older but still supported, is "git checkout 'branch name'". 
 18. **Delete your local branch without pushing to a remote or merging to your main branch. Show that it's gone.**
 * A screenshot showing the branch named "new" as deleted is stored in the "Screenshots" folder under the name "LocalBranchesAfterNewBranchDeleted.png".
