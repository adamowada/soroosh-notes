# Useful Terminal Commands

## Navigation

1. List files and folders. Add -a or -al to include hidden files and folders.

```bash
ls
ls -a  # lists hidden files and folders
ls -al  # lists hidden files and folders, in a detailed list
```

2. Prints the folder you're currently in.

```bash
pwd
```

3. Move to a different folder. Use .. to go up a folder. Tab autocomplete is your friend

```bash
cd <folder_name>  # go to <folder_name>
cd ..  # go up one folder
cd  # running cd alone takes you back to your home folder
```

4. Create a folder in current location.

```bash
mkdir <folder_name>
```

5. Create a file in current location.

```bash
touch <file_name>
```

6. Open vscode in current location.

```bash
code .
```

7. View contents of a text file. Useful if the file is short, creates a mess if the file is large or not text based.

```bash
cat <file_name>
```

8. Open file explorer in current location.

```bash
open .
```

9. Delete a file.

```bash
rm <file_name>
```

## Git

1. Clone into a git repository. Creates a new folder in current location.

```bash
git clone <repository_link>
```

2. What branch are you on, what files have been edited.

```bash
git status
```

3. Mark edited files to be saved (committed) to github. Use . to add all files. Use specfic file name(s) to be surgical. You can `git add` multiple times before committing.

```bash
git add .  # git add all edited files
git add <file_path1> <file_path2> ...  # git add one or more specific files
```

4.  Commit the added files, with a message describing the changes. You can `git commit` multiple times before pushing

```bash
git commit -m "your message here"
```

5. Push commit(s) to github, on current branch. For now use the `git push origin` pattern. 

```bash
git push origin <branch_name>  # safer and better when learning. it's more explicit
git push  # fine when tracking is set
```

6. Switch to an already created branch.

```bash
git checkout <branch_name>
```

7. Create a new branch, and switch to that branch.

```bash
git checkout -b <new_branch_name>
```

8. Bring changes from GitHub to local machine.

```bash
git pull origin <branch_name>
```
