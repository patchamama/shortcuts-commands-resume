# Summarises commands and instructions to be taught and used.

## Linux and MacOs terminal commands:

- `ls`: List files and directories in the current directory.
- `cat`: Concatenate and display the contents of a file.
- `pwd`: Print the current working directory.
- `history`: View a list of previously executed commands.
- `rm`: Remove files or directories. Be cautious as this command is irreversible.
- `mkdir`: Create a new directory.
- `find`: Search for files and directories in a specified location.
- `cd`: Change the current directory.
- `touch`: Create an empty file.
- `cp`: Copy files or directories from one location to another.
- `mv`: Move or rename files or directories.

<details>
<summary>Others</summary>
- `grep`: Search for text patterns within files.
- `echo`: Display a message or variable content in the terminal.
- `ps`: Display a list of currently running processes.
- `kill`: Terminate processes by their process ID (PID).
- `tar`: Create or extract compressed archive files.
- `df`: Show disk space usage.
- `du`: Display disk usage of files and directories.
- `alias`: Create shortcuts or custom commands.
- `sudo`: Execute a command with superuser (administrative) privileges.
- `wget`: Download files from the internet.
- `zip` (Linux) or `ditto` (macOS): Compress files and directories into zip archives.
- `unzip` (Linux) or `ditto` (macOS): Extract files from zip archives.
- `traceroute`: Trace the route packets take to reach a network host.
- `find`: Search for files and directories based on various criteria.
- `tree`: Display directory structure as a tree.
- `who` or `w`: Show who is logged in.
- `chmod`: Change file permissions.
- `chown`: Change file ownership.
- `quota`: Display disk usage and quotas for a user.
- `sudo`: Execute a command with superuser (administrative) privileges.
- `shutdown`: Shut down or restart the system.
- `reboot`: Reboot the system.
- `history`: View and manage command history.
</details>

## GitHub commands frequently used

### Configuration

```
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### Commands

- `git init`: Initialize a new Git repository in the current directory.
- `git clone <repository>`: Create a local copy of a remote repository.
- `git remote add <name> <URL>`: Add a new remote repository.
- `git add <file>`: Stage changes for commit. Example: `git add .` **(to add all the files).**
- `git commit -m "Message"`: **Commit staged changes with a descriptive message.**
- `git status`: View the status of your working directory and staged changes.
- `git log`: Display a history of commits in the repository.
- `git switch  <branch>`: Switch to a different branch.
- `git switch -c  <branch>`: Create an switch to a different branch.
- `git push`: **Push local commits to a remote repository.**
- `git push origin <branch-name>`: Push local commits to a branch in the remote repository.
- `git switch -c updates-branch && git push --set-upstream origin updates-branch`: Create and update a new branch <updates-branch>

<details>
<summary>Others</summary>
- `git branch`: List all local branches and highlight the current branch.
- `git checkout <branch>`: Switch to a different branch.
- `git merge <branch>`: Merge changes from one branch into the current branch.
- `git pull`: Fetch and merge changes from a remote repository.
- `git push`: Push local commits to a remote repository.
- `git remote -v`: View information about remote repositories.
- `git fetch <remote>`: Download changes from a remote repository.
- `git reset <file>`: Unstage changes for a specific file.
- `git reset --hard <commit>`: Reset the current branch to a specific commit.
- `git stash`: Temporarily save changes that are not ready to be committed.
- `git tag <tagname>`: Create a lightweight tag for a specific commit.
- `git diff`: Show differences between the working directory and the last commit.
- `git blame <file>`: Display who made each change to a file and in which commit.
- `git remote remove <name>`: Remove a remote repository.
- `git push --tags`: Push tags to a remote repository.
- `git checkout -b <new-branch>`: Create and switch to a new branch.
- `git branch -d <branch-name>`: Delete a local branch.
- `git push origin --delete <branch-name>`: Delete a remote branch.
- `git rebase <branch>`: Move or combine commits from one branch onto another.
- `git fetch --prune`: Remove references to remote branches that no longer exist.
- `git log --author=<author>`: View commits by a specific author.
- `git log --grep=<pattern>`: Search commit messages for a specific pattern.
- `git log <file>`: View the commit history for a specific file.
- `git remote set-url origin <new-URL>`: Change the URL of a remote repository.
- `git cherry-pick <commit>`: Apply a specific commit to the current branch.
- `git reflog`: Display a log of all Git references, including branch changes.
- `git clean -df`: Remove untracked files and directories.
- `git bisect`: Find the commit that introduced a bug using binary search.
- `git submodule`: Manage Git submodules within a repository.
- `git log --oneline --graph --all`: Display a compact graph of the commit history.
- `git commit --amend`: Modify the last commit with new changes.
- `git remote prune origin`: Prune stale remote-tracking branches.
- `git pull --rebase`: Pull and rebase instead of merging.
- `git log --since=<date>`: Show commits since a specific date.
- `git stash pop`: Apply the last stashed changes and remove them from the stash.
- `git revert <commit>`: Create a new commit that undoes changes from a specific commit.
- `git log --oneline --abbrev-commit`: Display shortened commit hashes in the log.
- `git log --stat`: Show statistics about changes in each commit.
- `git log --graph --decorate`: Display a commit graph with branch and tag labels.
- `git remote show <remote>`: Show information about a remote repository.
- `git log -p <file>`: Display the changes made to a specific file in each commit.
- `git bisect start`: Start the bisection process for finding a bug.
- `git bisect good <commit>`: Mark a commit as good during bisection.
- `git bisect bad <commit>`: Mark a commit as bad during bisection.
- `git bisect reset`: Reset the bisection process.
- `git bisect visualize`: Visualize the bisection process.
- `git clean -n`: Dry run of `git clean` to see what would be removed.
- `git clean -i`: Interactively choose which untracked files to remove.
- `git blame -L <start>,<end> <file>`: Annotate only specific lines of a file.
- `git push -u <remote> <branch>`: Push a local branch to a remote and set up tracking.
- `git cherry-pick --edit <commit>`: Cherry-pick a commit and edit the message.
- `git log --no-merges`: Display a log without merge commits.
- `git log --all --graph --decorate --oneline`: A compact and visual commit history.
- `git grep <pattern>`: Search for a pattern in the contents of files.
- `git log --format="%h %an %s" --since="2 weeks ago"`: Customized log format and time range.
</details>

## Software for developers

- [Google Chrome](https://www.google.com/chrome/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Postman](https://www.postman.com/downloads/)
- [Node](https://nodejs.org/es/)
- [Git](https://git-scm.com/)

## Additional terminal programs

- [Homebrew](https://brew.sh/) Install: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
- [Midnight Commander - mc](https://midnight-commander.org/) Install: `brew install mc` Ex.: `mc` Open editor: `mcedit`
- [Node Version Manager - nvm](https://github.com/nvm-sh/nvm) Install: `brew install nvm` Ex.: `nvm install 16` `nvm use 16`
- [Copilot, for your terminal - plz](https://github.com/m1guelpf/plz-cli) Install: `brew install plz-cli` Ex: `plz how to install react with vite tools`

## VSCode extensions

- [Activitus Bar](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.activitusbar)
- [Paste JSON as Code](https://marketplace.visualstudio.com/items?itemName=quicktype.quicktype)

### Themes:

- [Tokyo Night](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
- [Iconos](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)

### React

- [ES7 React/Redux](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
- [Simple React Snippets](https://marketplace.visualstudio.com/items?itemName=burkeholland.simple-react-snippets)
- [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
- [TypeScript Importer](https://marketplace.visualstudio.com/items?itemName=pmneo.tsimporter)
- [Wallpapers Developer](https://drive.google.com/drive/folders/1ItU8rbSGJjnh2USOBGwaCo9nYKifPJ6m?usp=sharing)

## To do (sections)

- [x] Common commands used in the terminal
- [x] GitHub commands frequently used
- [x] VSCode plugins for developers
- [x] Additional terminal programs to be used in the terminal: mc, homebrew, plz (copilot assistant),...
- [ ] Online IDEs to coding and integrate with github (gitpod, codeanywhere, codesandbox, kodi.link)
- [ ] Markdown and Readme references
- [ ] Free resources (images, icons, wireframes, colors, fonts, designs, libraries)
