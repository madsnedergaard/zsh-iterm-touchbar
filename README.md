# zsh iTerm Touchbar

> Display feedback of terminal in the 🍏 Touchbar

![preview1](./preview1.jpg)

![preview2](./preview2.gif)

## Features

  * F1 - Current directory 👉
    * runs ls -la
  * F2 - Current git branch 🎋
    * Lists available braches
    * allows your to switch to selected branch
  * F3 - Current git repo status 🔥 / 🙌
    * `+` — uncommitted changes in the index;
    * `!` — unstaged changes;
    * `?` — untracked changes;
    * `$` — stashed changes;
    * `⇣` — unpulled commits;
    * `⇡` — unpushed commits.
  * F4 - Push to origin branch (git push origin [branch]) ✉️
  * F5 - Display `yarn run` scripts from `package.json` ⚡️
    * Lists available scripts
    * Runs selected script
  * F6 - Display `rake tasks` ⚡️
    * Lists available tasks
    * Runs selected task


### Requirements

* iTerm2 3.1.beta.3 (OS 10.10+) - [Download](https://www.iterm2.com/downloads.html)
* [zsh](http://www.zsh.org/) shell

**Into iterm2:** Go into `View -> Customize Tool Bar...` and drag & drop the `Fn` module

### Installing plugin

Clone the repo in your plugins directory:

* `$ cd ${ZSH_CUSTOM1:-$ZSH/custom}/plugins`
* `$ git clone https://github.com/bschnieders86/zsh-iterm-touchbar.git`

Then add the plugin into your `~/.zshrc`:

```
plugins=(... zsh-iterm-touchbar)
```

### Customize

ENV variables for git icons:

```shell
GIT_UNCOMMITTED="+"
GIT_UNSTAGED="!"
GIT_UNTRACKED="?"
GIT_STASHED="$"
GIT_UNPULLED="⇣"
GIT_UNPUSHED="⇡"
```

### Read more / Credits

* [Original iTerm2 issue for TouchBar support](https://gitlab.com/gnachman/iterm2/issues/5281)
* [Thank's to spaceship-zsh-theme for git functions](https://github.com/denysdovhan/spaceship-zsh-theme/blob/9dbaee2cc6cfe0ac407cf901ebb97894ed279660/spaceship.zsh#L143-L173)
