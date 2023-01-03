# Openwrt Docker

[![ci](https://github.com/xpertdev/openwrt-docker/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/xpertdev/openwrt-docker/actions/workflows/docker-publish.yml)

This is a docker container for the [OpenWRT](https://openwrt.org/). Based of [openwrtorg/rootfs](https://hub.docker.com/r/openwrtorg/rootfs)

To build, execute the following command:
```
docker build --rm -f "OpenWRT\Dockerfile" -t openwrt:x86_64 OpenWRT
```
To run, execute the following command:
```
docker run --rm -it -p 2222:22/tcp -p 44343:443/tcp -p 8080:80/tcp --name=openwrt-acevpn openwrt:x86_64
```
Prebuilt image is at https://hub.docker.com/r/acevpn/openwrt
```
docker pull acevpn/openwrt
```
### Tags Supported

* x86_64
* ~~armvirt-32~~
* ~~armvirt-64~~
* ~~arm_cortex-a15_neon-vfpv4~~
* ~~arm_cortex-a9_vfpv3-d16~~
* ~~aarch64_generic~~
* ~~mips_24kc~~
* ~~malta-be~~
* ~~i386_pentium4~~

Questions? Contact [Acevpn](https://www.acevpn.com/)
