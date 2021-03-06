# Sets 1024x768 as boot screen resolution #

Ships a /etc/default/grub.d/30_screen_resolution.cfg configuration file, that
injects "vga=0x0317" into the GRUB_CMDLINE_LINUX_DEFAULT variable.

For better usability.

Installing this package in Qubes might cause issues, see:
https://phabricator.whonix.org/T353
This is the only reason why this package is not merged into any other package.
## How to install `grub-screen-resolution` using apt-get ##

1\. Download [Whonix's Signing Key]().

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `grub-screen-resolution`.

```
sudo apt-get install grub-screen-resolution
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/grub-screen-resolution). (Replace `package-name` with the actual name of this package.)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`grub-screen-resolution` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
