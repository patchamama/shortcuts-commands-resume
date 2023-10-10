# Summarises commands and instructions to be taught and used.

## Linux and MacOs terminal commands:

- `ls`: List files and directories in the current directory.
- `cat`: Concatenate and display the contents of a file.
- `pwd`: Print the current working directory.
- `history`: View a list of previously executed commands. Ex.: `history .` , `history -5`
- `rm`: Remove files or directories. Be cautious as this command is irreversible.
- `mkdir`: Create a new directory.
- `find`: Search for files and directories in a specified location.
- `cd`: Change the current directory.
- `touch`: Create an empty file. Ex.: `touch file-to-create.text`
- `cp`: Copy files or directories from one location to another.
- `mv`: Move or rename files or directories.
- `grep`: Search for text patterns within files. Ex.: `history . | grep <command-to-search>`

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

</details>

## GitHub commands frequently used

### Configuration

```
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global color.ui true
```

### Commands

- `git init`: Initialize a new Git repository in the current directory.

- `git clone <repository>`: Create a local copy of a remote repository.

- `git remote add <name> <URL>`: Add a new remote repository.

- `git add <file>`: Stage changes for commit. Example: `git add .` **(to add all the files).**

- `git commit -m "Message"`: **Commit staged changes with a descriptive message.**

- `git commit -am "commit message"`: **Commit all your tracked files to versioned history**

- `git status`: View the status of your working directory and staged changes.

- `git log`: Display a history of commits in the repository.

- `git switch  <branch>` or `git checkout <branch>`: Switch to a different branch.

- `git switch -c  <branch>` or `git checkout -b <branch>`: Create an switch to a different branch.

- `git push`: **Push local commits to a remote repository.**

- `git push origin <branch-name>`: Push local commits to a branch in the remote repository.

- `git switch -c updates-branch && git push --set-upstream origin updates-branch`: Create and update a new branch <updates-branch>

- `git branch -a`: list the branches

### Make a _Pull Request_ for a provisional branch <lastupdate>

```
git checkout -b lastupdate
git push origin lastupdate

# Open a Pull Request in https://github.com/<project>/lastupdate -> Click: This branch is xxx commits ahead, xxxx commit behind origin-repo:main.

# Merge the lastupdate branch with main
git checkout main
git merge lastupdate

#Remove the lastupdate branch
git branch -d lastupdate
# git push origin --delete lastupdate

```

[Git Command Explorer](https://gitexplorer.com/)

_[Git Cheat Sheet](https://www.reddit.com/media?url=https%3A%2F%2Fi.redd.it%2F8341g68g1v7y.png)_

![Git Cheat Sheet](https://qph.cf2.quoracdn.net/main-qimg-be0c4389a44fea9757d650d578252164-pjlq)

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
- [Mongo Compass](https://www.mongodb.com/try/download/compass)\*
- [Table Plus](https://tableplus.com/)\*
- [Node](https://nodejs.org/es/)\*
- [Docker Desktop](https://www.docker.com/get-started)
  Download docker images: `docker pull mongo:6.0.6`\*

_\* for backend development_

## Additional terminal programs

- [Homebrew](https://brew.sh/) Install: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
- [Midnight Commander - mc](https://midnight-commander.org/) Install: `brew install mc` Ex.: `mc` Open editor: `mcedit`
- [Node Version Manager - nvm](https://github.com/nvm-sh/nvm) Install: `brew install nvm` Ex.: `nvm install 16` `nvm use 16`
- [Copilot, for your terminal - plz](https://github.com/m1guelpf/plz-cli) Install: `brew install plz-cli` Ex: `plz how to install react with vite tools` Conf.: `export OPENAI_API_KEY='sk-...'`

## VSCode extensions

- [Activitus Bar](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.activitusbar)
- [Paste JSON as Code](https://marketplace.visualstudio.com/items?itemName=quicktype.quicktype)
- [Version Lens](https://marketplace.visualstudio.com/items?itemName=pflannery.vscode-versionlens)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens): ErrorLens turbo-charges language diagnostic features by making diagnostics stand out more prominently, highlighting the entire line wherever a diagnostic is generated by the language and also prints the message inline.
- [Console Ninja](https://marketplace.visualstudio.com/items?itemName=WallabyJs.console-ninja): JavaScript console.log output and runtime errors right next to your code.
- [Image Preview](https://marketplace.visualstudio.com/items?itemName=kisstkondoros.vscode-gutter-preview): Shows image preview in the gutter and on hover
- [Fluent Icons](https://marketplace.visualstudio.com/items?itemName=miguelsolorio.fluent-icons): Fluent product icons for Visual Studio Code

### Themes:

- [Tokyo Night](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
- [Icons](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)

### React

- [ES7 React/Redux](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
- [Simple React Snippets](https://marketplace.visualstudio.com/items?itemName=burkeholland.simple-react-snippets)
- [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
- [TypeScript Importer](https://marketplace.visualstudio.com/items?itemName=pmneo.tsimporter)
- [Wallpapers Developer](https://drive.google.com/drive/folders/1ItU8rbSGJjnh2USOBGwaCo9nYKifPJ6m?usp=sharing)

### NodeJS and Django (backend)

- [.env](https://marketplace.visualstudio.com/items?itemName=mikestead.dotenv)
- [Better Dockerfile Syntax](https://marketplace.visualstudio.com/items?itemName=jeff-hykin.better-dockerfile-syntax)
- [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
- [Dockers VSCode](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
- [Terminal](https://marketplace.visualstudio.com/items?itemName=formulahendry.terminal&ssr=false#overview)

## Online IDEs to coding and tools to integrate with github

### IDE Integrated with github to coding and sync the repository

- [GitPod](https://gitpod.io/) | [GitHub Chrome Plugin](https://chrome.google.com/webstore/detail/gitpod/dodmmooeoklaejobgleioelladacbeki) | [Template to fork](https://github.com/Code-Institute-Org/gitpod-full-template)
- [CodeAnyWhere](https://codeanywhere.com/signin) | [GitHub Chrome Plugin](https://chrome.google.com/webstore/detail/codeanywhere/jdofbmaiblhheoneemdjccjeeihbiabl) | [Template to fork](https://github.com/Code-Institute-Org/ci-full-template)
- [Chrome to open GitHub in VS Code](https://chrome.google.com/webstore/detail/open-github-in-vs-code/pnhnmmcigmleaooedjnodnioapklfngc)

### Online live editor to coding and share

- [CodeSandbox](https://codesandbox.io/): An online code editor for web development. Support JavaScript, TypeScript, React, HTML, CSS, and more.
- [codi.link](https://codi.link) | [codi.link in github](https://github.com/midudev/codi.link): A simple platform for sharing code snippets in JS, HTML, CSS and is possible to install libraries with npm.
- [replit.com](https://replit.com/): An online IDE for coding and collaboration with over 50 languages including Python, JavaScript, Java, C++, and more.
- [Python Tutor](https://pythontutor.com/): An interactive Python code visualizer, that support JavaScript ES6, python 2.7, 3.6 and 3.11, c (c17 + GNU extensions, gcc 9.3), c++, java 8.
- [Google Colabs](https://colab.research.google.com/): A cloud-based Jupyter Notebook for Python.
- [Python Online Compiler - Programiz](https://www.programiz.com/python-programming/online-compiler/?ref=735b4d58): An online Python code compiler by Programiz.
- [Code Pen](https://codepen.io/pen/): HTML, CSS and JavaScript online editor.
- [Amazon Cloud IDE - AWS Cloud9](https://aws.amazon.com/cloud9/): Cloud9 IDE is an Online IDE (integrated development environment), published as open source from version 2.0, until version 3.0. It supports multiple programming languages, including C, C++, PHP, Ruby, Perl, Python, JavaScript with Node.js, and Go.
- [WebStorm](https://www.jetbrains.com/webstorm/): WebStorm is a powerful IDE for JavaScript development which helps you write high-quality code quickly, regardless of how complex your projects might be. With out-of-the-box support for all popular technologies.

## Free online courses

- [Full Stack open with certification](https://fullstackopen.com/en/) | [Videos in spanish](https://patchamama.github.io/fast-simple-course-generator/): Deep Dive Into Modern Web Development. Learn React, Redux, Node.js, MongoDB, GraphQL and TypeScript in one go! This course will introduce you to modern JavaScript-based web development. The main focus is on building single page applications with ReactJS that use REST APIs built with Node.js. The course is available in english, spanish, francais and portuguese.
- [CS50's Web Programming with Python and JavaScript - Computer Science, Harvard University](https://pll.harvard.edu/course/cs50s-web-programming-python-and-javascript?delta=0): This course picks up where CS50 leaves off, diving more deeply into the design and implementation of web apps with Python, JavaScript, and SQL using frameworks like Django, React, and Bootstrap.
- [freeCodeCamp](https://www.freecodecamp.org/): Learn to code — for free. Build projects. Earn certifications.
- [Aprende JavaScript](https://www.aprendejavascript.dev/): Curso para aprender paso a paso JavaScript.
  100% gratis y práctico. Desde cero.
- [El Tutorial de JavaScript Moderno](https://es.javascript.info/): Aquí aprenderemos JavaScript, empezando desde cero y llegaremos hasta conceptos avanzados como POO.
- [Learn Python with certification](https://programiz.pro/learn/master-python?utm_source=compiler-nav&utm_campaign=programiz&utm_medium=referral): Learn to code in Python—a beginner-friendly programming language used in data analysis, web development, task automation, and many other fields.
- [Preguntas de entrevista para React](https://github.com/midudev/preguntas-entrevista-react): De cero a experto. Con respuestas detalladas en Español
- [Scrimba.com](Scrimba.com)

  ## English certifications

- https://www.efset.org (free)

<details>

<summary>Others youtube courses</summary>

- https://www.youtube.com/@DevTalles/playlists (flutter, riverpod, react, dart, javascript, git+ github, javascript)

- https://www.youtube.com/@midulive/playlists (react, nodejs, typescript, javascript)

- https://www.youtube.com/@freecodecampespanol/playlists | https://www.youtube.com/@freecodecamp/playlists (html, css, python, ... all in one)

- https://www.youtube.com/@jonmircha/playlists (html, css, flexbox CSS, php (17+43), javascript (fullstack 165), figma, bootstrap, nodeJS (45), React (109))

- https://www.youtube.com/@pildorasinformaticas/playlists (html + css, java, php, excel, access, c++, laravel, android, python)

- https://www.youtube.com/playlist?list=PLSnadb41DsdKxcWm4wFElbfM6aUhwHjzL (git, html, css, react)

- https://www.youtube.com/@Develoteca/playlists (html, php, laravel, python, java)

</details>

<details>

<summary>Games to learn to program</summary>

- Git → ohmygit․org

- Python → codedex․io

- CSS → flukeout․github․io

- JavaScript → warriorjs․com

- VIM → vim-adventures․com

- SQL → mystery.knightlab․com

- TypeScript → codingame․com

- Ruby → github․com/ryanb/ruby-warrior

</details>

<details>

<summary>Algorithms and programming logic</summary>

- https://frontendmentor.io
- https://es.khanacademy.org/computing/computer-science/algorithms
- https://app.codesignal.com
- https://the-algorithms.com/es
- https://www.patterns.dev/
- https://adventjs․dev
- https://leetcode․com
- https://codewars․com
- https://exercism․org
- https://coderbyte․com
- https://codesignal․com
- https://hackerrank․com

</details>

## Webs to test _logic of programming_

- [adventjs․dev](https://adventjs․dev)
- [leetcode․com](https://leetcode․com)
- [codewars․com](https://codewars․com)
- [exercism․org](https://exercism․org)
- [coderbyte․com](https://coderbyte․com)
- [codesignal․com](https://codesignal․com)
- [hackerrank․com](https://hackerrank․com)
- [Project Euler](https://projecteuler.net/)

## Deploy servers gratis (+github integration)

- [Fl0](https://www.fl0.com/): One app gratis, js, python, php, go and Rust. Dockerfile, github integration

## Dockers and containers

- [OrbStack](https://orbstack.dev):OrbStack is the fast, light, and easy way to run Docker containers and Linux. Develop at lightspeed with our Docker Desktop alternative.

## Databases servers and installations

## Install react from scratch

- With vite see details [here](docs/react-vite-install/README.md)

## Programming resources

### CSS Libraries

- [Bootstrap](https://getbootstrap.com/): Powerful, extensible, and feature-packed frontend toolkit. Build and customize with Sass, utilize prebuilt grid system and components, and bring projects to life with powerful JavaScript plugins
- [Tailwind Elements](https://tailwind-elements.com/): Bootstrap components recreated with Tailwind CSS, but with better design and more functionalities
- [CSS Animations](https://animista.net)
- https://cssgrid-generator.netlify.app

### Icons

- https://tabler-icons.io

### HTTP Status Code (Errors, and more...)

- https://http.cat

### Create JSON with data to tests and convertions

- https://jsondataai.com
- https://app.quicktype.io

### Free web templates to start a project

- windbasics.com

## To do (sections)

- [x] Common commands used in the terminal
- [x] GitHub commands frequently used
- [x] VSCode plugins for developers
- [x] Additional terminal programs to be used in the terminal: mc, homebrew, plz (copilot assistant),...
- [x] Online IDEs to coding and integrate with github (gitpod, codeanywhere, codesandbox, codi.link)
- [x] Free online courses
- [ ] Markdown and Readme references
- [ ] Free resources (images, icons, wireframes, colors, fonts, designs, libraries)
- [ ] Basic installation of react with vite, create-react-app, pnpm and main libraries with some tips
- [ ] Basic installation of nodeJS with main libraries, esLint
- [x] Main free servers to deploy app in cloud
- [ ] Database servers and installations
