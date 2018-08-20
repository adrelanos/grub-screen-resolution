# Sets 1024x768 as boot screen resolution #

Ships a /etc/default/grub.d/30_screen_resolution.cfg configuration file, that
injects "vga=0x0317" into the GRUB_CMDLINE_LINUX_DEFAULT variable.

For better usability.
## How to install `grub-screen-resolution` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org stretch main" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `grub-screen-resolution`.

```
sudo apt-get install grub-screen-resolution
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `grub-screen-resolution` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Payments ##

`grub-screen-resolution` requires [payments](https://www.whonix.org/wiki/Payments) to stay alive!
