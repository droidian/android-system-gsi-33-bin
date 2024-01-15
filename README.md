android-system-gsi-33-bin
=========================

This package ships a pre-built Android 13 GSI (Generic System Image)
so that the Halium initramfs can pick it up during boot.

Why does it matter?
-------------------

Shipping the system image as a package allows to bundle it directly
during rootfs creation.
This essentially removes the need to download a suitable system image
manually.

Furthermore, updates can be then supplied via APT as standard Debian
packages.

Can the system image be overridden?
-----------------------------------

Yes, if you put your `android-rootfs.img` image in /userdata as you
usually would with halium9, you're good to go.
