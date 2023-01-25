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

*[Fish](http://fishshell.com/)-like fast/unobtrusive autosuggestions for zsh.*

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