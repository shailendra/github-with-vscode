# github-with-vscode

### Reference links
- How to use Git Integration in Visual Studio Code<br>
https://www.digitalocean.com/community/tutorials/how-to-use-git-integration-in-visual-studio-code
- Github Readme Emoji cheat sheet<br>
https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md
- Working with GitHub in VS Code<br>
https://code.visualstudio.com/docs/editor/github
- Book<br>
https://git-scm.com/book


<br><br><br><br>

### Install Git on your machine
Go to the following website: https://git-scm.com/download.  Download file and install on your machine. After installed git, open command prompt and type ` git `, it will display information about git.
<br><br><br>

### Configure Username and Email in Git
Open CMD and type below command to configure username and email on current system.
```cmd
git config --global user.name "username"
git config --global user.email "user@gmail.com"
```
To list global config
```cmd
git config --global --list
```
<br><br>

### Create a Git repository on github

- click on **new repository**
<br><br>
![alt](images/create-repo.jpg)
<br>

- Give name to repository 
<br><br>
![alt](images/create-repo-info.jpg) <br>
check box **“Initialize this repository with a README”**
if you initialize project locally using git init  then do not click on checkbox, it should be unselect.
<br><br><br><br>


# Cloning a repository in VSCode
- Open Visual Studio Code and click on the Source Control tab (the icon looks like a split in the road) in the left-side panel:
- Click on `Clone Repository`<br>
![alt](images/source-control.jpg)<br>
- Here you have to provide repository path
![alt](images/repo-url.jpg)<br>
You can also open above dialog box using the **Git: Clone** command in the Command Palette `(Ctrl+Shift+P)`
- After `Pres Enter Key` file browser window will open. Provide location to clone repository.
- After Cloned repository on given location. Make changes in file or add any new file.<br>
![alt](images/after-change.png)

- Now you’ll see in the Source Control panel that your new file shows up with the letter `U` beside it. `U` stands for untracked file, meaning a file that is new or changed, but has not yet been added to the repository:
- To commit your changes, type a commit message into the input box at the top of the Source Control panel. Then, click the check icon to perform the commit<br>
![alt](images/commit.jpg)

- Now All committed changes are on local repository. To upload on github repository, Click on push.<br>
![alt](images/push.jpg)

- Now you will see a prompt to sign in. VS Code requires GitHub authentication first time.<br>
![alt](images/auth-prompt.png)<br>

- Follow the steps to sign into GitHub and return to VS Code. After doing so, all local repository will upload on github repository. You must be owner or contributor of that repository.

<br><br><br><br>


# Upload an existing VSCode Project in github
follow below steps to upload an existing VSCode Project in github
- Create a repository on github & copy url
- Goto VS Code and open project/folder
- check git is enabled from settings
- **Initialise Repository** <br>
Click on Source Control icon and Initialize Repository.<br>
![alt](images/initialise-project.jpg)<br>
You can also Initialize using the **Git: Initialize Repository** command in the Command Palette `(Ctrl+Shift+P)`
![alt](images/initialise-project-command.jpg) <br>
then select or choose project location.<br>
![alt](images/workspace-path.jpg)
- **Commit message** <br>
Type a commit message into the input box at the top of the Source Control panel. Then, click the check icon to perform the commit<br>
![alt](images/commit.jpg)<br>
- **Add to remote repository** <br>
After commit upload local git project to github, for this open Command Palette using `(Ctrl+Shift+P)` and type **Git: Add Remote**.<br>
![alt](images/add-remote.jpg)<br>
provide repository url<br>
![alt](images/add-remote-url.jpg)<br>
Give Remote name<br>
![alt](images/add-remote-name.jpg)<br>

- Push commited changes to github repo<br>
![alt](images/push.jpg)
- Check changes on github repo

<br><br><br><br>

# Track or Untrack and Status
Remember that each file in your working directory can be in one of two states: **tracked** or **untracked**. Tracked files are files that were track by git; they can be **unmodified**, **modified**, or **staged**. In short, tracked files are files that Git knows about.<br>
When you first clone a repository, all of your files will be tracked and unmodified because Git just checked them out and you haven’t edited anything.<br>
![alt](images/track-untrack.jpg)<br>
You can check status in two way.
1. Click on Source Control icon. In left side panel every file status will indicate with `U`, `M` and `A`.
2. Type `git status` in terminal and will display status.

![alt](images/status.jpg)


<br><br><br><br>




# Commit Timeline / History
In Timeline you can see commit history of specific file. Select file, then click Timeline Tab. You can see commit history against selected file. Click on any commit to see difference<br>
![alt](images/timeline.jpg)

<br><br><br><br>

# Restore / Revert
### Restore/Revert Specific file
If you accidentally committed a bad version of a file and need to restore from a back version of commit. First look require file in back commit.
1. Select file.
2. Select Timeline Tab
3. Check commit history for correct file. `Right Click` and select `Copy Commit ID`.
![alt](images/timeline-restore.jpg)<br>
you can also view commit id from Command Prompt by `git log --oneline`<br>

Now type `checkout` command with `Commit Id` and `Filename with Relative path` in Command Prompt <br>
```CMD
git checkout commitId filename
git checkout 8046891 images/source-control.jpg
```

<br><br><br><br><br><br><br><br><br><br>


## README.md Markdown Code
Github Readme Emoji cheat sheet<br>
https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md
 
`code or highlight`
- unorder list
- unorder list
1. first
2. second
3. third

**Bold Text**
<br>

![alt](images/source-control-icon.png)

[Link to text ](https://github.com/shailendra/github-with-vscode)
<br>
*Italic text

# Heading

## Heading

### Heading

#### Heading

horizontal rule

----------


