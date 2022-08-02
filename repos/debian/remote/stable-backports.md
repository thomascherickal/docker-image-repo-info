## `debian:stable-backports`

```console
$ docker pull debian@sha256:d8b6cbd33e8961418834f4984c57a75f358e7edc81cb9e432999431afff28136
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:5da3c1908186eda7376c90fe065d3aabfed088048c6730a530aeda08b5500dd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54999645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20555756d69411fe29f657609491c5e61563c9bb7643b32f8b2f887e2659bcf6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:21:28 GMT
ADD file:bcb1ce267ba1b1299bb26cb6b0607643a46a017bfbe8333de7e3a37ae1d16032 in / 
# Tue, 12 Jul 2022 01:21:28 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:21:32 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d6d0c636c9e6d290934ea337ff3ea173a84e6714f24819eaedfd95b85915384a`  
		Last Modified: Tue, 12 Jul 2022 01:26:49 GMT  
		Size: 55.0 MB (54999423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b879d28db041b19736df4f71b35e9d36adcea57909c15d8586cd1ef0c39e8d21`  
		Last Modified: Tue, 12 Jul 2022 01:26:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:2e4e375e31a42409c92e721bc246e9d35a7fc15b9d79151134a8be61e580a91b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52537545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:213c1994138af7cee17fa73022a49f3797038f8162f5a287c8543d3fb750f22e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:50:49 GMT
ADD file:52a6d8229e5ac4dfbb34fe2fb2d592f5568d94577af32ea2f582a7572230cfa0 in / 
# Tue, 02 Aug 2022 00:50:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:50:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bbfa844297afdb04b2d19f686b44257db9d439144828f7cbe63079baa3aff5d3`  
		Last Modified: Tue, 02 Aug 2022 00:59:27 GMT  
		Size: 52.5 MB (52537323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c52e50f26309d44f22c4fa41c3f3dcd0aa0ca0a8d9884e8f1afd413e7ab8ab6`  
		Last Modified: Tue, 02 Aug 2022 00:59:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b18d85fcd3192773f6e7df5598a29a5d50a54fb1e1efd43e0fe2a37b1d9a6d00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50195528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6836a1f6ff0da6511ed459ca2ef4787256dee00385b4a464448d1d07bfeb4137`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:18 GMT
ADD file:87779f497c3b9ebf91ec2cf311358f76f20eb515ed6b183da52c14088803fc85 in / 
# Tue, 02 Aug 2022 01:01:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:01:26 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:08a6bdc1003bf2bd374f4295cb01d1755444f3bd214e75a8369e8e11001cd2c5`  
		Last Modified: Tue, 02 Aug 2022 01:09:46 GMT  
		Size: 50.2 MB (50195306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725e760ab7589c6e9d7d3d54893d6f241831c1e4b4a016b35aa93f2a3f27e42e`  
		Last Modified: Tue, 02 Aug 2022 01:09:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d4f698df794761cbc51e118cf85d98724b23785358a6cae144477f456320d8fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53683259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d68f06b7578157852aed9d7767eb15399c2b2acaee4e885416d5012ba3ea934`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:56 GMT
ADD file:e9e1a80abdd9e28b7a7279be8f171672f11c4eef9f8303a5afed5035269f2a6f in / 
# Tue, 02 Aug 2022 00:41:57 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:42:03 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1d90322913db8b41c2e5aad681509b79eaa89aae0f4060e6101919637809ab74`  
		Last Modified: Tue, 02 Aug 2022 00:48:33 GMT  
		Size: 53.7 MB (53683037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367372a44d75671088f9d16b72e1caf3331192d151be18d11b992993de2ed190`  
		Last Modified: Tue, 02 Aug 2022 00:48:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:429cc1726a0800b1c14a32501d5e3018b5469c2b2f49a3f1f0065f47ad664996
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56002396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1ed227dfc6b371caa03482930d045aaf1e8bd307f4971d0a7d2654d8da816c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:44 GMT
ADD file:9852bd11f2ac634027eacf67314290b88218522fc900a95a2c67c3ba1943dca2 in / 
# Tue, 02 Aug 2022 00:40:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:40:50 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1c092776bb568ebc5f3310d657622e6b172affb770546c2ce1246cec19563507`  
		Last Modified: Tue, 02 Aug 2022 00:47:54 GMT  
		Size: 56.0 MB (56002171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8be317792d3f17016bda83410372f413836b952924b159dc886cb8850c437ab`  
		Last Modified: Tue, 02 Aug 2022 00:48:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:90a04283a91bacfd08fefb1f911456d05801649870a1ae46a7a6321616dfa266
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53263527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3591c0db2ac1fc601fe44b4c7147c22d0d122534c48b30391c0019ffa9dd66f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:45:06 GMT
ADD file:659356a7807ff0035dc510130909c221a049c585036989d0ce9f5027ad89c308 in / 
# Tue, 12 Jul 2022 04:45:12 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:45:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:135d9662eca45a17273c44e35394fd544be26103818019defda5f02b8eff1eb0`  
		Last Modified: Tue, 12 Jul 2022 04:56:08 GMT  
		Size: 53.3 MB (53263302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c831cf32da65d40ca9fb773233e5639424f0681c3925039793df5a66857b6202`  
		Last Modified: Tue, 12 Jul 2022 04:56:18 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:de2489e33bfa65ec99d018ddb35d48e24c5f2e89e2f5dd91322bf92acd13814d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58895907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c00f33b5d5ad91ce4b53e5f1bb92f343f445ce0553eecc59c701ed9db5fdfe43`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:28:16 GMT
ADD file:2212464e195bc1af7220bfadb9e7dee33af051ed5bb42b3f486d9ee2f9d727fd in / 
# Tue, 12 Jul 2022 01:28:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:28:33 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c302b0ef08e182e287cd8cb7c5c504c624efa1c1a0062485cd78ac7062137552`  
		Last Modified: Tue, 12 Jul 2022 01:42:11 GMT  
		Size: 58.9 MB (58895684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605487b5e5ad1284471f735f13c2952efbc3215310aa3d3a74732b32ce522879`  
		Last Modified: Tue, 12 Jul 2022 01:42:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:bf51516b157c351f2311fc080c35b79ae9ea110b37c083734f4ba6db7d08a2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53269505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab285031ddee2b28a86a00262b92845d01c6282d10c58d85fcd5bab5d8559a58`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:43:58 GMT
ADD file:b8eb179ea4633930d534f97a4492919ef0f04b76e64638ca420126e8e6c283de in / 
# Tue, 02 Aug 2022 00:44:01 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:44:07 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:138917c3beea79078118bf931fd764018dee33be43999326d009971680156b4d`  
		Last Modified: Tue, 02 Aug 2022 00:50:22 GMT  
		Size: 53.3 MB (53269283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b38b88b13451f9c034d20a094c4cdea475275588c4e057fd7bf3ca5578cd70`  
		Last Modified: Tue, 02 Aug 2022 00:50:30 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
