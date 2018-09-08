dhcrelay Docker Image for ARM v7 hf
===================================

A docker image that simply runs dhcrelay on ARM v7 hf, e.g. Raspberry Pi 3.

As DHCP requests are broadcast it's best to create containers with `--net=host`.

For example, this image is useful if you want to use Pi-hole as your DHCP server
but still want to put it's web interface behind a proxy like nginx. Simply use
this image to relay the DHCP requests allowing control over what ports on the
host Pi-hole opens on the host.

The infrastructure for building ARM images on Docker Hub from
[Building ARM containers on any x86 machine, even DockerHub](https://resin.io/blog/building-arm-containers-on-any-x86-machine-even-dockerhub/).
