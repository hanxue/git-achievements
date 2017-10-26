# Git Achievements

Git-Achievements records all of the achievements you acquire while using Git.

There are over 40 achievements, most with different levels to be achieved. After a git command is executed if a new achievement is unlocked git-achievements will display a message on the console for your enjoyment:

```
********************************************************************************
                            Git Achievement Unlocked!

                                    Caretaker
                    Added a .gitignore file to a repository.
********************************************************************************
```

## GitHub Pages

A log of all of your achievements is kept locally, but you can also publish it to GitHub pages so you can share your achievements (and there is an RSS feed so people can track your achievements).

For example the project maintainer's achievements page is at http://hanxue.github.io/git-achievements/.

If you are viewing a forked version of git-achievements you want to replace hanxue with the GitHub user account you want to see like so:

http://**username**.github.com/git-achievements

To push your achievements to GitHub first fork the project on GitHub, clone *your* repository and set the following config to true:

```
git config --global achievement.upload "true"
```

When an achievement is unlocked the index.html file will be overwritten, committed, and then a `git push origin` will be executed.


## Install

Add git-achievements to your path and alias git to git-achievements. For example add the following to the end of your `~/.bash_profile`

```
export PATH="$PATH":~/git/git-achievements
alias git="git-achievements"
```

You can get your first achievement by running

```
git achievements --help
```

### macOS

You need to install GNU Coreutils and make the GNU `readlink` command available as `greadlink`. An easy way to do that is to use Homebrew to install coreutils. 

```
brew update && brew install coreutils
```

Run the followng command or add it to your `~/.bash_profile~

```
export PATH="/usr/local/opt/coreutils/libexec/gnubin:$PATH"
```

