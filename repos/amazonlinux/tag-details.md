<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20230207.0`](#amazonlinux20202302070)
-	[`amazonlinux:2.0.20230207.0-with-sources`](#amazonlinux20202302070-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20230207.0`](#amazonlinux2018030202302070)
-	[`amazonlinux:2018.03.0.20230207.0-with-sources`](#amazonlinux2018030202302070-with-sources)
-	[`amazonlinux:2023`](#amazonlinux2023)
-	[`amazonlinux:2023.0.20230222.1`](#amazonlinux20230202302221)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:a329dbd0215bdaa48c4a79fdecc5e1acb855c713548b078a1a852a310b9959ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:435d8b094f1ff1de6f5ca266f8c40fda193a745a2779162a72e06c40efd8e6da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62267134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e27aa8dda477db348e067707a84d1df86660cc87d397a2ad6cd80a8e3b575a8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 10 Feb 2023 18:19:33 GMT
ADD file:f748cf37d9bb118581db4644923fc7f81aeac9af93188e42a5c85bbbba9770f0 in / 
# Fri, 10 Feb 2023 18:19:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:42f354128e7b08a45107942fd4ecc2977b7144b5ec9a6c343c288a99da208911`  
		Last Modified: Fri, 10 Feb 2023 18:20:39 GMT  
		Size: 62.3 MB (62267134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:f6dc1046eb8d41c757177414c99b795644dc61483066dd074bd487fd1ae6971f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:db6f5b872cf347550fbc84997035060cb3f29b4092a502414aea35e1614a58d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515032600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de55c246e0ff336c46024f08fa4c8a76b99da444999c63a7a28e4590eafa6608`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 10 Feb 2023 18:19:33 GMT
ADD file:f748cf37d9bb118581db4644923fc7f81aeac9af93188e42a5c85bbbba9770f0 in / 
# Fri, 10 Feb 2023 18:19:34 GMT
CMD ["/bin/bash"]
# Fri, 10 Feb 2023 18:19:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2f3f7e5ea9b509a345d00531d4b8504f7720dde9cae889e01f4d4e8dbc71db34.tar.gz"     && echo "717d08c398cc28d075ab0ebe75c3785a5277a51c6ab89f5a959b7f1c7d2b98fa  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:42f354128e7b08a45107942fd4ecc2977b7144b5ec9a6c343c288a99da208911`  
		Last Modified: Fri, 10 Feb 2023 18:20:39 GMT  
		Size: 62.3 MB (62267134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c8a964734f86273bdbe5f0d0815e887a76e38d1cdcd222072559d44584cef7`  
		Last Modified: Fri, 10 Feb 2023 18:21:31 GMT  
		Size: 452.8 MB (452765466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:1bed949a5cbe3aa92107828d42f08f33dd2c1f1c46178831b3face787853f628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ea15c2f28f8059473d48fb5c3069ebff7534e729845d605edcc2ebe2df85ba84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62386320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51864d78b86c87b7c81f185ba2b050e79b5108fe7d5e3b5e78eeab383d224ec8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 21:20:09 GMT
ADD file:29cd40b7c56d98385ece53bcbadfefd25bc70ccf0326777986ef6a5720bdfe83 in / 
# Thu, 16 Feb 2023 21:20:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d78505e615251c4f4af6eaa9507b67917d263d23551dcc5a1eed3c012d32a54d`  
		Last Modified: Wed, 15 Feb 2023 00:09:42 GMT  
		Size: 62.4 MB (62386320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:7e0f1977f3d15433efc550cdf216b105e4faa4858ff430a17a2822cef0573831
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (64003805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de8f3ab21e15af79ac81ad63ba143b49d1302ac9d1c7d0f88da5326cd7393323`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 20:39:31 GMT
ADD file:17574026c2754afa903450c59a6d8f7d0905209b174cbe9c13252a61d5a6f916 in / 
# Thu, 16 Feb 2023 20:39:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:71343c2791199c6e2c19c308cff6493497a02f57e225c11405e1934dc7428b3c`  
		Last Modified: Wed, 15 Feb 2023 03:16:17 GMT  
		Size: 64.0 MB (64003805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:c4b2a5f5fb26e7450ea583866daabe17846bf5153dd32f528c87677fabb1e117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3fa69e7667e2798b355efa1cb986e0ce87646a102faef7c1557982eb1b0411fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.7 MB (492732704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5da14082e500f08e79e37c063e3ed02b7a4ddef1a580b553c91045fec60f0146`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 21:20:09 GMT
ADD file:29cd40b7c56d98385ece53bcbadfefd25bc70ccf0326777986ef6a5720bdfe83 in / 
# Thu, 16 Feb 2023 21:20:10 GMT
CMD ["/bin/bash"]
# Thu, 16 Feb 2023 21:20:38 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7e289542d782642b256d8350ebcc22b568c00303c6cedda53c0cc26f5de6cca4.tar.gz"     && echo "28173c8559de7e4838d9ae0e1c163243d6d1274f28d242ced6e7fa44272b36bb  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d78505e615251c4f4af6eaa9507b67917d263d23551dcc5a1eed3c012d32a54d`  
		Last Modified: Wed, 15 Feb 2023 00:09:42 GMT  
		Size: 62.4 MB (62386320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e448b8061a833ba558b9628ae3dc088e3690f1a0c1624d5813333ca0224c06`  
		Last Modified: Thu, 16 Feb 2023 21:21:46 GMT  
		Size: 430.3 MB (430346384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ba3f1afa6fa0103b96d2c2d4a70a860e5e21426cc566d1fba15be4558808f5b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **494.4 MB (494350183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b75bcfc11d633380eb8a00eaa5fbd5672efa3107a1d65f850b71dfea70bf46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 20:39:31 GMT
ADD file:17574026c2754afa903450c59a6d8f7d0905209b174cbe9c13252a61d5a6f916 in / 
# Thu, 16 Feb 2023 20:39:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Feb 2023 20:39:53 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7e289542d782642b256d8350ebcc22b568c00303c6cedda53c0cc26f5de6cca4.tar.gz"     && echo "28173c8559de7e4838d9ae0e1c163243d6d1274f28d242ced6e7fa44272b36bb  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:71343c2791199c6e2c19c308cff6493497a02f57e225c11405e1934dc7428b3c`  
		Last Modified: Wed, 15 Feb 2023 03:16:17 GMT  
		Size: 64.0 MB (64003805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64a7d1a6cba2e41239f96a04c0f08457a2254983add1e7c6f48ed5668abad4b`  
		Last Modified: Thu, 16 Feb 2023 20:40:47 GMT  
		Size: 430.3 MB (430346378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20230207.0`

```console
$ docker pull amazonlinux@sha256:1bed949a5cbe3aa92107828d42f08f33dd2c1f1c46178831b3face787853f628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20230207.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ea15c2f28f8059473d48fb5c3069ebff7534e729845d605edcc2ebe2df85ba84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62386320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51864d78b86c87b7c81f185ba2b050e79b5108fe7d5e3b5e78eeab383d224ec8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 21:20:09 GMT
ADD file:29cd40b7c56d98385ece53bcbadfefd25bc70ccf0326777986ef6a5720bdfe83 in / 
# Thu, 16 Feb 2023 21:20:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d78505e615251c4f4af6eaa9507b67917d263d23551dcc5a1eed3c012d32a54d`  
		Last Modified: Wed, 15 Feb 2023 00:09:42 GMT  
		Size: 62.4 MB (62386320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20230207.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:7e0f1977f3d15433efc550cdf216b105e4faa4858ff430a17a2822cef0573831
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (64003805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de8f3ab21e15af79ac81ad63ba143b49d1302ac9d1c7d0f88da5326cd7393323`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 20:39:31 GMT
ADD file:17574026c2754afa903450c59a6d8f7d0905209b174cbe9c13252a61d5a6f916 in / 
# Thu, 16 Feb 2023 20:39:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:71343c2791199c6e2c19c308cff6493497a02f57e225c11405e1934dc7428b3c`  
		Last Modified: Wed, 15 Feb 2023 03:16:17 GMT  
		Size: 64.0 MB (64003805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20230207.0-with-sources`

```console
$ docker pull amazonlinux@sha256:c4b2a5f5fb26e7450ea583866daabe17846bf5153dd32f528c87677fabb1e117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20230207.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3fa69e7667e2798b355efa1cb986e0ce87646a102faef7c1557982eb1b0411fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.7 MB (492732704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5da14082e500f08e79e37c063e3ed02b7a4ddef1a580b553c91045fec60f0146`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 21:20:09 GMT
ADD file:29cd40b7c56d98385ece53bcbadfefd25bc70ccf0326777986ef6a5720bdfe83 in / 
# Thu, 16 Feb 2023 21:20:10 GMT
CMD ["/bin/bash"]
# Thu, 16 Feb 2023 21:20:38 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7e289542d782642b256d8350ebcc22b568c00303c6cedda53c0cc26f5de6cca4.tar.gz"     && echo "28173c8559de7e4838d9ae0e1c163243d6d1274f28d242ced6e7fa44272b36bb  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d78505e615251c4f4af6eaa9507b67917d263d23551dcc5a1eed3c012d32a54d`  
		Last Modified: Wed, 15 Feb 2023 00:09:42 GMT  
		Size: 62.4 MB (62386320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e448b8061a833ba558b9628ae3dc088e3690f1a0c1624d5813333ca0224c06`  
		Last Modified: Thu, 16 Feb 2023 21:21:46 GMT  
		Size: 430.3 MB (430346384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20230207.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ba3f1afa6fa0103b96d2c2d4a70a860e5e21426cc566d1fba15be4558808f5b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **494.4 MB (494350183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b75bcfc11d633380eb8a00eaa5fbd5672efa3107a1d65f850b71dfea70bf46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 20:39:31 GMT
ADD file:17574026c2754afa903450c59a6d8f7d0905209b174cbe9c13252a61d5a6f916 in / 
# Thu, 16 Feb 2023 20:39:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Feb 2023 20:39:53 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7e289542d782642b256d8350ebcc22b568c00303c6cedda53c0cc26f5de6cca4.tar.gz"     && echo "28173c8559de7e4838d9ae0e1c163243d6d1274f28d242ced6e7fa44272b36bb  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:71343c2791199c6e2c19c308cff6493497a02f57e225c11405e1934dc7428b3c`  
		Last Modified: Wed, 15 Feb 2023 03:16:17 GMT  
		Size: 64.0 MB (64003805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64a7d1a6cba2e41239f96a04c0f08457a2254983add1e7c6f48ed5668abad4b`  
		Last Modified: Thu, 16 Feb 2023 20:40:47 GMT  
		Size: 430.3 MB (430346378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:a329dbd0215bdaa48c4a79fdecc5e1acb855c713548b078a1a852a310b9959ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:435d8b094f1ff1de6f5ca266f8c40fda193a745a2779162a72e06c40efd8e6da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62267134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e27aa8dda477db348e067707a84d1df86660cc87d397a2ad6cd80a8e3b575a8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 10 Feb 2023 18:19:33 GMT
ADD file:f748cf37d9bb118581db4644923fc7f81aeac9af93188e42a5c85bbbba9770f0 in / 
# Fri, 10 Feb 2023 18:19:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:42f354128e7b08a45107942fd4ecc2977b7144b5ec9a6c343c288a99da208911`  
		Last Modified: Fri, 10 Feb 2023 18:20:39 GMT  
		Size: 62.3 MB (62267134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:f6dc1046eb8d41c757177414c99b795644dc61483066dd074bd487fd1ae6971f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:db6f5b872cf347550fbc84997035060cb3f29b4092a502414aea35e1614a58d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515032600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de55c246e0ff336c46024f08fa4c8a76b99da444999c63a7a28e4590eafa6608`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 10 Feb 2023 18:19:33 GMT
ADD file:f748cf37d9bb118581db4644923fc7f81aeac9af93188e42a5c85bbbba9770f0 in / 
# Fri, 10 Feb 2023 18:19:34 GMT
CMD ["/bin/bash"]
# Fri, 10 Feb 2023 18:19:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2f3f7e5ea9b509a345d00531d4b8504f7720dde9cae889e01f4d4e8dbc71db34.tar.gz"     && echo "717d08c398cc28d075ab0ebe75c3785a5277a51c6ab89f5a959b7f1c7d2b98fa  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:42f354128e7b08a45107942fd4ecc2977b7144b5ec9a6c343c288a99da208911`  
		Last Modified: Fri, 10 Feb 2023 18:20:39 GMT  
		Size: 62.3 MB (62267134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c8a964734f86273bdbe5f0d0815e887a76e38d1cdcd222072559d44584cef7`  
		Last Modified: Fri, 10 Feb 2023 18:21:31 GMT  
		Size: 452.8 MB (452765466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20230207.0`

```console
$ docker pull amazonlinux@sha256:a329dbd0215bdaa48c4a79fdecc5e1acb855c713548b078a1a852a310b9959ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20230207.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:435d8b094f1ff1de6f5ca266f8c40fda193a745a2779162a72e06c40efd8e6da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62267134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e27aa8dda477db348e067707a84d1df86660cc87d397a2ad6cd80a8e3b575a8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 10 Feb 2023 18:19:33 GMT
ADD file:f748cf37d9bb118581db4644923fc7f81aeac9af93188e42a5c85bbbba9770f0 in / 
# Fri, 10 Feb 2023 18:19:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:42f354128e7b08a45107942fd4ecc2977b7144b5ec9a6c343c288a99da208911`  
		Last Modified: Fri, 10 Feb 2023 18:20:39 GMT  
		Size: 62.3 MB (62267134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20230207.0-with-sources`

```console
$ docker pull amazonlinux@sha256:f6dc1046eb8d41c757177414c99b795644dc61483066dd074bd487fd1ae6971f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20230207.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:db6f5b872cf347550fbc84997035060cb3f29b4092a502414aea35e1614a58d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515032600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de55c246e0ff336c46024f08fa4c8a76b99da444999c63a7a28e4590eafa6608`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 10 Feb 2023 18:19:33 GMT
ADD file:f748cf37d9bb118581db4644923fc7f81aeac9af93188e42a5c85bbbba9770f0 in / 
# Fri, 10 Feb 2023 18:19:34 GMT
CMD ["/bin/bash"]
# Fri, 10 Feb 2023 18:19:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2f3f7e5ea9b509a345d00531d4b8504f7720dde9cae889e01f4d4e8dbc71db34.tar.gz"     && echo "717d08c398cc28d075ab0ebe75c3785a5277a51c6ab89f5a959b7f1c7d2b98fa  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:42f354128e7b08a45107942fd4ecc2977b7144b5ec9a6c343c288a99da208911`  
		Last Modified: Fri, 10 Feb 2023 18:20:39 GMT  
		Size: 62.3 MB (62267134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c8a964734f86273bdbe5f0d0815e887a76e38d1cdcd222072559d44584cef7`  
		Last Modified: Fri, 10 Feb 2023 18:21:31 GMT  
		Size: 452.8 MB (452765466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2023`

```console
$ docker pull amazonlinux@sha256:ac3826f385e30bf80076d641d74a2a2602a06f5b2068d5f7e9b3734f5f6de173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2023` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:439d1493d4282f5b0100cc0e3402a866c94560d7642e9d83be985874a540d880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56790024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3539e64f7cb7b619497f0d27b9b23341735197bb7dcd7051ba5d1490f5a579`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:44:43 GMT
COPY dir:e18ec8188712eb2ec29f47c38d4bd2b5f601796a4cb5aefa70578b4888aecc1a in / 
# Wed, 01 Mar 2023 01:44:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b4265814d5cf87aa7f7c439c4b75d9938d6fda1cca899224c7895fe095af6f54`  
		Last Modified: Wed, 01 Mar 2023 01:45:13 GMT  
		Size: 56.8 MB (56790024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2023.0.20230222.1`

```console
$ docker pull amazonlinux@sha256:ac3826f385e30bf80076d641d74a2a2602a06f5b2068d5f7e9b3734f5f6de173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2023.0.20230222.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:439d1493d4282f5b0100cc0e3402a866c94560d7642e9d83be985874a540d880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56790024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3539e64f7cb7b619497f0d27b9b23341735197bb7dcd7051ba5d1490f5a579`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:44:43 GMT
COPY dir:e18ec8188712eb2ec29f47c38d4bd2b5f601796a4cb5aefa70578b4888aecc1a in / 
# Wed, 01 Mar 2023 01:44:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b4265814d5cf87aa7f7c439c4b75d9938d6fda1cca899224c7895fe095af6f54`  
		Last Modified: Wed, 01 Mar 2023 01:45:13 GMT  
		Size: 56.8 MB (56790024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:7e5fb59629b04975b55ea922653f37b185ad79828d2a34f9872b84bd2ad9347e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c09be3439eb2f0aa95355fbf59f6c33753f77022ac06e71f9a10507099dd2cde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57916237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2748fd231f3d65fea95fa89d239d40006782a4e865ab98ff4eadead624915d7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:19:36 GMT
ADD file:98ef92cdf32a39d761092e3dbc916e083179c438c365e21a2ea68b801a3f595d in / 
# Thu, 02 Feb 2023 20:19:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:044c2e2e5f7c74ee29fba14bd0c17aba2da682d4bb1f235b6efaeb7365c09814`  
		Last Modified: Thu, 02 Feb 2023 20:20:38 GMT  
		Size: 57.9 MB (57916237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:439d1493d4282f5b0100cc0e3402a866c94560d7642e9d83be985874a540d880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56790024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3539e64f7cb7b619497f0d27b9b23341735197bb7dcd7051ba5d1490f5a579`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:44:43 GMT
COPY dir:e18ec8188712eb2ec29f47c38d4bd2b5f601796a4cb5aefa70578b4888aecc1a in / 
# Wed, 01 Mar 2023 01:44:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b4265814d5cf87aa7f7c439c4b75d9938d6fda1cca899224c7895fe095af6f54`  
		Last Modified: Wed, 01 Mar 2023 01:45:13 GMT  
		Size: 56.8 MB (56790024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:1bed949a5cbe3aa92107828d42f08f33dd2c1f1c46178831b3face787853f628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ea15c2f28f8059473d48fb5c3069ebff7534e729845d605edcc2ebe2df85ba84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62386320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51864d78b86c87b7c81f185ba2b050e79b5108fe7d5e3b5e78eeab383d224ec8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 21:20:09 GMT
ADD file:29cd40b7c56d98385ece53bcbadfefd25bc70ccf0326777986ef6a5720bdfe83 in / 
# Thu, 16 Feb 2023 21:20:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d78505e615251c4f4af6eaa9507b67917d263d23551dcc5a1eed3c012d32a54d`  
		Last Modified: Wed, 15 Feb 2023 00:09:42 GMT  
		Size: 62.4 MB (62386320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:7e0f1977f3d15433efc550cdf216b105e4faa4858ff430a17a2822cef0573831
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (64003805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de8f3ab21e15af79ac81ad63ba143b49d1302ac9d1c7d0f88da5326cd7393323`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 20:39:31 GMT
ADD file:17574026c2754afa903450c59a6d8f7d0905209b174cbe9c13252a61d5a6f916 in / 
# Thu, 16 Feb 2023 20:39:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:71343c2791199c6e2c19c308cff6493497a02f57e225c11405e1934dc7428b3c`  
		Last Modified: Wed, 15 Feb 2023 03:16:17 GMT  
		Size: 64.0 MB (64003805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:c4b2a5f5fb26e7450ea583866daabe17846bf5153dd32f528c87677fabb1e117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3fa69e7667e2798b355efa1cb986e0ce87646a102faef7c1557982eb1b0411fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.7 MB (492732704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5da14082e500f08e79e37c063e3ed02b7a4ddef1a580b553c91045fec60f0146`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 21:20:09 GMT
ADD file:29cd40b7c56d98385ece53bcbadfefd25bc70ccf0326777986ef6a5720bdfe83 in / 
# Thu, 16 Feb 2023 21:20:10 GMT
CMD ["/bin/bash"]
# Thu, 16 Feb 2023 21:20:38 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7e289542d782642b256d8350ebcc22b568c00303c6cedda53c0cc26f5de6cca4.tar.gz"     && echo "28173c8559de7e4838d9ae0e1c163243d6d1274f28d242ced6e7fa44272b36bb  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d78505e615251c4f4af6eaa9507b67917d263d23551dcc5a1eed3c012d32a54d`  
		Last Modified: Wed, 15 Feb 2023 00:09:42 GMT  
		Size: 62.4 MB (62386320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e448b8061a833ba558b9628ae3dc088e3690f1a0c1624d5813333ca0224c06`  
		Last Modified: Thu, 16 Feb 2023 21:21:46 GMT  
		Size: 430.3 MB (430346384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ba3f1afa6fa0103b96d2c2d4a70a860e5e21426cc566d1fba15be4558808f5b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **494.4 MB (494350183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b75bcfc11d633380eb8a00eaa5fbd5672efa3107a1d65f850b71dfea70bf46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Feb 2023 20:39:31 GMT
ADD file:17574026c2754afa903450c59a6d8f7d0905209b174cbe9c13252a61d5a6f916 in / 
# Thu, 16 Feb 2023 20:39:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Feb 2023 20:39:53 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7e289542d782642b256d8350ebcc22b568c00303c6cedda53c0cc26f5de6cca4.tar.gz"     && echo "28173c8559de7e4838d9ae0e1c163243d6d1274f28d242ced6e7fa44272b36bb  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:71343c2791199c6e2c19c308cff6493497a02f57e225c11405e1934dc7428b3c`  
		Last Modified: Wed, 15 Feb 2023 03:16:17 GMT  
		Size: 64.0 MB (64003805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64a7d1a6cba2e41239f96a04c0f08457a2254983add1e7c6f48ed5668abad4b`  
		Last Modified: Thu, 16 Feb 2023 20:40:47 GMT  
		Size: 430.3 MB (430346378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
