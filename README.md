# **:computer: OS Init**

This repository introduces the essential CLI toolkit to initialize a linux OS from scratch.

# 1. **Oh My Zsh**

[Oh My ZSH](https://github.com/ohmyzsh/ohmyzsh) is an open source, community-driven framework for managing your [zsh](https://www.zsh.org) configuration.

## **Getting Started**

### **Prerequisites**

- A Unix-like operating system: macOS, Linux, BSD. On Windows: WSL2 is preferred, but cygwin or msys also mostly work.

- [Zsh](https://www.zsh.org) should be installed (v4.3.9 or more recent is fine but 5.0.8 and newer is preferred).

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
<td style="text-align:center; padding-top: 20px">

**curl**

</td>
<td style="padding-top: 20px">

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

</td>
</tr>
<tr>
<td style="text-align:center; padding-top: 20px">

**wget**

</td>
<td style="padding-top: 20px">

```bash
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

</td>
</tr>
<tr>
<td style="text-align:center; padding-top: 20px">

**fetch**

</td>
<td style="padding-top: 20px">

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

Oh My Zsh world has over one hundred and fifty themes now bundled.

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

# **2. Nala**

[Nala](https://github.com/volitank/nala) is a front-end for `libapt-pkg`. Especially for newer users it can be hard to understand what `apt` is trying to do when installing or upgrading. Nala aims to solve this by not showing some redundant messages, formatting the packages better, and using color to show specifically what will happen with a package during install, removal, or an upgrade.

## **Installation**

See [installation.md](nala/installation.md).

# **3. Exa**

A modern replacement for *ls*.

[Exa](https://github.com/ogham/exa) is a modern replacement for the venerable file-listing command-line program `ls` that ships with Unix and Linux operating systems, giving it more features and better defaults. It uses colours to distinguish file types and metadata. It knows about symlinks, extended attributes, and Git. And it’s **small**, **fast**, and just **one single binary**.

By deliberately making some decisions differently, exa attempts to be a more featureful, more user-friendly version of `ls`. For more information, see [exa’s website](https://the.exa.website/).

## **Command-line Options**

See [command-line-options.md](exa/command-line-options.md).

## **Installation**

### **Debian**

```bash
apt install exa
```

### **Ubuntu**

On Ubuntu 20.10 (Groovy Gorilla) and later:

```sh
sudo apt install exa
```

### **Manual installation from GitHub**

Compiled binary versions of exa are uploaded to GitHub when a release is made. You can install exa manually by [downloading a release](https://github.com/ogham/exa/releases), extracting it, and copying the binary to a directory in your `$PATH`, such as `/usr/local/bin`.

For more information, see the [Manual Installation page](https://the.exa.website/install/linux#manual).

# 4. **V2ray**

[V2ray](https://github.com/v2fly/v2ray-core) platform for building proxies to bypass network restrictions.

## **Installation**

To install v2ray, use the following script:

```sh
bash <(curl -L https://raw.githubusercontent.com/v2fly/fhs-install-v2ray/master/install-release.sh)
```

To install v2ray assets, use the following script, this will add the geoip and geosite files.

```sh
bash <(curl -L https://raw.githubusercontent.com/v2fly/fhs-install-v2ray/master/install-dat-release.sh)
```

To uninstall v2ray from your system, use the following script

```sh
bash <(curl -L https://raw.githubusercontent.com/v2fly/fhs-install-v2ray/master/install-release.sh) --remove
```

## **:electric_plug: Qv2ray: Suitable Linux Client for V2ray**

[Qv2ray](https://github.com/Qv2ray/Qv2ray), is a Qt frontend for V2Ray written in C++.

## **Installation and Configuration**

See [installation.md](qv2ray/installation.md).

