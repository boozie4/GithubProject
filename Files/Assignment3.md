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
