<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20220121.0`](#amazonlinux20202201210)
-	[`amazonlinux:2.0.20220121.0-with-sources`](#amazonlinux20202201210-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20220119.1`](#amazonlinux2018030202201191)
-	[`amazonlinux:2018.03.0.20220119.1-with-sources`](#amazonlinux2018030202201191-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20220202.0`](#amazonlinux20220202202020)
-	[`amazonlinux:2022.0.20220202.0-with-sources`](#amazonlinux20220202202020-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:10467da6a94c64e9681f741adad27c46038e702578c925714d607a2c2a64b6f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:920febdad8fa3e59e4e339f18e1c0336edd665dbdaf1d0495e59f1580eb63af6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62391060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228f30e2ad72297512987b009351164c7ba1f430250f2efa9e385c5535b0e348`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Jan 2022 23:41:05 GMT
ADD file:9368a3b891d3811881ac957b51c5d8fbc62e50ac1b36e08e721877da00fcf852 in / 
# Thu, 27 Jan 2022 23:41:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ab4651db2b38ccb9987dbd8f89afc7b18dba5f4886456b9fe2c3f153e0cb1a17`  
		Last Modified: Thu, 27 Jan 2022 23:42:06 GMT  
		Size: 62.4 MB (62391060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:9bf2a0dd0532389209ee16e4d89133c4911580c07d7eb01e3ed1cd6cb3b24cd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:28c2b345fb8c5350946f5ace109f7e6c11db9dcfbf60e3159a2f96de39a86836
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515005681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29dcea5a92f4f38f10147976b572599d1ad45ba854e7970b6900529443342ae4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Jan 2022 23:41:05 GMT
ADD file:9368a3b891d3811881ac957b51c5d8fbc62e50ac1b36e08e721877da00fcf852 in / 
# Thu, 27 Jan 2022 23:41:06 GMT
CMD ["/bin/bash"]
# Thu, 27 Jan 2022 23:41:34 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-130e950e6fd637910aab7091bd642e931a601a4cb070782644264ea9b3283031.tar.gz"  && echo "4c580d08afabb56f120f4b3b310f10858508729953a738b0734d857158c63be5  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ab4651db2b38ccb9987dbd8f89afc7b18dba5f4886456b9fe2c3f153e0cb1a17`  
		Last Modified: Thu, 27 Jan 2022 23:42:06 GMT  
		Size: 62.4 MB (62391060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2bcae1c28206ab057633f715df38b6e8f1700cab1e2a8de3bff04229114e69`  
		Last Modified: Thu, 27 Jan 2022 23:42:40 GMT  
		Size: 452.6 MB (452614621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:f3a37f84f2644095e2c6f6fdf2bf4dbf68d5436c51afcfbfa747a5de391d5d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:a4cfc190f7c549bc8a3f260a8f3af45ddeae63fb10ccad70f914d411aec1e431
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62237845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab2a8d1dc5555599378fc9c5a5661470b0151ed10e3d663a8fbf0b09d6e3d09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f35513003c7129a7bb7870b2e8c67de71757a4c159a9f82d5700ede79e35ffbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63857619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ade329e71d3dc6d7d95d56f9c6d2a1f72b658804fd8ac21a81c4dea5b348968`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 21:33:28 GMT
ADD file:38bb92c68a8a2ac1145ea8d422911f6f0d9c62cccc02b3bdeda096047efecef5 in / 
# Fri, 04 Feb 2022 21:33:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:591d91c97b5df29e14efc53ca38020094df8fa114d32d412bb8f02344aad2411`  
		Last Modified: Fri, 28 Jan 2022 02:04:32 GMT  
		Size: 63.9 MB (63857619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:c2f0c611f77e8ded995da88754355e30443e07c251f4b30d29bf06a7a1b30d0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c2f6a88e3f9cb6221b13a2d961456a081975b936580387b6933cfff6e664af9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.4 MB (485371765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8932d75666cadda98036af5cd135cad7a648d26fc9b62458558ca3b2a56a435`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 23:40:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-86059ff059c15219c13900625367028ea52b1d95d6f6515947fe04983baf9add.tar.gz"  && echo "7cbab49134e393024873c4c8ad4937d84c8b7ed316b4d6260ae6b425cdd89e91  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df40d5f106fd4ab71023a3b15de586ad3165bbec356559856b77c24ad4d33883`  
		Last Modified: Fri, 04 Feb 2022 23:42:04 GMT  
		Size: 423.1 MB (423133920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f58dd8b85d7147b4896f4d240af84876653ff9923fb6cfe0880a74a82297628a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.0 MB (486991491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b947352f3862b8967e6d17d19f985aa482f0f5cb748dd0e5f17e8eba20b60748`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 21:33:28 GMT
ADD file:38bb92c68a8a2ac1145ea8d422911f6f0d9c62cccc02b3bdeda096047efecef5 in / 
# Fri, 04 Feb 2022 21:33:29 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 21:33:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-86059ff059c15219c13900625367028ea52b1d95d6f6515947fe04983baf9add.tar.gz"  && echo "7cbab49134e393024873c4c8ad4937d84c8b7ed316b4d6260ae6b425cdd89e91  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:591d91c97b5df29e14efc53ca38020094df8fa114d32d412bb8f02344aad2411`  
		Last Modified: Fri, 28 Jan 2022 02:04:32 GMT  
		Size: 63.9 MB (63857619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2457150579cd30968d3d34537bde803d2fba631f46f9e31090da275e0b41cb`  
		Last Modified: Fri, 04 Feb 2022 21:35:14 GMT  
		Size: 423.1 MB (423133872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220121.0`

```console
$ docker pull amazonlinux@sha256:f3a37f84f2644095e2c6f6fdf2bf4dbf68d5436c51afcfbfa747a5de391d5d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220121.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:a4cfc190f7c549bc8a3f260a8f3af45ddeae63fb10ccad70f914d411aec1e431
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62237845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab2a8d1dc5555599378fc9c5a5661470b0151ed10e3d663a8fbf0b09d6e3d09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220121.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f35513003c7129a7bb7870b2e8c67de71757a4c159a9f82d5700ede79e35ffbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63857619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ade329e71d3dc6d7d95d56f9c6d2a1f72b658804fd8ac21a81c4dea5b348968`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 21:33:28 GMT
ADD file:38bb92c68a8a2ac1145ea8d422911f6f0d9c62cccc02b3bdeda096047efecef5 in / 
# Fri, 04 Feb 2022 21:33:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:591d91c97b5df29e14efc53ca38020094df8fa114d32d412bb8f02344aad2411`  
		Last Modified: Fri, 28 Jan 2022 02:04:32 GMT  
		Size: 63.9 MB (63857619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220121.0-with-sources`

```console
$ docker pull amazonlinux@sha256:c2f0c611f77e8ded995da88754355e30443e07c251f4b30d29bf06a7a1b30d0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220121.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c2f6a88e3f9cb6221b13a2d961456a081975b936580387b6933cfff6e664af9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.4 MB (485371765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8932d75666cadda98036af5cd135cad7a648d26fc9b62458558ca3b2a56a435`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 23:40:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-86059ff059c15219c13900625367028ea52b1d95d6f6515947fe04983baf9add.tar.gz"  && echo "7cbab49134e393024873c4c8ad4937d84c8b7ed316b4d6260ae6b425cdd89e91  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df40d5f106fd4ab71023a3b15de586ad3165bbec356559856b77c24ad4d33883`  
		Last Modified: Fri, 04 Feb 2022 23:42:04 GMT  
		Size: 423.1 MB (423133920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220121.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f58dd8b85d7147b4896f4d240af84876653ff9923fb6cfe0880a74a82297628a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.0 MB (486991491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b947352f3862b8967e6d17d19f985aa482f0f5cb748dd0e5f17e8eba20b60748`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 21:33:28 GMT
ADD file:38bb92c68a8a2ac1145ea8d422911f6f0d9c62cccc02b3bdeda096047efecef5 in / 
# Fri, 04 Feb 2022 21:33:29 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 21:33:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-86059ff059c15219c13900625367028ea52b1d95d6f6515947fe04983baf9add.tar.gz"  && echo "7cbab49134e393024873c4c8ad4937d84c8b7ed316b4d6260ae6b425cdd89e91  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:591d91c97b5df29e14efc53ca38020094df8fa114d32d412bb8f02344aad2411`  
		Last Modified: Fri, 28 Jan 2022 02:04:32 GMT  
		Size: 63.9 MB (63857619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2457150579cd30968d3d34537bde803d2fba631f46f9e31090da275e0b41cb`  
		Last Modified: Fri, 04 Feb 2022 21:35:14 GMT  
		Size: 423.1 MB (423133872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:10467da6a94c64e9681f741adad27c46038e702578c925714d607a2c2a64b6f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:920febdad8fa3e59e4e339f18e1c0336edd665dbdaf1d0495e59f1580eb63af6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62391060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228f30e2ad72297512987b009351164c7ba1f430250f2efa9e385c5535b0e348`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Jan 2022 23:41:05 GMT
ADD file:9368a3b891d3811881ac957b51c5d8fbc62e50ac1b36e08e721877da00fcf852 in / 
# Thu, 27 Jan 2022 23:41:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ab4651db2b38ccb9987dbd8f89afc7b18dba5f4886456b9fe2c3f153e0cb1a17`  
		Last Modified: Thu, 27 Jan 2022 23:42:06 GMT  
		Size: 62.4 MB (62391060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:9bf2a0dd0532389209ee16e4d89133c4911580c07d7eb01e3ed1cd6cb3b24cd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:28c2b345fb8c5350946f5ace109f7e6c11db9dcfbf60e3159a2f96de39a86836
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515005681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29dcea5a92f4f38f10147976b572599d1ad45ba854e7970b6900529443342ae4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Jan 2022 23:41:05 GMT
ADD file:9368a3b891d3811881ac957b51c5d8fbc62e50ac1b36e08e721877da00fcf852 in / 
# Thu, 27 Jan 2022 23:41:06 GMT
CMD ["/bin/bash"]
# Thu, 27 Jan 2022 23:41:34 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-130e950e6fd637910aab7091bd642e931a601a4cb070782644264ea9b3283031.tar.gz"  && echo "4c580d08afabb56f120f4b3b310f10858508729953a738b0734d857158c63be5  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ab4651db2b38ccb9987dbd8f89afc7b18dba5f4886456b9fe2c3f153e0cb1a17`  
		Last Modified: Thu, 27 Jan 2022 23:42:06 GMT  
		Size: 62.4 MB (62391060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2bcae1c28206ab057633f715df38b6e8f1700cab1e2a8de3bff04229114e69`  
		Last Modified: Thu, 27 Jan 2022 23:42:40 GMT  
		Size: 452.6 MB (452614621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220119.1`

```console
$ docker pull amazonlinux@sha256:10467da6a94c64e9681f741adad27c46038e702578c925714d607a2c2a64b6f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220119.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:920febdad8fa3e59e4e339f18e1c0336edd665dbdaf1d0495e59f1580eb63af6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62391060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228f30e2ad72297512987b009351164c7ba1f430250f2efa9e385c5535b0e348`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Jan 2022 23:41:05 GMT
ADD file:9368a3b891d3811881ac957b51c5d8fbc62e50ac1b36e08e721877da00fcf852 in / 
# Thu, 27 Jan 2022 23:41:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ab4651db2b38ccb9987dbd8f89afc7b18dba5f4886456b9fe2c3f153e0cb1a17`  
		Last Modified: Thu, 27 Jan 2022 23:42:06 GMT  
		Size: 62.4 MB (62391060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220119.1-with-sources`

```console
$ docker pull amazonlinux@sha256:9bf2a0dd0532389209ee16e4d89133c4911580c07d7eb01e3ed1cd6cb3b24cd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220119.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:28c2b345fb8c5350946f5ace109f7e6c11db9dcfbf60e3159a2f96de39a86836
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515005681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29dcea5a92f4f38f10147976b572599d1ad45ba854e7970b6900529443342ae4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Jan 2022 23:41:05 GMT
ADD file:9368a3b891d3811881ac957b51c5d8fbc62e50ac1b36e08e721877da00fcf852 in / 
# Thu, 27 Jan 2022 23:41:06 GMT
CMD ["/bin/bash"]
# Thu, 27 Jan 2022 23:41:34 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-130e950e6fd637910aab7091bd642e931a601a4cb070782644264ea9b3283031.tar.gz"  && echo "4c580d08afabb56f120f4b3b310f10858508729953a738b0734d857158c63be5  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ab4651db2b38ccb9987dbd8f89afc7b18dba5f4886456b9fe2c3f153e0cb1a17`  
		Last Modified: Thu, 27 Jan 2022 23:42:06 GMT  
		Size: 62.4 MB (62391060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2bcae1c28206ab057633f715df38b6e8f1700cab1e2a8de3bff04229114e69`  
		Last Modified: Thu, 27 Jan 2022 23:42:40 GMT  
		Size: 452.6 MB (452614621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

**does not exist** (yet?)

## `amazonlinux:2022-with-sources`

**does not exist** (yet?)

## `amazonlinux:2022.0.20220202.0`

**does not exist** (yet?)

## `amazonlinux:2022.0.20220202.0-with-sources`

**does not exist** (yet?)

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:f3a37f84f2644095e2c6f6fdf2bf4dbf68d5436c51afcfbfa747a5de391d5d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:a4cfc190f7c549bc8a3f260a8f3af45ddeae63fb10ccad70f914d411aec1e431
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62237845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab2a8d1dc5555599378fc9c5a5661470b0151ed10e3d663a8fbf0b09d6e3d09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f35513003c7129a7bb7870b2e8c67de71757a4c159a9f82d5700ede79e35ffbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63857619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ade329e71d3dc6d7d95d56f9c6d2a1f72b658804fd8ac21a81c4dea5b348968`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 21:33:28 GMT
ADD file:38bb92c68a8a2ac1145ea8d422911f6f0d9c62cccc02b3bdeda096047efecef5 in / 
# Fri, 04 Feb 2022 21:33:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:591d91c97b5df29e14efc53ca38020094df8fa114d32d412bb8f02344aad2411`  
		Last Modified: Fri, 28 Jan 2022 02:04:32 GMT  
		Size: 63.9 MB (63857619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:c2f0c611f77e8ded995da88754355e30443e07c251f4b30d29bf06a7a1b30d0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c2f6a88e3f9cb6221b13a2d961456a081975b936580387b6933cfff6e664af9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.4 MB (485371765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8932d75666cadda98036af5cd135cad7a648d26fc9b62458558ca3b2a56a435`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 23:40:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-86059ff059c15219c13900625367028ea52b1d95d6f6515947fe04983baf9add.tar.gz"  && echo "7cbab49134e393024873c4c8ad4937d84c8b7ed316b4d6260ae6b425cdd89e91  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df40d5f106fd4ab71023a3b15de586ad3165bbec356559856b77c24ad4d33883`  
		Last Modified: Fri, 04 Feb 2022 23:42:04 GMT  
		Size: 423.1 MB (423133920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f58dd8b85d7147b4896f4d240af84876653ff9923fb6cfe0880a74a82297628a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.0 MB (486991491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b947352f3862b8967e6d17d19f985aa482f0f5cb748dd0e5f17e8eba20b60748`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 21:33:28 GMT
ADD file:38bb92c68a8a2ac1145ea8d422911f6f0d9c62cccc02b3bdeda096047efecef5 in / 
# Fri, 04 Feb 2022 21:33:29 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 21:33:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-86059ff059c15219c13900625367028ea52b1d95d6f6515947fe04983baf9add.tar.gz"  && echo "7cbab49134e393024873c4c8ad4937d84c8b7ed316b4d6260ae6b425cdd89e91  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:591d91c97b5df29e14efc53ca38020094df8fa114d32d412bb8f02344aad2411`  
		Last Modified: Fri, 28 Jan 2022 02:04:32 GMT  
		Size: 63.9 MB (63857619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2457150579cd30968d3d34537bde803d2fba631f46f9e31090da275e0b41cb`  
		Last Modified: Fri, 04 Feb 2022 21:35:14 GMT  
		Size: 423.1 MB (423133872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
