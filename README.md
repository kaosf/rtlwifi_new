rtlwifi_new
===========

A repo for the newest Realtek rtlwifi codes.

This code will build on any kernel 3.0 and newer. It includes the following drivers:

rtl8192ce, rtl8192se, rtl8192de, rtl8188ee, rtl8192ee, rtl8723ae, rtl8723be, and rtl8821ae.

My notes
========

Environment
-----------

* Ubuntu 14.04.2 amd64
* Linux Kernel 4.0.9-040009-generic (Updated by myself)

### Reference

* [Kernel/MainlineBuilds - Ubuntu Wiki](https://wiki.ubuntu.com/Kernel/MainlineBuilds?action=show&redirect=KernelMainlineBuilds)

How to install
--------------

    make
    sudo make install

`*.ko` files are deployed to `/lib/modules/$KERNEL_VERSION/kernel/net/rtlwifi`.

Default driver files in that directory are backuped by the name of
`backup_drivers.tar`. It keeps absolute path by `P` option of `tar` command.

### References

* `Makefile` in this repository
* [rtl8192ce intermittent connection. / Kernel & Hardware / Arch Linux Forums](https://bbs.archlinux.org/viewtopic.php?id=132931)
