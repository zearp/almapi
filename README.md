# Alma Linux 10 for unsupported Raspberry Pi's

Currently only tested on a 3b but will do testing on other 64bit models that are no longer or not supported at all supported by Alma Linux themselves.

Building needs to be done on an arm64 host. Unltil ```appliance-tools``` is available for EL10 building has to be done on an EL9 distro. Default login and password are ```almalinux``` and sudo is enabled for it.

## Prep
```
dnf -y install git appliance-tools
```

## Usage
Clone the repo:
```
git clone https://github.com/zearp/almapi && cd almapi
```

Edit the kickstart:
```
nano kickstart/pumice.aarch64.ks
```

Built the image:
```
./built pumice
```
The image can be found in the ```pumice-DATE-TIME.aarch64``` folder and can be written to sd card.

## Misc
```
```
