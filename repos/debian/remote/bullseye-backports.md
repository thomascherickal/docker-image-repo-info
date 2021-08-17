## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:3bc592c6df7a2659d16a4f1476698b816e4986c697cf24364c312b4c952ebefa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:f0f65440a4f9c023ab04f1a9e261453ba1265d149a8b6f9327df05ebdae61c25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54915232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c4ba95b6e46d72b7458cbf3177d0add2917bd8c9701be201d5f799d1c61c303`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:23:31 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f193ec645cc959a84e9c576a46d048fd85b77561d50d7f6aa8210fb0488cfef`  
		Last Modified: Tue, 17 Aug 2021 01:29:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:b5f4a3da8c4f6f33fd557756527977bdf28aba65c3e0cbf312f385b3df85c348
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52452468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:954ca127d5f5b4642abd3397e9cf4d10de09d0a5d8c8ddd941de24e50e98ab1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:55:30 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1d3e899706ce4cb5bf0e1bb95a75cf13df42f4c49cb23a4958204bb3669621`  
		Last Modified: Tue, 17 Aug 2021 02:10:42 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:730dc4b877861722620c557f2aa9701f638f28dbf72eba9000c1027eaa25f34d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50107857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f744e3726aaf0a6fe2c0214e7c4822e65bdd53ac144941efed671166c9ae08`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:02:14 GMT
ADD file:e95bfea309b4c4cf7a3a7367d3a3ed606af0f897282dd0e3e2effd01a126625f in / 
# Thu, 22 Jul 2021 02:02:16 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:02:29 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7b19ab02b95dd8c04699b4e2ac6ee9898e2f6813d01c5c529b1e3f2dd356d20f`  
		Last Modified: Thu, 22 Jul 2021 02:14:18 GMT  
		Size: 50.1 MB (50107629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1a3181b67e386e3c2c8e407e9ab7335bb6ec281b8e70036eadc51e8ef0c0c`  
		Last Modified: Thu, 22 Jul 2021 02:14:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:a5764bb45fddafbb4e173a50eada03274126c9f288fb63454b84482bd3c5e4ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53601238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e4eaf516becce4a90cd32d7e9126f4a77425f448884824eaabc60fcb51078c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:45:56 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41198e75d87d040b5bc5b16bbc80739339d60d4e0ec1153aba9ec610e1c35784`  
		Last Modified: Tue, 17 Aug 2021 01:53:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:0a364b50622f671d731c4bd19d7f14893d44b6f2cb942d88e24914d4290efaeb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55922771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d70be8a163ffc0866ba5236c14afd26b6b250fdbc7a7ea5dcc77dc23154220d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:39:59 GMT
ADD file:9a18b2fe412d515e1cddf03975540bdf3800e8016d3f9a11f1540e5a44c1daa3 in / 
# Tue, 17 Aug 2021 01:40:00 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:40:10 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:37481791ac63726d7596e6cc5512ba4153b294411573b617bc05d7179bfa2013`  
		Last Modified: Tue, 17 Aug 2021 01:49:20 GMT  
		Size: 55.9 MB (55922543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4ed89007d8aa5d9e9c22bb8226aea5f878874c517514874955f0f508794ba4`  
		Last Modified: Tue, 17 Aug 2021 01:49:40 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:102438b1ef6f36b830d502b1c397e06b0477fc42866fde6573cf46ef23f5cc1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53167563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80bc2579ff527ccfe06c8dd7b04fb11d10652cfbbe7e9141f61a7d09f448eb3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:11:17 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dc772d05044d3d60d4f33bb101da929d97910793d2c8930907857c17dd9b5a`  
		Last Modified: Tue, 17 Aug 2021 01:19:51 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:cf378442692654f9b5377df5d7005e5a6b2500d78b092a80ad49f9a12ef505f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58816259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94217e07346788cd33dc5f04787d00023bb979600308f2f278b972d04e26179f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:32:52 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd520c4c58e455a675af932063231049b30b7c09e9b0a294439e5c428d3b0f20`  
		Last Modified: Tue, 17 Aug 2021 01:45:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:531056d36a2c134201addce833f531bfd46fb7c0be8ccd789b5db687422ae0d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53194259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c767fada2251ee98b617a2da2facdf757027490a479fab6b2d77d2253c22da81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:48:50 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a973378096ae8a68fc198dae05578d7c77e33d019b3302ef562affb04946c25f`  
		Last Modified: Tue, 17 Aug 2021 01:57:24 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
