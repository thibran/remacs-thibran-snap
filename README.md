Remacs Snap Package
===================

[Remacs Repo](https://github.com/Wilfred/remacs)


The snap should be build on an Ubuntu 16.04 host.

Build Steps:
------------

Install Snapcraft:

    sudo snap install --classic snapcraft


To build the snap, run inside the `remacs-thibran-snap` folder:

    snapcraft


To install the snap-package:

    sudo snap install remacs-thibran_*.snap --classic --dangerous

The `--dangerous` is necessary because the local build snap is not signed by the snap-store.

Run
---

To ignore `.emacs.d`, start the snap with `-q`:

    remacs-thibran.remacs -q

Note: Starting a snap for the first time is takes a bit longer than succeeding launches.

Links
=====

[Snapcraft Docs](https://docs.snapcraft.io/)  
[Snap Build Service](https://build.snapcraft.io/)  
[About Snaps](https://www.ubuntu.com/desktop/snappy)