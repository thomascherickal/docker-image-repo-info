## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:6765f1de1cf27fae6b3324e69041efced9d772f95503da396861502642c6d13d
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
$ docker pull debian@sha256:29223aded45ca92f12c719970ab5c42aae68df83c46b39093599cb42b41486ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54927907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db3a1c5e40069f9ae82d036fbec723047f7c89665eed6244e956958fe7d03667`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:22:29 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dae4a85b0ed46e56c415e3482da8fa633a8f47b0e007309d77252511c600ef7`  
		Last Modified: Tue, 28 Sep 2021 01:28:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:b7c927d70f6f61bb258e954b5f122f345f12f58c0548765fc8a59e60bde386da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52462830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c28e73e1376ef734c426b938155f240dc5b02ad3fd14571acd55ddb353af057`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:50:19 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5ed19bf15b455763d6efd2a8d3e6a9710fcd1afa5ef71750b1f84d6ac28cb9`  
		Last Modified: Tue, 28 Sep 2021 02:06:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b25dedbb396dd85738891aa1979bbbd95ac5730760bb2341c51ff8c08b976855
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50128218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064d051c6b9394f3b1e73cc6287ed72273afc824fdf8327ee18143e5963f21de`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 18:02:39 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aed33a6596980fe469cd51dbe80e25d86500951fdbb4d04723a8f1a93bb0b7c`  
		Last Modified: Thu, 30 Sep 2021 18:19:02 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:90c53c04603b72deaab03b592d9011562b4123e08ef8d443921ffcc7cac75cdb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53613823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba1d8795ddff6749cdafc85666fb057aafbe14501ca04c5a08a06c587cbd4a99`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:40:34 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55bf91a68aa3eeda16c1c42c39c000114a33ded2617eee358755a1184bc76a5`  
		Last Modified: Tue, 28 Sep 2021 01:48:13 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:f359ef240325e492797a4bd627333a752101ddc5ff983facbee6b299db74d8dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55932463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aed41a0d70b57cfd9280c8ad50ae9a0a0cd13bf5d04d07e9ff72eb8d1399b73`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:39:55 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648b8798ad6d5a39fcddf3eac777c7c94924500830b0f77145faf04a5f71bcb1`  
		Last Modified: Tue, 28 Sep 2021 01:48:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3319415597cb58bbf2de4416f5ce8d1ee5144ea01e457dfaef7095341e3869f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53178045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffa490dc24483e1a7f4ee3bf595a511f9edaa6259dd4e34419be663de4efc2b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:10:05 GMT
ADD file:fa139347f50faea85a5b3b4670c35cefd41b93de492dc47fcac13844e6ef3fa7 in / 
# Tue, 28 Sep 2021 02:10:06 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:10:16 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8238f36a9a08cb584f6fed203a421c1179967398b18223c38b40a04204650099`  
		Last Modified: Tue, 28 Sep 2021 02:20:00 GMT  
		Size: 53.2 MB (53177818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189566a78d12b6dcc52028012799982f3f011e91965eb66cfe4d803682a1a24`  
		Last Modified: Tue, 28 Sep 2021 02:20:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:fb866c97f9f9a14deb4f9ce33d0d2d2412a954041ae99339f8d4afb797024b86
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58819661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97cb20e3a8b193c742dc4fd6ee7531f3254be626f3fc4bd973aac52842ff9c12`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:22:56 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb86e4144f884b8beaa24436c2083e1476457877dc8cd08b6cea44470ae0d0c`  
		Last Modified: Fri, 03 Sep 2021 01:36:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:45b079bdec0b593bb0e9547a7dcd8a32b1429fea1d8bf2f9674341bf7ca56816
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53202535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79e5f0236f032bdb7181f17aa157743c1d43270f3e5081008cf61f9ea4932720`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:42:47 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ae71f1083a89591ef0422474a0fc359cd7dfd471d67b5c86b2a2dec213fa0e`  
		Last Modified: Tue, 28 Sep 2021 01:48:52 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
