# Generic Netlink example

This repository contains an example of how to use the Generic Netlink
communication protocol of the Linux Kernel both in kernel space and user space.

For more information read my introductory article
[here](https://www.yaroslavps.com/weblog/genl-intro/); or if you are the
adventurous kind just read the source, it's got plenty of comments :)

## Build and run

### Kernel module

In order to build the kernel module you need to have installed the Linux kernel
headers in your system.

Once you've got the requirements covered just switch to the `ks/` directory and 
`make` it.

If the build completed successfully, you should be able to load the
`genltest.ko` module using insmod.

### User space program

In order to build the program you need to have libnl installed.

Once installed just switch to the `us/` directory and `make` it.

If the build completed successfully, and once you have loaded the aforementioned
`genltest.ko` module, you should be able to run the program `./genltest`.
