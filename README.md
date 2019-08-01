# Disables VirtualBox guest addition's time synchronization feature #

When VirtualBox guest additions are installed in a VirtualBox Virtual Machine
(VM), VirtualBox will set the VM's time to the host's time. In most cases,
this is a useful feature, but not in context of anonymity/privacy, where the
VM's clock is supposed to differ from the host's clock.

VirtualBox's feature would interfere with other network time synchronization
mechanisms, such as sdwdate or bootclockrandomization.

This package contains an init script, that disables this VirtualBox feature.
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

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `vbox-disable-timesync` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`vbox-disable-timesync` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
