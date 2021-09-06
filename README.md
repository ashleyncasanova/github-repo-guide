# Practice GitHub


## Create project

```
cd ~/projects

mkdir <project-name>

cd <project-name>
```

## Initialize repository

```
git init
```

> Optionally: Rename branch to `main`

```
git branch -m main
```

## Add initial commit

```
git add .

git commit -m "Initial commit"
```

## Push to GitHub

1. Navigate to GitHub
1. Click the plus icon (top right) to add a new repository
1. Add repository name and click create repository
1. Copy/paste the last two commands

```
git remote add origin https://github.com/ashleyncasanova/practice-github.git
git push -u origin main
```

## Make changes to repository

Create feature branch

```
git checkout -b <branch-name>
```

Make changes

Commit changes

```
git add .

git commit -m "Describe what you've changed"
```

Push branch to GitHub

```
git push origin <branch-name>
```

