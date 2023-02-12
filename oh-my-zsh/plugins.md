# **zsh-syntax-highlighting**

This package provides syntax highlighting for the shell zsh. It enables highlighting of commands whilst they are typed at a zsh prompt into an interactive terminal. This helps in reviewing commands before running them, particularly in catching syntax errors.

## **How to Install**

### **In your ~/.zshrc:**

Simply clone this repository and source the script:

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
```

Then, enable syntax highlighting in the current interactive shell:

```bash
source ./zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```

If `git` is not installed, download and extract a snapshot of the latest development tree from:

```
https://github.com/zsh-users/zsh-syntax-highlighting/archive/master.tar.gz
```

Note the `source` command must be **at the end** of `~/.zshrc`.

### **With oh-my-zsh**

1. Clone this repository in oh-my-zsh's plugins directory:

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

2. Activate the plugin in `~/.zshrc`:

```
plugins=( [plugins...] zsh-syntax-highlighting)
```

3. Restart zsh (such as by opening a new instance of your terminal emulator).

# **zsh-autosuggestions**

_[Fish](http://fishshell.com/)-like fast/unobtrusive autosuggestions for zsh._

It suggests commands as you type based on history and completions.

## **How to Install**

### **In your ~/.zshrc:**

1. Clone this repository somewhere on your machine. This guide will assume `~/.zsh/zsh-autosuggestions`.

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
```

2. Add the following to your `.zshrc`:

```bash
source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh
```

3. Start a new terminal session.

### **With oh-my-zsh**

1. Clone this repository into `$ZSH_CUSTOM/plugins` (by default `~/.oh-my-zsh/custom/plugins`):

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

2. Add the plugin to the list of plugins for Oh My Zsh to load (inside `~/.zshrc`):

```
plugins=(
    # other plugins...
    zsh-autosuggestions
)
```

3. Start a new terminal session.

# **git-flow-completion**

Bash, Zsh and fish completion support for [git-flow](http://github.com/nvie/gitflow).

The contained completion routines provide support for completing:

- git-flow init and version
- feature, hotfix and release branches
- remote feature, hotfix and release branch names

## **Installation for Bash**

To achieve git-flow completion nirvana:

0. [Install git-completion](http://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion).

1. Install `git-flow-completion.bash`. Either:

   i. Place it in your `bash_completion.d` folder, usually something like `/etc/bash_completion.d`, `/usr/local/etc/bash_completion.d` or `~/bash_completion.d`.

   ii. Or, copy it somewhere (e.g. `~/git-flow-completion.bash`) and put the following line in the `.profile` or `.bashrc` file in your home directory:

   ```bash
    source ~/git-flow-completion.bash
   ```

2. If you are using Git < 1.7.1, you will need to edit git-completion (usually `/etc/bash_completion.d/git` or `git-completion.sh`) and add the following line to the `$command` case in `_git`:

   ```bash
   _git ()
   {
       [...]
       case "$command" in
          [...]
          flow)        _git_flow ;;
          *)           COMPREPLY=() ;;
       esac
   }
   ```

## **Installation for Zsh**

To achieve git-flow completion nirvana:

0. Update your zsh's git-completion module to the newest version -- [available here](http://sourceforge.net/p/zsh/code/ci/master/tree/Completion/Unix/Command/_git). Optional if you have an up-to-date version of zsh.

1. Install `git-flow-completion.zsh`.

   Either:

    <ol style="list-style-type: lower-roman">
    <li>

   Place it in your `.zshrc`.

    </li>
    <li>

   Or, copy it somewhere (e.g. `~/.git-flow-completion.zsh`) and put the following line in your `.zshrc`:

   ```bash
    source ~/.git-flow-completion.zsh
   ```

    </li>
    <li>Or, use this file as an oh-my-zsh plugin.</li>
    <ol style="list-style-type: lower-alpha">
    <li>

   Install the plugin by cloning this repository to your directory for [custom oh-my-zsh plugins](https://github.com/robbyrussell/oh-my-zsh#customization):

   ```bash
   git clone https://github.com/bobthecow/git-flow-completion ~/.oh-my-zsh/custom/plugins/git-flow-completion
   ```

    </li>
    <li>

   Add the plugin to the list of plugins for Oh My Zsh to load (inside `~/.zshrc`):

   ```
   plugins=(
       # other plugins...
       git-flow-completion
   )
   ```

    </li>
    <li>Start a new terminal session.</li>
    </ol>
    </ol>
