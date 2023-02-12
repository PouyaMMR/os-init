# **Debian Testing/Sid**

Nala is officially in the testing and sid repos.

```bash
sudo apt install nala
```

# **Volian Scar**

Alternatively you can use the **Volian Scar** repo.

Updates from this repo are slightly faster than the Debian repos, but usually only about a day sooner.

## **Install the Repository and Keyring**

Head over to [The Volian Archive Release Page](https://gitlab.com/volian/volian-archive/-/releases)

## **Download the following packages:**

- volian-archive-keyring_0.1.0_all.deb

- volian-archive-nala_0.1.0_all.deb

## **Install the archive packages:**

```bash
sudo apt install ./volian-archive*.deb
```

# **Ubuntu 22.04 / Debian Testing/Sid**

Newer releases need to use the mainline package. It is a pure python installation.

After the repository and key are installed simply run:

```bash
sudo apt update && sudo apt install nala
```

# **Ubuntu 21.04 / Debian Stable**

For older distributions you should install `nala-legacy` instead.

```bash
sudo apt update && sudo apt install nala-legacy
```

# **Ubuntu 18.04 / Debian Buster and older**

These distros will not be officially supported.


# **Local .deb**

You can also choose to download our `.deb` and install it locally through `apt` or `dpkg`.

To download the package you can head over to our [Releases](https://gitlab.com/volian/nala/-/releases) page.

From there you can run the command below to install `nala`.

```bash
sudo apt install /path/to/nala_version_arch.deb
```

## **Installing From Source**

There are 2 choices to make on what source to install from:

- Main Branch. This may be ahead of the current release.

- Main Branch, but targeting a specific version.

The first step is to clone the repository. Make sure the following build depends are installed.

```bash
sudo apt install git python3-apt python3-debian pandoc -y
```

## **Clone Main**

```bash
git clone https://gitlab.com/volian/nala.git
cd nala/
```


## **Clone Specific Release**

```bash
git clone --branch=v0.12.1 https://gitlab.com/volian/nala.git
cd nala/
```

## **Ubuntu 22.04 / Debian Stable/Testing/Sid**

```bash
sudo make install
```

## **Ubuntu 20.04 / Debian Buster**

*And maybe older releases*

#### ***The following commands will all install Nala with pip, along with the man pages, translations, shell completions and configuration file.***

Nala requires python3.9+, which these distros do not have.

This method will install python3.10 from source, as that's the version Nala is developed with.
Before continuing you will need the following additional build dependencies:

```bash
sudo apt-get install -y wget build-essential zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libreadline-dev libffi-dev libsqlite3-dev libbz2-dev
```

Now you can get to building and installing Nala!

```bash
sudo make legacy
```

After this is installed, anytime you want to update, a command is provided that will skip building python.

```bash
sudo make legacy-update
```

### **Uninstalling**

```bash
sudo make uninstall
```

If you build the legacy way:

```bash
sudo make uninstall-legacy
```

That's it! Enjoy using Nala!