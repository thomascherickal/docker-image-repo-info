## `debian:stable-backports`

```console
$ docker pull debian@sha256:c7ab854be73c43465916431d7eb5adbb8b0340c6f1fe920b5d6ba47239db1a68
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
$ docker pull debian@sha256:3728c824b61893dab76332e2b7fbf3d61b6357ac26c121c39cc79f86d54456b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55009459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8422e2ca356a49a14aa03284c57e9cc64fad2044f5eb5e80d7f00122a769e28a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:21:50 GMT
ADD file:31590dd8520f4e157f9874c2f734273f9e7c672ccc50e38d493d7bb0ea12fd06 in / 
# Sat, 28 May 2022 01:21:50 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:21:53 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d257fca7b66eda93f1a2dec168cac0c4be7ba41aaf1ef4cb3666b0207ade1625`  
		Last Modified: Sat, 28 May 2022 01:28:04 GMT  
		Size: 55.0 MB (55009236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513c43cc03e0845f361031deb9295ac2fb8f685b60ee91e0551fe9e0d2e7ddf4`  
		Last Modified: Sat, 28 May 2022 01:28:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:bb6e07ace4b854ef21fe99b99107b86fc8d4672a417d2b747c3b0496671d96ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52476854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36bc40eaa148c61220fa693426bd79f2e10d6e6646554aa9b2effeba47ab2835`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:54:37 GMT
ADD file:6b5d9fb1dcd89975c59319d94c9048759069ec5b363c5f03ab1207358133e06b in / 
# Wed, 11 May 2022 00:54:38 GMT
CMD ["bash"]
# Wed, 11 May 2022 00:54:50 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d2a4feda66e274d3031e4219d93b4c906d0c3a62930ec9636a138434eadeb8c8`  
		Last Modified: Wed, 11 May 2022 01:11:48 GMT  
		Size: 52.5 MB (52476631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d32fc2ee030caf4a5f36e17cd61c5b09d3c56d9536ae51b5fcdb5ff6e8fcec8`  
		Last Modified: Wed, 11 May 2022 01:11:59 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:99fa2729d3dfc25ac6879a50f9e99947a3852c1428d3d02946fb1284a134f6e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50199589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51dd00a0cda3782d3eef4a8dbd7c5006a9c37e1d71baf067c6e39b1fb0aa97d8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:04:16 GMT
ADD file:5996ca40b14395257ee9465f542e325742df193190697f32656a16f82ba8be0f in / 
# Sat, 28 May 2022 01:04:17 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:04:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a629aa7acf7526a04f6b205da1795f21b7636b731d96f0bdcce4354230cccd33`  
		Last Modified: Sat, 28 May 2022 01:20:42 GMT  
		Size: 50.2 MB (50199366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3bac480179da16bbc4852ed461845f3656865dc30a91c0315a4b9fd3d95607`  
		Last Modified: Sat, 28 May 2022 01:20:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:716b2bb6b120704dffba15df825e7db42ba4f2852be5bf65f45bde65b09646a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53697199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6fc3561914206da3df980eaa4da006f6dbeb1954304f6595d7b887bf4aa83d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:42:21 GMT
ADD file:ff1cc52bba4a6a12b43ef4e8dc200d5179b265981e08a3b7a4bd2896ff2a7ff8 in / 
# Sat, 28 May 2022 00:42:22 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:42:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1e2623ac7c4f668298956a826900c9848f8de14a932c41e28bebeb1946741d06`  
		Last Modified: Sat, 28 May 2022 00:50:41 GMT  
		Size: 53.7 MB (53696974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093539695cf6715d7056998ab5d4998d8ae0e2d00368297c24d19896d4077849`  
		Last Modified: Sat, 28 May 2022 00:50:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:47e974cda1beacb1740674d787c00fa3eced7e37bf18634e97031c7b7a65e8b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56008310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31609093e76e3fbf74112fc4db72c28d2160d3befc09f595f13964f0545e11ca`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:41:24 GMT
ADD file:d7f6d5496b54319f0d60f5cdf12d34094f5d33f49f174d4a9f1a7a6509c8057e in / 
# Sat, 28 May 2022 00:41:25 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:41:31 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a3312bca7d30f7a52702aa72d2757cae357a6ee0867338b83f5c368d22451f9d`  
		Last Modified: Sat, 28 May 2022 00:49:50 GMT  
		Size: 56.0 MB (56008089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2e6393c27675df6b06ab3294d8e2318d894c693962012c073112cfd1608291`  
		Last Modified: Sat, 28 May 2022 00:50:00 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:ccadc47d807376c3f29d38280dfc40f0f04ebca251304089cd056c0eda89a50d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53272554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27148cb154704afb08d7ac7ff72e0bb907a8bd300249bc09ae59d0d463728d84`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:15:08 GMT
ADD file:be557b3d74a39c8051f2c00e84687ab16ebd892b36e8082a5ea300cb6bb7ad14 in / 
# Sat, 28 May 2022 01:15:13 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:15:26 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5716b5cfdffd75127dbe0991eff876f003b4eed04041291b556b7b099c1e527d`  
		Last Modified: Sat, 28 May 2022 01:26:01 GMT  
		Size: 53.3 MB (53272331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c532bfb0596dc121c8b023756a1718ca8bb67e2b2e14482c44d28c2201de69b7`  
		Last Modified: Sat, 28 May 2022 01:26:13 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:5ffe7093ac4f95ac6b4f4c11e8f91941ed2e4f3e44d92aa1e64fb5585eaf836f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58902893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78302adefcb237675c0211213c66c5c50053d3c5d2c3cb91801d605eef8c2278`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:25:50 GMT
ADD file:7c27d3f8cd82082cd3b792b3650524a2c8adbc4494d9ad7e6d7ae79b0689ed10 in / 
# Sat, 28 May 2022 01:25:55 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:26:08 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7b10a36258949d27f558770f76e91c58abf97f000104d582f67fbd7d43aa89c0`  
		Last Modified: Sat, 28 May 2022 01:35:32 GMT  
		Size: 58.9 MB (58902668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563df939dcf42236b7ccb739b48a87ed253fd8aa8bbe7914f395d86147cdaf13`  
		Last Modified: Sat, 28 May 2022 01:35:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:546177261b5faaca0d75cde8cd0b7a6a257605088cc3ce8683decb9ace9c10c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53276848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe9370b3eed5fc9f0dbec0216eadcd09a6bd5aa0b4759f846066355a1809087`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:45:06 GMT
ADD file:96522e5ce7a50d833ad67450e3de3d32e9ee12642f0de49a94571afa59294408 in / 
# Sat, 28 May 2022 00:45:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:45:18 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:886de4048c228418dcc85f81c6f97297fe69c74bca502dba5f7fecdacb9f1ec2`  
		Last Modified: Sat, 28 May 2022 00:51:24 GMT  
		Size: 53.3 MB (53276626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0e6e1ebf1fe25c13ccf2b3ed7ef852445c6c9fd0622d4d620b720d7507ba43`  
		Last Modified: Sat, 28 May 2022 00:51:32 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
