## `debian:experimental`

```console
$ docker pull debian@sha256:b7f93024be2919438764a919348668d691d998ff01ed7f2dfaf2071223c29e12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:4a5c3d1d15c062e82d63251d8ffe4e115576ac0b42081626ff5f8a7731cdda47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54902758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cac957c1ff118de9da741ad8f2d022f3d7f999cf356b5648c66b07549b37019`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:50 GMT
ADD file:12f4eb3a1a689858fc32fbe9a7edf8018d61d5193a8ce6658008d7850ee0f5ee in / 
# Wed, 23 Jun 2021 00:22:51 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:05 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9bda09e9e014f65f659ac7608bd89daaf108fd662c413f3497f3ac2a04897de2`  
		Last Modified: Wed, 23 Jun 2021 00:29:38 GMT  
		Size: 54.9 MB (54902539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678b7c1eaad5bd088dff2224dea719d60d484913477fcb7ed7df8ad0c08fc619`  
		Last Modified: Wed, 23 Jun 2021 00:30:05 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:c64add789d1b98db5a790d0d25a675ce0cc1becfbea50ac7f0c17d90f807c5eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52440269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a07bf51988a5815cc91093602f3a9a13a79a4e9599a7f787ffb74de538f9e9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:54:30 GMT
ADD file:4deff0c1d4b5bc3d1481546e8c00ea0bc5bbc7f11eab126c63132c4a89af197d in / 
# Tue, 22 Jun 2021 23:54:33 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:55:01 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6c75627c7ad259b47cd86117095f9d4ecd22dd47930dda21b514a467655d93bc`  
		Last Modified: Wed, 23 Jun 2021 00:09:22 GMT  
		Size: 52.4 MB (52440047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54adfc90ce1bcfb16b8497ca246a0981919822a2fb7e1c978fa287a750519d86`  
		Last Modified: Wed, 23 Jun 2021 00:10:07 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:9df9dd996069a79eb9cc1b5efaf51b52864589f2b7b657be98e8a155a876aefa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50105805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:572681df20dfb572c68f103b50c5e9bb0d95b4e4a662cb0997b46a12c756fa34`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:24:48 GMT
ADD file:046230cc2e63fa920188287620ddab040b933d21b46b9df85a3cb7f9b3aa2a5a in / 
# Wed, 23 Jun 2021 00:24:51 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:25:18 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:bffb8c2ebf2dfa7754b0616fef743c4d36549eeb40af998350f01cdd0acac7b1`  
		Last Modified: Wed, 23 Jun 2021 00:38:56 GMT  
		Size: 50.1 MB (50105588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0612c97b2a42cfb85858057ee17bb6750d8a7bcabd27a86633f7bd82aada0e`  
		Last Modified: Wed, 23 Jun 2021 00:39:36 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:42534fc6140075f483f116750bccc4d97b9afc4d2dc4d3651bcde2e0e7a876c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53586737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b73eaa500fdbfe714a69e1ae5408b9c1250cf5d4ed51ba6c0e4addac9e12dd22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:46 GMT
ADD file:dd7cd376385de15973c0ee3a1c707fbeb104314bbf11fce9e362749f075bcd3d in / 
# Tue, 22 Jun 2021 23:51:46 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:52:01 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c28a889ee822dbb032f1a883bac45829d02d269e860aa024f091853c8b478135`  
		Last Modified: Tue, 22 Jun 2021 23:59:30 GMT  
		Size: 53.6 MB (53586518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18ed9980eb2eaf5db77997c49b52042ad9a3ada37e15e67f0fee44b0f140ab2`  
		Last Modified: Tue, 22 Jun 2021 23:59:59 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:1cbc19d6bb6a6221cf7ed1327bf0810c6076a7599717713d043a9b6f48e42962
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55915136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78f0bd47c2868faa386c9d1f70d04eeeb6a7d61f03c434aa4fa890e00b8a46b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:10 GMT
ADD file:de8ace10ccb419ce96dc4872bae1b80d95e00e4df51cc6dc289afa8498cf225e in / 
# Tue, 22 Jun 2021 23:42:11 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:42:29 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:35f1b1a9f4f54eda9febd1094b401563b0aa59d98ab53225945c2ec3aa631938`  
		Last Modified: Tue, 22 Jun 2021 23:51:11 GMT  
		Size: 55.9 MB (55914912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d578ead7ad6a99dd85ba202ac1adbd140528dd44862490149f9a7c0fe4c3b2`  
		Last Modified: Tue, 22 Jun 2021 23:51:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:1cc866d19fc4b5467a69ad28c5ebd1088631c41e91fa2cea432279390d68efa1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53157331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baa3c871297a146484b451584ea79e3210a878af758f4730fed893fad5a19c17`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:12:17 GMT
ADD file:11ace88a8133b0ff98af72f05571ac3b5686ad22a390e1e9a4d76e7bad58c6aa in / 
# Wed, 23 Jun 2021 00:12:18 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:12:41 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b3baadf12036606e8b0a2459ae29df21b379334a0c3cabb11a651df9626603b8`  
		Last Modified: Wed, 23 Jun 2021 00:20:27 GMT  
		Size: 53.2 MB (53157107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e997ee55fd33fe9ecbf886634f397e4ac06f3d0a46f35fa25482fa6b6ee03`  
		Last Modified: Wed, 23 Jun 2021 00:21:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:7afb718a4930c30b16071cb7eded244efc4364f2019aa3cb1ce6846a7af16ed4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58813078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6558213b04d1a8c9cc07614b7c8c9a901ed2caf97f42d3d0e974b6926ac02f07`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:33:50 GMT
ADD file:84cec57951ba2d65e741a0ca5ba1e21c83a2d63c914204c312710ad13c2af038 in / 
# Wed, 23 Jun 2021 00:33:58 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:34:36 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:52e73d714e5a9f1563927902501d011a91e7a57450c9140fce0e99cffb35c95e`  
		Last Modified: Wed, 23 Jun 2021 00:39:45 GMT  
		Size: 58.8 MB (58812854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed9f9195f47dfd3e86b07366a754f99be6a102025a5fe9f9f4967c21db1830e`  
		Last Modified: Wed, 23 Jun 2021 00:40:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:23d6c10618149c7dc94b0bb028b307e138421da10b48e1b7457c0e8b3de4386e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50393565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6325929aa7af65ea584d16a1a3d6984329be55f6ef828ede0af504f8d7170c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 08 Jul 2021 19:47:37 GMT
ADD file:0c113a26fab6a5608f8bd9f56e001f511b880a7c4c4a3bd7affd1ec069d46fa4 in / 
# Thu, 08 Jul 2021 19:47:40 GMT
CMD ["bash"]
# Thu, 08 Jul 2021 19:50:58 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2ebdfd6f5baa9ec5ca573d31556a766c3e812a0809525b929f1511ea6fd3dd85`  
		Last Modified: Thu, 08 Jul 2021 19:57:33 GMT  
		Size: 50.4 MB (50393335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e7b0b3e34806db22510cb26c6e4543f73ab46bde83a9899b26f80a94a8bb3`  
		Last Modified: Thu, 08 Jul 2021 19:56:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:039d5e80f8fae6eca6124f046fea8615b9b6b2738567721f20d2a9015230dd6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53184199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3554eb2b168ca0fefed23e2b5dea3aa9d2a9d3596cd5838a5a827d709af99b41`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 02:52:18 GMT
ADD file:a1e1619038554ac7a0cdb24cb503b98e595d0acb05f694a8b1a511325e9f7b18 in / 
# Fri, 09 Jul 2021 02:52:21 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 02:52:40 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f5ff7c5b50956a1c59b68faf4cf7a2dd9c0db8d05cc4ea67f1dcb6e327dac346`  
		Last Modified: Tue, 22 Jun 2021 23:47:16 GMT  
		Size: 53.2 MB (53183975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a311f27127f0a4cf7e209b0e729bebaf2f9f02d344e02ac82b0751d8c1cca6d`  
		Last Modified: Fri, 09 Jul 2021 02:56:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
