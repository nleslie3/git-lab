# Local git Workflow
- `mkdir my-local-repo` - Creates a new directory
- `cd my-local-repo` - Move into the directory
- `git init` - Initialize a git repository
- `vi readme.txt` - Edit a file `readme.txt`
- Lets write:
```
Learning git is...
FUN!!!
```
- `git status`
- This change hasn't been stage for commit yet.
- `git add readme.txt`
- `git commit -m "Created readme.txt"`
- Lets change how learning git is
- First lets create a new branch: `git checkout -b dev`
- View branches `git branch`
- `vi readme.txt`
- Change "FUN" to "BAD"
- View that the file has been changed, `git status`
- View the actual changes `git diff`
- Lets add the changes to the repo
- `git add readme.txt`
- And commit - `git commit -m "Updated how learning git is."`
- Change branch `git checkout master`, notice that the changes we just made aren't actually visible anymore. That is because the changes were made to a different branch.
- We need to merge our changes back into master.
- `git merge dev`


# Team git Workflow

## Fork the Repo
- Forking is a way to copy a repository into your own account
- It allows you to experiment with changes without affecting the original source. It allows you to propose changes.
- Go to this repo: https://github.com/jdsiddon/git-lab and click "Fork" in the upper right corner.

## Clone the repo
`git clone [YOUR FORKED REPO URL]`

## Change
- Lets update `/index.js`
- Let's pass cheese to our function instead of pepperoni
- From the command line run `git status`
- We still need to add the change to our staging area, `git add index.js`
- Now the change is in our staging area.
- View it using `git diff --staged`
- Now lets push the changes to our own repository `git push origin master`
- You can see those our in git hub


## Submit a Pull Request
- Open your repository in Github and click "New Pull Request"
- View the changes you are asking to be rolled into the main branch
- Click "Create pull request"









https://git-school.github.io/visualizing-git/#free