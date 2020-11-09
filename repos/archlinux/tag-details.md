<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20201108.0.8567`](#archlinuxbase-2020110808567)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20201108.0.8567`](#archlinuxbase-devel-2020110808567)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:bbb47c4a937fbdf8fffe919864ad638a0228c8da16ffa224d32409270eff6476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:18fef06d6e50bfd37c300c7cf3a0c98d6f7ef0e7b28daff33638513aa4d23802
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.7 MB (150690315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8af7d703d0829db17266ee183e234f283e62a6abc54fd419b9b0bc7f0db59a0`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Wed, 04 Nov 2020 20:20:10 GMT
COPY dir:2c46d626418f4d72d1c32ace0281e7388df32ce589e0bbae07092b59d30a7b6f in / 
# Wed, 04 Nov 2020 20:20:14 GMT
RUN ldconfig && update-ca-trust && locale-gen
# Wed, 04 Nov 2020 20:20:16 GMT
RUN sh -c 'ls usr/lib/sysusers.d/*.conf | /usr/share/libalpm/scripts/systemd-hook sysusers '
# Wed, 04 Nov 2020 20:20:19 GMT
RUN ln -s /usr/lib/os-release /etc/os-release
# Wed, 04 Nov 2020 20:20:32 GMT
RUN pacman-key --init && pacman-key --populate archlinux && bash -c "rm -rf etc/pacman.d/gnupg/{openpgp-revocs.d/,private-keys-v1.d/,pubring.gpg~,gnupg.S.}*"
# Wed, 04 Nov 2020 20:20:32 GMT
ENV LANG=en_US.UTF-8
# Wed, 04 Nov 2020 20:20:32 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:4d6a3daaa4e18d3039017236988f299b0c20686077aa00720754cb913d80c1db`  
		Last Modified: Wed, 04 Nov 2020 20:22:26 GMT  
		Size: 148.2 MB (148167846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b65ac2377d2949ce63400e1530f38a5f427a38bd8c0c9114343f1086f7a89c`  
		Last Modified: Wed, 04 Nov 2020 20:22:02 GMT  
		Size: 1.6 MB (1584815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5a7d9d27127ab0c938966311f16f1a31641ad335de4c52a1955f6bbcfbfb6e`  
		Last Modified: Wed, 04 Nov 2020 20:22:00 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aae39893a70fbb7ca7bbc0856ac4c4ac51f0b5750e76def0a7a09f11d81cc3`  
		Last Modified: Wed, 04 Nov 2020 20:22:00 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d01483340c5b0831ccf76954b6ccedce7cbdfa7a0e9606497c7563b7d47982`  
		Last Modified: Wed, 04 Nov 2020 20:22:00 GMT  
		Size: 936.4 KB (936388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20201108.0.8567`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:93ebac3c3c6aa236aabf50507766ec896a566262abfc1e1354b81c9024136257
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:2de343a5b3be645972cab2c577b294d22819fa3417a5d2d88d682073f2a1ce5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.0 MB (221031956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb0ac01bd73590c415d6d140997078d9193da52bd3bdcde51bde4ccb792e02e`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Wed, 04 Nov 2020 20:21:28 GMT
COPY dir:3bbd6d707516b932ffd619fa524b56af1f1856eba3a59fdadf696785cc6ab9b5 in / 
# Wed, 04 Nov 2020 20:21:32 GMT
RUN ldconfig && update-ca-trust && locale-gen
# Wed, 04 Nov 2020 20:21:33 GMT
RUN sh -c 'ls usr/lib/sysusers.d/*.conf | /usr/share/libalpm/scripts/systemd-hook sysusers '
# Wed, 04 Nov 2020 20:21:34 GMT
RUN ln -s /usr/lib/os-release /etc/os-release
# Wed, 04 Nov 2020 20:21:48 GMT
RUN pacman-key --init && pacman-key --populate archlinux && bash -c "rm -rf etc/pacman.d/gnupg/{openpgp-revocs.d/,private-keys-v1.d/,pubring.gpg~,gnupg.S.}*"
# Wed, 04 Nov 2020 20:21:48 GMT
ENV LANG=en_US.UTF-8
# Wed, 04 Nov 2020 20:21:48 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:dc37e78fa77e6788859b037b93c2651f6f7389bdc7c1609e8fa41fcc1b004d1c`  
		Last Modified: Wed, 04 Nov 2020 20:23:20 GMT  
		Size: 218.5 MB (218509078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc6b3830f30c0bb731f38ebbc84aea9dfe9ba1fef5df8c5e1ce9ed3dc0581b9`  
		Last Modified: Wed, 04 Nov 2020 20:22:33 GMT  
		Size: 1.6 MB (1585223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb3edc663d3925af83e1e3395b95eac3a41be5412e9bf42bb82b7f600d8425a`  
		Last Modified: Wed, 04 Nov 2020 20:22:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6044b7e30446da300b2355d7c33ff02d44afed0f1dc9f1fea08cb990d7793bdf`  
		Last Modified: Wed, 04 Nov 2020 20:22:33 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c925352aecf100bb003b448f54e10ff2f642fb77ad404d8cc536b2cecfb837c`  
		Last Modified: Wed, 04 Nov 2020 20:22:32 GMT  
		Size: 936.4 KB (936391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20201108.0.8567`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:bbb47c4a937fbdf8fffe919864ad638a0228c8da16ffa224d32409270eff6476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:18fef06d6e50bfd37c300c7cf3a0c98d6f7ef0e7b28daff33638513aa4d23802
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.7 MB (150690315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8af7d703d0829db17266ee183e234f283e62a6abc54fd419b9b0bc7f0db59a0`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Wed, 04 Nov 2020 20:20:10 GMT
COPY dir:2c46d626418f4d72d1c32ace0281e7388df32ce589e0bbae07092b59d30a7b6f in / 
# Wed, 04 Nov 2020 20:20:14 GMT
RUN ldconfig && update-ca-trust && locale-gen
# Wed, 04 Nov 2020 20:20:16 GMT
RUN sh -c 'ls usr/lib/sysusers.d/*.conf | /usr/share/libalpm/scripts/systemd-hook sysusers '
# Wed, 04 Nov 2020 20:20:19 GMT
RUN ln -s /usr/lib/os-release /etc/os-release
# Wed, 04 Nov 2020 20:20:32 GMT
RUN pacman-key --init && pacman-key --populate archlinux && bash -c "rm -rf etc/pacman.d/gnupg/{openpgp-revocs.d/,private-keys-v1.d/,pubring.gpg~,gnupg.S.}*"
# Wed, 04 Nov 2020 20:20:32 GMT
ENV LANG=en_US.UTF-8
# Wed, 04 Nov 2020 20:20:32 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:4d6a3daaa4e18d3039017236988f299b0c20686077aa00720754cb913d80c1db`  
		Last Modified: Wed, 04 Nov 2020 20:22:26 GMT  
		Size: 148.2 MB (148167846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b65ac2377d2949ce63400e1530f38a5f427a38bd8c0c9114343f1086f7a89c`  
		Last Modified: Wed, 04 Nov 2020 20:22:02 GMT  
		Size: 1.6 MB (1584815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5a7d9d27127ab0c938966311f16f1a31641ad335de4c52a1955f6bbcfbfb6e`  
		Last Modified: Wed, 04 Nov 2020 20:22:00 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aae39893a70fbb7ca7bbc0856ac4c4ac51f0b5750e76def0a7a09f11d81cc3`  
		Last Modified: Wed, 04 Nov 2020 20:22:00 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d01483340c5b0831ccf76954b6ccedce7cbdfa7a0e9606497c7563b7d47982`  
		Last Modified: Wed, 04 Nov 2020 20:22:00 GMT  
		Size: 936.4 KB (936388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
