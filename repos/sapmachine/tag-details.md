<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sapmachine`

-	[`sapmachine:11`](#sapmachine11)
-	[`sapmachine:11.0.17`](#sapmachine11017)
-	[`sapmachine:17`](#sapmachine17)
-	[`sapmachine:17.0.5`](#sapmachine1705)
-	[`sapmachine:19`](#sapmachine19)
-	[`sapmachine:19.0.1`](#sapmachine1901)
-	[`sapmachine:latest`](#sapmachinelatest)
-	[`sapmachine:lts`](#sapmachinelts)

## `sapmachine:11`

```console
$ docker pull sapmachine@sha256:73e35712b03e1478b99888cf917e3babea2d9158cd0c00d7daf9e64ad48e68a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:11` - linux; amd64

```console
$ docker pull sapmachine@sha256:1fe8cdd778e5a340583808012fcf720250b425bf8d073b51a6c854d4ebcf5430
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235114432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0021c73c34a6935392eefea6334b8445b9c282ae3b65352733c2c8dde08a0b5`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:08:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:00 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.17     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Fri, 09 Dec 2022 06:09:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f9829f76f3bad367d27d5bf3e91e6bc0f738874c547c1b6c35ea445acb9f11`  
		Last Modified: Fri, 09 Dec 2022 06:10:29 GMT  
		Size: 7.9 MB (7912181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3254af40efba3734a3c923ae88743bb80a4fac422cba2b175b3771fc0f67b8`  
		Last Modified: Fri, 09 Dec 2022 06:10:42 GMT  
		Size: 198.6 MB (198625369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:11` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:52f6b488c241f550f6f6281468bf6a980c57d5920c75293f87480c1b2d6b40e5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231763548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c74b82342b56ded5952c129fe82c8308c95dadf0b60c9b3a4051a01647ecf9d1`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 23:47:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:26 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.17     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Wed, 11 Jan 2023 23:48:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00c408cc2d94c0e75087f6aa9151688fe5b2714a5acb9a30aaf9ec603b385e`  
		Last Modified: Wed, 11 Jan 2023 23:49:41 GMT  
		Size: 7.8 MB (7754081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5ea7e3d110fbeb5c66b58ebd34929183dddbaf5c23020bbce2754ad72fb8c0`  
		Last Modified: Wed, 11 Jan 2023 23:49:52 GMT  
		Size: 196.8 MB (196816299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:11` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:3d35d84fb581c9025b5759b7d30c6f5be12b1d74efb83b5238ada5fdbd28abda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227408075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9fe0cf3c0ef56a52829b234218b2eb2b2f938cef05a73fa090e4854e399c3c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 00:36:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:38:23 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.17     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:38:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 12 Jan 2023 00:38:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbada04aab656bc06ae2d40eaeb8eb9f9173689e7ed896896e37d12276ef867d`  
		Last Modified: Thu, 12 Jan 2023 00:42:51 GMT  
		Size: 9.3 MB (9312481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9139e6ada8773348351a2e9d56f0cb9d5f2beab86190b6f4b44d2aa87b2391d8`  
		Last Modified: Thu, 12 Jan 2023 00:43:12 GMT  
		Size: 184.8 MB (184796121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:11.0.17`

```console
$ docker pull sapmachine@sha256:73e35712b03e1478b99888cf917e3babea2d9158cd0c00d7daf9e64ad48e68a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:11.0.17` - linux; amd64

```console
$ docker pull sapmachine@sha256:1fe8cdd778e5a340583808012fcf720250b425bf8d073b51a6c854d4ebcf5430
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235114432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0021c73c34a6935392eefea6334b8445b9c282ae3b65352733c2c8dde08a0b5`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:08:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:00 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.17     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Fri, 09 Dec 2022 06:09:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f9829f76f3bad367d27d5bf3e91e6bc0f738874c547c1b6c35ea445acb9f11`  
		Last Modified: Fri, 09 Dec 2022 06:10:29 GMT  
		Size: 7.9 MB (7912181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3254af40efba3734a3c923ae88743bb80a4fac422cba2b175b3771fc0f67b8`  
		Last Modified: Fri, 09 Dec 2022 06:10:42 GMT  
		Size: 198.6 MB (198625369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:11.0.17` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:52f6b488c241f550f6f6281468bf6a980c57d5920c75293f87480c1b2d6b40e5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231763548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c74b82342b56ded5952c129fe82c8308c95dadf0b60c9b3a4051a01647ecf9d1`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 23:47:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:26 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.17     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Wed, 11 Jan 2023 23:48:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00c408cc2d94c0e75087f6aa9151688fe5b2714a5acb9a30aaf9ec603b385e`  
		Last Modified: Wed, 11 Jan 2023 23:49:41 GMT  
		Size: 7.8 MB (7754081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5ea7e3d110fbeb5c66b58ebd34929183dddbaf5c23020bbce2754ad72fb8c0`  
		Last Modified: Wed, 11 Jan 2023 23:49:52 GMT  
		Size: 196.8 MB (196816299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:11.0.17` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:3d35d84fb581c9025b5759b7d30c6f5be12b1d74efb83b5238ada5fdbd28abda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227408075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9fe0cf3c0ef56a52829b234218b2eb2b2f938cef05a73fa090e4854e399c3c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 00:36:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:38:23 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.17     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:38:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 12 Jan 2023 00:38:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbada04aab656bc06ae2d40eaeb8eb9f9173689e7ed896896e37d12276ef867d`  
		Last Modified: Thu, 12 Jan 2023 00:42:51 GMT  
		Size: 9.3 MB (9312481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9139e6ada8773348351a2e9d56f0cb9d5f2beab86190b6f4b44d2aa87b2391d8`  
		Last Modified: Thu, 12 Jan 2023 00:43:12 GMT  
		Size: 184.8 MB (184796121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:17`

```console
$ docker pull sapmachine@sha256:16b5ba43aba88e18bf9c857e0e1aa0aa8032a65f76f60027f17b3dc6b63fc342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:17` - linux; amd64

```console
$ docker pull sapmachine@sha256:a3db9b76311a92ce5e404e46607a74dcea0154fe002ba2bd0d8aadcf700dd7c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234527597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1eff4ffa2d79172bb29b776742a67f0b0b423bab7e330069230954d8580595`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:08:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:38 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Fri, 09 Dec 2022 06:09:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f9829f76f3bad367d27d5bf3e91e6bc0f738874c547c1b6c35ea445acb9f11`  
		Last Modified: Fri, 09 Dec 2022 06:10:29 GMT  
		Size: 7.9 MB (7912181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f782630874769148332fc6cb09cc233f9d28d10d82349f85f85cd9a5e50b80`  
		Last Modified: Fri, 09 Dec 2022 06:11:06 GMT  
		Size: 198.0 MB (198038534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:17` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:30fb409334891779b0124a31467408aae466f9c8f860c3819a2c72d547b2c3cc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (231004756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c247c806137e8c5825cc1f5e0dab5514a744c3751506fde3ec213ff9fd1d9b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 23:47:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:56 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Wed, 11 Jan 2023 23:48:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00c408cc2d94c0e75087f6aa9151688fe5b2714a5acb9a30aaf9ec603b385e`  
		Last Modified: Wed, 11 Jan 2023 23:49:41 GMT  
		Size: 7.8 MB (7754081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a4503e73ad3dbedceded998c6b620c463f436b0f7dce14fc97e80175cb8ccb`  
		Last Modified: Wed, 11 Jan 2023 23:50:14 GMT  
		Size: 196.1 MB (196057507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:17` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:7935a7aa1ce2026f8bf6f52932fd21ed046fc85f6fabc5e6c4c7676a0994586d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.8 MB (240788634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b7591ced004315b74576553b9d7a09e5c5d2e52c43d85636c2fa7f7dd6f779`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 00:36:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:40:00 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:40:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Thu, 12 Jan 2023 00:40:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbada04aab656bc06ae2d40eaeb8eb9f9173689e7ed896896e37d12276ef867d`  
		Last Modified: Thu, 12 Jan 2023 00:42:51 GMT  
		Size: 9.3 MB (9312481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0079af51e1c2c2d114f5378f1338e4186f17292bb3d584ee778696e8c5cf7a8`  
		Last Modified: Thu, 12 Jan 2023 00:43:50 GMT  
		Size: 198.2 MB (198176680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:17.0.5`

```console
$ docker pull sapmachine@sha256:16b5ba43aba88e18bf9c857e0e1aa0aa8032a65f76f60027f17b3dc6b63fc342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:17.0.5` - linux; amd64

```console
$ docker pull sapmachine@sha256:a3db9b76311a92ce5e404e46607a74dcea0154fe002ba2bd0d8aadcf700dd7c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234527597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1eff4ffa2d79172bb29b776742a67f0b0b423bab7e330069230954d8580595`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:08:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:38 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Fri, 09 Dec 2022 06:09:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f9829f76f3bad367d27d5bf3e91e6bc0f738874c547c1b6c35ea445acb9f11`  
		Last Modified: Fri, 09 Dec 2022 06:10:29 GMT  
		Size: 7.9 MB (7912181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f782630874769148332fc6cb09cc233f9d28d10d82349f85f85cd9a5e50b80`  
		Last Modified: Fri, 09 Dec 2022 06:11:06 GMT  
		Size: 198.0 MB (198038534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:17.0.5` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:30fb409334891779b0124a31467408aae466f9c8f860c3819a2c72d547b2c3cc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (231004756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c247c806137e8c5825cc1f5e0dab5514a744c3751506fde3ec213ff9fd1d9b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 23:47:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:56 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Wed, 11 Jan 2023 23:48:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00c408cc2d94c0e75087f6aa9151688fe5b2714a5acb9a30aaf9ec603b385e`  
		Last Modified: Wed, 11 Jan 2023 23:49:41 GMT  
		Size: 7.8 MB (7754081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a4503e73ad3dbedceded998c6b620c463f436b0f7dce14fc97e80175cb8ccb`  
		Last Modified: Wed, 11 Jan 2023 23:50:14 GMT  
		Size: 196.1 MB (196057507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:17.0.5` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:7935a7aa1ce2026f8bf6f52932fd21ed046fc85f6fabc5e6c4c7676a0994586d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.8 MB (240788634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b7591ced004315b74576553b9d7a09e5c5d2e52c43d85636c2fa7f7dd6f779`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 00:36:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:40:00 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:40:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Thu, 12 Jan 2023 00:40:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbada04aab656bc06ae2d40eaeb8eb9f9173689e7ed896896e37d12276ef867d`  
		Last Modified: Thu, 12 Jan 2023 00:42:51 GMT  
		Size: 9.3 MB (9312481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0079af51e1c2c2d114f5378f1338e4186f17292bb3d584ee778696e8c5cf7a8`  
		Last Modified: Thu, 12 Jan 2023 00:43:50 GMT  
		Size: 198.2 MB (198176680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:19`

```console
$ docker pull sapmachine@sha256:a8a6ebf2d2097aecb1b819ffcc5482f446d3462c711ea0cb2678faeca8ebbaf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:19` - linux; amd64

```console
$ docker pull sapmachine@sha256:aa6393748ec415f025e4282ff5eb398cd6741a64df8136f529f77540d7c7fd62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.9 MB (242915807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cab298d94a0719b6257cf47c42c519c450300786c182e52476d7c614bf62e03`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:08:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:10:12 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-19-jdk=19.0.1     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:10:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-19
# Fri, 09 Dec 2022 06:10:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f9829f76f3bad367d27d5bf3e91e6bc0f738874c547c1b6c35ea445acb9f11`  
		Last Modified: Fri, 09 Dec 2022 06:10:29 GMT  
		Size: 7.9 MB (7912181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134b6ef55c3e727e415062aa62a2b3907ca95f3e0b01844b32d31cceb3f30f07`  
		Last Modified: Fri, 09 Dec 2022 06:11:32 GMT  
		Size: 206.4 MB (206426744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:19` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:f1d651e4a331f13080e63b5414c274289f1bb9c922e95236c4df042b170c9e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239495169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ca7c08958b85496a783103dd58c68ea3727dfa86f913f9fecbd47516ff7fdf`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 23:47:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:49:23 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-19-jdk=19.0.1     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:49:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-19
# Wed, 11 Jan 2023 23:49:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00c408cc2d94c0e75087f6aa9151688fe5b2714a5acb9a30aaf9ec603b385e`  
		Last Modified: Wed, 11 Jan 2023 23:49:41 GMT  
		Size: 7.8 MB (7754081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460772f0194dd00f3024b65173124704138f0fae2a00c4b82ef37dc0f2911830`  
		Last Modified: Wed, 11 Jan 2023 23:50:38 GMT  
		Size: 204.5 MB (204547920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:19` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:6a52892e6e43878e76efb4f5edf0aa1e028687688abb3110324f1ff93d389fc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (249044845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:750099c6017783d272865656e3fdaec1ee9f4cf0ec04bb1870bd5b34fb61b81e`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 00:36:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:42:03 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-19-jdk=19.0.1     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:42:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-19
# Thu, 12 Jan 2023 00:42:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbada04aab656bc06ae2d40eaeb8eb9f9173689e7ed896896e37d12276ef867d`  
		Last Modified: Thu, 12 Jan 2023 00:42:51 GMT  
		Size: 9.3 MB (9312481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4ac6ffd286b91e3bbbf5d3f348928d36bf89af10b2c1d6baae63cb757b934`  
		Last Modified: Thu, 12 Jan 2023 00:44:32 GMT  
		Size: 206.4 MB (206432891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:19.0.1`

```console
$ docker pull sapmachine@sha256:a8a6ebf2d2097aecb1b819ffcc5482f446d3462c711ea0cb2678faeca8ebbaf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:19.0.1` - linux; amd64

```console
$ docker pull sapmachine@sha256:aa6393748ec415f025e4282ff5eb398cd6741a64df8136f529f77540d7c7fd62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.9 MB (242915807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cab298d94a0719b6257cf47c42c519c450300786c182e52476d7c614bf62e03`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:08:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:10:12 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-19-jdk=19.0.1     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:10:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-19
# Fri, 09 Dec 2022 06:10:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f9829f76f3bad367d27d5bf3e91e6bc0f738874c547c1b6c35ea445acb9f11`  
		Last Modified: Fri, 09 Dec 2022 06:10:29 GMT  
		Size: 7.9 MB (7912181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134b6ef55c3e727e415062aa62a2b3907ca95f3e0b01844b32d31cceb3f30f07`  
		Last Modified: Fri, 09 Dec 2022 06:11:32 GMT  
		Size: 206.4 MB (206426744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:19.0.1` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:f1d651e4a331f13080e63b5414c274289f1bb9c922e95236c4df042b170c9e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239495169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ca7c08958b85496a783103dd58c68ea3727dfa86f913f9fecbd47516ff7fdf`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 23:47:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:49:23 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-19-jdk=19.0.1     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:49:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-19
# Wed, 11 Jan 2023 23:49:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00c408cc2d94c0e75087f6aa9151688fe5b2714a5acb9a30aaf9ec603b385e`  
		Last Modified: Wed, 11 Jan 2023 23:49:41 GMT  
		Size: 7.8 MB (7754081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460772f0194dd00f3024b65173124704138f0fae2a00c4b82ef37dc0f2911830`  
		Last Modified: Wed, 11 Jan 2023 23:50:38 GMT  
		Size: 204.5 MB (204547920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:19.0.1` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:6a52892e6e43878e76efb4f5edf0aa1e028687688abb3110324f1ff93d389fc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (249044845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:750099c6017783d272865656e3fdaec1ee9f4cf0ec04bb1870bd5b34fb61b81e`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 00:36:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:42:03 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-19-jdk=19.0.1     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:42:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-19
# Thu, 12 Jan 2023 00:42:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbada04aab656bc06ae2d40eaeb8eb9f9173689e7ed896896e37d12276ef867d`  
		Last Modified: Thu, 12 Jan 2023 00:42:51 GMT  
		Size: 9.3 MB (9312481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4ac6ffd286b91e3bbbf5d3f348928d36bf89af10b2c1d6baae63cb757b934`  
		Last Modified: Thu, 12 Jan 2023 00:44:32 GMT  
		Size: 206.4 MB (206432891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:a8a6ebf2d2097aecb1b819ffcc5482f446d3462c711ea0cb2678faeca8ebbaf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:aa6393748ec415f025e4282ff5eb398cd6741a64df8136f529f77540d7c7fd62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.9 MB (242915807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cab298d94a0719b6257cf47c42c519c450300786c182e52476d7c614bf62e03`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:08:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:10:12 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-19-jdk=19.0.1     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:10:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-19
# Fri, 09 Dec 2022 06:10:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f9829f76f3bad367d27d5bf3e91e6bc0f738874c547c1b6c35ea445acb9f11`  
		Last Modified: Fri, 09 Dec 2022 06:10:29 GMT  
		Size: 7.9 MB (7912181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134b6ef55c3e727e415062aa62a2b3907ca95f3e0b01844b32d31cceb3f30f07`  
		Last Modified: Fri, 09 Dec 2022 06:11:32 GMT  
		Size: 206.4 MB (206426744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:latest` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:f1d651e4a331f13080e63b5414c274289f1bb9c922e95236c4df042b170c9e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239495169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ca7c08958b85496a783103dd58c68ea3727dfa86f913f9fecbd47516ff7fdf`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 23:47:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:49:23 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-19-jdk=19.0.1     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:49:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-19
# Wed, 11 Jan 2023 23:49:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00c408cc2d94c0e75087f6aa9151688fe5b2714a5acb9a30aaf9ec603b385e`  
		Last Modified: Wed, 11 Jan 2023 23:49:41 GMT  
		Size: 7.8 MB (7754081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460772f0194dd00f3024b65173124704138f0fae2a00c4b82ef37dc0f2911830`  
		Last Modified: Wed, 11 Jan 2023 23:50:38 GMT  
		Size: 204.5 MB (204547920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:latest` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:6a52892e6e43878e76efb4f5edf0aa1e028687688abb3110324f1ff93d389fc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (249044845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:750099c6017783d272865656e3fdaec1ee9f4cf0ec04bb1870bd5b34fb61b81e`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 00:36:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:42:03 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-19-jdk=19.0.1     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:42:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-19
# Thu, 12 Jan 2023 00:42:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbada04aab656bc06ae2d40eaeb8eb9f9173689e7ed896896e37d12276ef867d`  
		Last Modified: Thu, 12 Jan 2023 00:42:51 GMT  
		Size: 9.3 MB (9312481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4ac6ffd286b91e3bbbf5d3f348928d36bf89af10b2c1d6baae63cb757b934`  
		Last Modified: Thu, 12 Jan 2023 00:44:32 GMT  
		Size: 206.4 MB (206432891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:16b5ba43aba88e18bf9c857e0e1aa0aa8032a65f76f60027f17b3dc6b63fc342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:a3db9b76311a92ce5e404e46607a74dcea0154fe002ba2bd0d8aadcf700dd7c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234527597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1eff4ffa2d79172bb29b776742a67f0b0b423bab7e330069230954d8580595`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:08:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:38 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Fri, 09 Dec 2022 06:09:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f9829f76f3bad367d27d5bf3e91e6bc0f738874c547c1b6c35ea445acb9f11`  
		Last Modified: Fri, 09 Dec 2022 06:10:29 GMT  
		Size: 7.9 MB (7912181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f782630874769148332fc6cb09cc233f9d28d10d82349f85f85cd9a5e50b80`  
		Last Modified: Fri, 09 Dec 2022 06:11:06 GMT  
		Size: 198.0 MB (198038534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:lts` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:30fb409334891779b0124a31467408aae466f9c8f860c3819a2c72d547b2c3cc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (231004756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c247c806137e8c5825cc1f5e0dab5514a744c3751506fde3ec213ff9fd1d9b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 23:47:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:56 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Wed, 11 Jan 2023 23:48:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00c408cc2d94c0e75087f6aa9151688fe5b2714a5acb9a30aaf9ec603b385e`  
		Last Modified: Wed, 11 Jan 2023 23:49:41 GMT  
		Size: 7.8 MB (7754081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a4503e73ad3dbedceded998c6b620c463f436b0f7dce14fc97e80175cb8ccb`  
		Last Modified: Wed, 11 Jan 2023 23:50:14 GMT  
		Size: 196.1 MB (196057507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:lts` - linux; ppc64le

```console
$ docker pull sapmachine@sha256:7935a7aa1ce2026f8bf6f52932fd21ed046fc85f6fabc5e6c4c7676a0994586d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.8 MB (240788634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b7591ced004315b74576553b9d7a09e5c5d2e52c43d85636c2fa7f7dd6f779`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 00:36:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:40:00 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:40:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Thu, 12 Jan 2023 00:40:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbada04aab656bc06ae2d40eaeb8eb9f9173689e7ed896896e37d12276ef867d`  
		Last Modified: Thu, 12 Jan 2023 00:42:51 GMT  
		Size: 9.3 MB (9312481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0079af51e1c2c2d114f5378f1338e4186f17292bb3d584ee778696e8c5cf7a8`  
		Last Modified: Thu, 12 Jan 2023 00:43:50 GMT  
		Size: 198.2 MB (198176680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
