# **:computer: OS Init**

This repository introduces the essential toolkit to initialize a linux OS from scratch.

# 1.  **[Oh My ZSH](https://github.com/ohmyzsh/ohmyzsh)**

Oh My Zsh is an open source, community-driven framework for managing your [zsh](https://www.zsh.org) configuration.

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

*Note that any previous `.zshrc` will be renamed to `.zshrc.pre-oh-my-zsh`. After installation, you can move the configuration you want to preserve into the new `.zshrc`.*

## **Using Oh My Zsh**

### **Plugins**

Oh My Zsh comes with a shitload of plugins for you to take advantage of. You can take a look in the [plugins](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins) directory and/or the [wiki](https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins) to see what's currently available.

## :wrench: **Worthy Plugins**

See [plugins.md](oh-my-zsh/plugins.md).

