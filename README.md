# Signing a Linux Kernel for Secure Boot
A step-by-step guide on how to install and sign a Linux kernel to boot with Secure Boot, because it shouldn't be so hard to have the latest drivers for your machine 

## Table of contents
<!--ts-->
  * [Why](#why)
  * [How](#how)
    * [Installing a Kernel](#Installing-a-Kernel)
    * [Signing a Kernel for Secure Boot](#Signing-a-Kernel-for-Secure-Boot)
<!--te-->

# Why
Hardware vendors, such as Intel, have started to disable features if Secure Boot is not enabled, which could leave a Linux distro completely unable to use integrated graphics. On top of that, some drivers are only now provided through new Kernel releases, so there is no easy way to install the drivers you may need. These problems will be more relevant with laptop installations of Linux.

I spent a long time trying to battle against Secure Boot not letting me install new kernels, because you need to sign them images yourself, and the guides I've found on how to do so tend to be aimed towards system administrators who know more than a general Linux user. So I decided to put a clear step-by-step guide because I think everyone deserves the latest Linux kernels.

# How
To cover the process beginning to end we'll separte the process in two steps: Installing a Kernel, and Signing it for Secure Boot

## Installing a Kernel
First check which kernel version you are currently using with:

```console
uname -r
```

Ubuntu Kernels: 
https://kernel.ubuntu.com/~kernel-ppa/mainline/?C=N;O=D

Put all the downloaded packages into a folder, then within that folder install the downloaded files with:

```console
sudo dpkg -i *.deb
```

## Signing a Kernel for Secure Boot


# References

Here is a list of different sources I got this information from:

Installing Ubuntu Kernels:
https://itsfoss.com/upgrade-linux-kernel-ubuntu/

Signing Kernel:
https://gloveboxes.github.io/Ubuntu-for-Azure-Developers/docs/signing-kernel-for-secure-boot.html


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
