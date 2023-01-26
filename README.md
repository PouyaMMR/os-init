# **:computer: OS Init**

This repository introduces the essential toolkit to initialize a linux OS from scratch.

# 1. **Oh My Zsh**

[Oh My ZSH](https://github.com/ohmyzsh/ohmyzsh) is an open source, community-driven framework for managing your [zsh](https://www.zsh.org) configuration.

## **Getting Started**

### **Prerequisites**

- A Unix-like operating system: macOS, Linux, BSD. On Windows: WSL2 is preferred, but cygwin or msys also mostly work.

- [Zsh](https://www.zsh.org) should be installed (v4.3.9 or more recent is fine but we prefer 5.0.8 and newer).

- `curl` or `wget` should be installed

- `git` should be installed (recommended v2.4.11 or higher)

### **Basic Installation**

Oh My Zsh is installed by running one of the following commands in your terminal. You can install this via the command-line with either `curl`, `wget` or another similar tool.

<table>
<tr>
<th>Method</th>
<th>Command</th>
</tr>
<tr>
<td>

**curl**

</td>
<td>

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

</td>
</tr>
<tr>
<td>

**wget**

</td>
<td>

```bash
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

</td>
</tr>
<tr>
<td>

**fetch**

</td>
<td>

```bash
sh -c "$(fetch -o - https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

</td>
</tr>
</table>

_Note that any previous_ `.zshrc` _will be renamed to_ `.zshrc.pre-oh-my-zsh`. _After installation, you can move the configuration you want to preserve into the new_ `.zshrc`.

## **Using Oh My Zsh**

## **Plugins**

Oh My Zsh comes with a shitload of plugins for you to take advantage of. You can take a look in the [plugins](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins) directory and/or the [wiki](https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins) to see what's currently available.

### :wrench: **Worthy Plugins**

See [plugins.md](oh-my-zsh/plugins.md).

## **Themes**

Early in the Oh My Zsh world, we may have gotten a bit too theme happy. We have over one hundred and fifty themes now bundled.

### **Selecting a Theme**

_Robby's theme is the default one. It's not the fanciest one. It's not the simplest one. It's just the right one (for him)._

Once you find a theme that you'd like to use, you will need to edit the `~/.zshrc` file. You'll see an environment variable (all caps) in there that looks like:

```
ZSH_THEME="robbyrussell"
```

To use a different theme, simply change the value to match the name of your desired theme. For example:

```
ZSH_THEME="agnoster" # (this is one of the fancy ones)
# see https://github.com/ohmyzsh/ohmyzsh/wiki/Themes#agnoster
```

_Note: Many themes require installing a [Powerline Font](https://github.com/powerline/fonts) or a [Nerd Font](https://github.com/ryanoasis/nerd-fonts) in order to render properly. Without them, these themes will render [weird prompt symbols](https://github.com/ohmyzsh/ohmyzsh/wiki/FAQ#i-have-a-weird-character-in-my-prompt)._

### :art: **Fancy Themes**

See [themes.md](oh-my-zsh/themes.md).
