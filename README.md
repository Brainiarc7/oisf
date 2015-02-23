This is a build of Suricata IDS with support for CUDA toolkit v. 6.5.

In the new toolkit, "sm_10" architecture has been deprectaed, and as such, for suricata (in this repo), I've also deprecated and removed references to "sm_10".

To build this package on Arch Linux, use this PKGBUILD from this gist:

https://gist.github.com/Brainiarc7/3f2c99941d50b53f52e5

Ensure that you copy all files from the Servicefiles directory to the directory where the PKGBUILD is before running makepkg.

Note that this PKGBUILD respects the make flags ($MAKEFLAGS) specified in your /etc/makepkg.conf.

To speed up the build and to generate highly optimized code for your system, tune your make flags as appropriate.

Note that CUDA 6.5 toolkit is required to make this package. See other dependencies in the PKGBUILD


