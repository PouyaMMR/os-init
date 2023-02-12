# **Installation**

You can install Qv2ray via several methods:

## **1. Via an App Store**

### **Snapcraft**

```sh
# To install the package:
snap install qv2ray
# snap install qv2ray --edge (dev branch)
# To update the package:
snap refresh qv2ray
```

### **Flathub**

1. Set up Flatpak environment according to the [official documentation](https://flatpak.org/setup/).

2. Install Qv2ray:

```sh
# To install the package:
flatpak install com.github.Qv2ray
# To update the package:
flatpak update
```

## **2. Via AppImage**

Go to the [official release page](https://github.com/Qv2ray/Qv2ray/releases) and download the Qv2ray.VERSION.linux-x64.AppImage version.


> <span style="font-size: 1.5rem">:information_source:</span>
 For Ubuntu 19.04 / Debian 10 (or greater): <br/>
 `qv2ray_VERSION_amd64.deb` (Moved to [Qv2ray Debian Repository](https://qv2ray.github.io/debian/) since v2.6.1)

 > <span style="font-size: 1.5rem">:information_source:</span> Notes for Linux AppImage users <br/>
 Although we have bundled `glibc` and some basic C++ libraries into the **AppImage** package to support some old but supported distros, moving yourself to a newer version of Distro/OS is strongly recommended.

# **Configuration**

Before proceeding this stage, make sure you have `v2ray` and its asset files installed as instructed in the [installation guide](../README.md#4-v2ray).

1. Open qv2ray and click on preferences.

2. Ensure that **V2Ray Core Executable Path** and **V2Ray Assets Directory** are filled up according to installed v2ray directories (e.g.: `usr/local/bin/v2ray` & `usr/local/share/v2ray` respectively).

3. Next, click on the **Inbound Settings** tab. Ensure that **set system proxy** is checked.

4. If you are familiar with creating connections and subscription groups in similar programs such as Matsuri, Shadowsocks, Nekoray, and V2rayNG, the process here is the same.

