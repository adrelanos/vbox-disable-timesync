# transitional package #

This is a transitional package.

Can be safely removed.
## How to install `vbox-disable-timesync` using apt-get ##

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

5\. Install `vbox-disable-timesync`.

```
sudo apt-get install vbox-disable-timesync
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/vbox-disable-timesync). (Replace `package-name` with the actual name of this package.)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`vbox-disable-timesync` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
