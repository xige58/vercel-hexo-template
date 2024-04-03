---
title: Linux driver for 8814AU
---


### step1 Open a terminal (e.g. Ctrl+Alt+T)

### step2 Update and upgrade system packages

``` bash
$ sudo apt update && sudo apt upgrade
```

### step3 Install the required packages

``` bash
$ sudo apt install -y build-essential dkms git iw
```

### Step 4: Create a directory to hold the downloaded driver

``` bash
$ mkdir -p ~/src
```


### Step 5: Move to the newly created directory

``` bash
$ cd ~/src
```

### Step 6: Download the driver
git clone https://github.com/morrownr/8814au.git

### Step 7: Move to the newly created driver directory
cd ~/src/8814au

### Step 8: Run the installation script (install-driver.sh)

#Example of good situation:

gcc 12.2 (used to compile the kernel)
gcc 12.1 (version of gcc in use)

#To determine the values:

cat /proc/version
gcc --version

sudo apt install gcc-12

sudo ./install-driver.sh or sudo sh install-driver.sh

