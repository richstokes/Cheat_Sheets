## Setup
Use oh-my-zsh with git plugin, this gives you inline git status on your prompt and tab completion!

```
git config --global user.email "rich.stokes@gmail.com"
git config --global user.name "Rich Stokes"
```

## Clone
`git clone https://github.com/richstokes/hello-world.git `

## Check Status
`git status`

## New Branch
`git checkout -b new-branch-name`

## Add your amended files to the staging area
`git add file.txt`

## Commit your changes
`git commit -m "Commit Message here"`

## Merge changes into original branch
```
git checkout master
git pull origin master
git merge test
git push origin master
```

## Delete branch
`git branch -d delete-this-branch`
