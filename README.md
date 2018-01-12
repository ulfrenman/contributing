Contributing
============
If you want to contribute to a project and make it better, your help is very welcome. Contributing is also a great way to learn more about social coding on Github, new technologies and and their ecosystems and how to make constructive, helpful bug reports, feature requests and the noblest of all contributions: a good, clean pull request.

### How to make a clean pull request

Look for a project's contribution instructions. If there are any, follow them.

- Create a personal fork of the project on Github.
  - Easiest is to use the Fork-button at the top-right of the github-page
- Clone the fork on your local machine. Your remote repo on Github is called `origin`.
  - To clone my (ulfrenman) newly created fork (contribution) use a command like:
    `git clone git@github.com:ulfrenman/contributing.git`
- Add the original repository as a remote called `upstream`.
  - `git remote add upstream https://github.com/MarcDiethelm/contributing.git`
  - See: https://help.github.com/articles/configuring-a-remote-for-a-fork/
- If you created your fork a while ago be sure to pull upstream changes into your local repository.
  - If you made no work with branches you are most likely still on the `master`-branch. Verify this with `git branch`, the star will tell you what branch is currently selected.
  - `pull` is *shorthand for git fetch followed by git merge* so use that:
    `git pull upstream master`
  - See: https://help.github.com/articles/syncing-a-fork/
- Create a new branch to work on! Branch from `develop` if it exists, else from `master`.
- Implement/fix your feature, comment your code.
- Follow the code style of the project, including indentation.
- If the project has tests run them!
- Write or adapt tests as needed.
- Add or change the documentation as needed.
- Squash your commits into a single commit with git's [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.
- Push your branch to your fork on Github, the remote `origin`.
- From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`!
- …
- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.
- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete
your extra branch(es).

And last but not least: Always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.
