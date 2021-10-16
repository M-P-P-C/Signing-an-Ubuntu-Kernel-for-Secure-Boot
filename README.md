# Signing a Linux Kernel for Secure Boot
A step-by-step guide on how to install and sign a linux kernel to boot with Secure Boot, because it shouldn't be so hard to have the latest drivers for your machine 
<hr>

# Why
Hardware vendors, such as Intel, have started to disable features if Secure Boot is not enabled, which could leave a Linux distro completely unable to use integrated graphics. On top of that, some drivers are only now provided through new Kernel releases, so there is no easy way to intall the drivers you may need. These problems will be more relevant with laptop installations of Linux.

I spent a long time trying to battle against Secure Boot not letting me install new kernels, because you need to sign them images yourself, and the guides I've found on how to do so tend to be aimed towards system administrators who know more than a general Linux user. So I decided to put a clear step-by-step guide because I think everyone deserves the latest Linux kernels.

# How
