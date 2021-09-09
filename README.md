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