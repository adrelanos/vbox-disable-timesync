# Disables VirtualBox guest addition's time synchronization feature #

When VirtualBox guest additions are installed in a VirtualBox Virtual Machine
(VM), VirtualBox will set the VM's time to the host's time. In most cases,
this is a useful feature, but not in context of anonymity/privacy, where the
VM's clock is supposed to differ from the host's clock.

VirtualBox's feature would interfere with other network time synchronization
mechanisms, such as sdwdate or bootclockrandomization.

This package contains an init script, that disables this VirtualBox feature.
## How to install `vbox-disable-timesync` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org buster main" | sudo tee /etc/apt/sources.list.d/whonix.list
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

## Payments ##

`vbox-disable-timesync` requires [payments](https://www.whonix.org/wiki/Payments) to stay alive!
