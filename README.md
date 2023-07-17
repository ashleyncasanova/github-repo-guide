# Practice GitHub


## 1. Create project

>Note: Execute the following commands in the terminal

```
    cd ~/projects

    mkdir <project-name>

    cd <project-name>
```

## 2. Initialize repository

```
    git init
```

> Option: Rename branch to `main`

```
    git branch -m main
```

## 3. Open VS Code

```
    code .
```

## 4. Add initial commit

>Note: Execute the remaining commands in the interactive terminal (VS Code)

>Note: Use [control + ~] to open terminal in project folder

1. Click new file icon and name (e.g. README.md)
1. Enter the following commands: 

```
    git add .

    git commit -m "Initial commit"
```

## 5. Push to GitHub

1. Navigate to GitHub
1. Click the plus icon (top right) to add a new repository
1. Add repository name and click create repository
1. Copy/paste the last two commands from the box titled "... or create a new repository on the command line"

```
    git remote add origin https://github.com/ashleyncasanova/practice-github.git
    git push -u origin main
```

## 6. Make changes to repository

1. Create feature branch

```
    git checkout -b <branch-name>
```

2. Make changes to file

3. Commit changes

```
    git add .

    git commit -m "Describe what you've changed"
```

4. Push branch to GitHub

```
    git push origin <branch-name>
```

## 7. Merge Pull Request

1. Navigate to GitHub > Profile > repository (practice-github) > Compare & pull request > option: rename > create pull request
1. From merge pull request drop down menu, select and click the option to squash & merge > confirm squash & merge > delete branch

## 8. Done

1. Navigate back to VS code and enter the following:

```
    git checkout main

    git branch -D <branch-name>

    git pull origin main
```

## 9. [Renaming a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository) (optional)

**Step 1: Rename Repository on Github**

1. On GitHub.com, navigate to the main page of the repository.
2. Under your repository name, click the `settings` tab.
3. In the repository name field, type the new name of your repository.
4. Click `rename`.

**Step 2: Reset URL on Local Machine**

1. Navigate back to the main page of your repository.
1. Copy the `NEW-URL` using the drop down menu of the `Code` tab. It should follow the syntax: `https://github.com/user-name/new-name.git`.
1. In the terminal, `cd` into the directory you are renaming.
1. Update any existing local clones to point to the new repository url using the command:

`git remote set-url origin NEW-URL`

**Step 3: Rename folder on your Computer**

1. In the terminal `cd` into the parent directory of the directory you are changing (using `cd ..`) and run the following command: 

`mv old_name new_name`


**Step 4: Check that our url was sucessfully changed**

1. First we need to `cd` back into our new directory.

2. Next we can one one or more of the following tests...

* To check the remote url:

`git config --get remote.origin.url`

* To see all of your remote urls: 

`git remote -v`

* For more information about the remote repository:

`git remote show origin`