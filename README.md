

# gittuto
**Table of Contents**

- [cheat sheet](#cheat-sheet)
  * [Installing git](#installing-git)
  * [About git](#about-git)
  * [Using Git](#using-git)
    + [configurations](#configurations)
    + [help](#help)
    + [Tracking a directory](#tracking-a-directory)
    + [Start tracking files](#start-tracking-files)
    + [Ignore Files](#ignore-files)



## cheat sheet
This cheat sheet is from Derak Banas website http://www.newthinktank.com/. (I just edited in a more clear Readme File)


### Installing git



1. Mac : http://sourceforge.net/projects/git-osx-installer/

2. Windows : http://msysgit.github.io/

3. Linux : apt-get install git-core OR yum install git-core

### About git

1. Git is a version control tool that saves changes to groups of files so you can revert back if needed.

2. There are different types of version control tools

	a. Local Version Control saves changes to files in a database

	b. Centralized Version Control saves changes to a shared server

	c. Distributed Version Control allows for easier sharing of files then LVC and also eliminates problems that could occur if access to the server is lost under a CVC system.

	d. DVC clients have a complete backup of the files on their computer. If the server is lost the client just waits to regain contact and then uploads changes.

3. When you commit changes to files Git stores a reference of what the files look like at that moment. If a file isn't changed it isn't stored again.

4. Each client has a complete history of all changes stored locally. The client can also access all changes made to the files historically with a simple command. Also those files cannot be changed without Git knowing and changes are difficult to lose.

5. Files transition between 3 states with Git

	a. Modified Files are files that have been recently changed

	b. Staged Files have been marked to be saved

	c. Committed Files are those that have been saved

6. Git saves all file changes to a directory as a compressed database. 

	a. You modify files in Working Directory

	b. You notify that want to save changes in your Staging Area

	c. After you Commit the file changes are saved in the Git directory

### Using Git
#### configurations

global credentials:
```bash
git config --global user.name "Derek Banas" 
git config --global user.email derekbanas@verizon.net

```
Set editor as vim :
```bash
git config --global core.editor "vim" 
```
Set editor as Text Wrangler Mac :
```bash
git config --global core.editor "edit -w" 

```

Show settings :
```bash
git config --list 

```
#### help
```bash
git help OR git help [COMMAND] OR git help add

```
#### Tracking a directory

1. Go to directory
2. shows all files 

```bash
ls -a 

```

3.   Creates the .git directory

```bash
git init

```

#### Start tracking files
a. By type : 
```bash
git add *.java
```

b. By name : 

```bash
git add AndroidManifest.xml

```
c. all :

```bash
git add .
```

 #### Ignore Files

Create a .gitignore file
https://github.com/github/gitignore






