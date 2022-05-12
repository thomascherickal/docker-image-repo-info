<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sapmachine`

-	[`sapmachine:11`](#sapmachine11)
-	[`sapmachine:11.0.15.0.1`](#sapmachine1101501)
-	[`sapmachine:17`](#sapmachine17)
-	[`sapmachine:17.0.3.0.1`](#sapmachine170301)
-	[`sapmachine:18`](#sapmachine18)
-	[`sapmachine:18.0.1.1`](#sapmachine18011)
-	[`sapmachine:latest`](#sapmachinelatest)
-	[`sapmachine:lts`](#sapmachinelts)

## `sapmachine:11`

```console
$ docker pull sapmachine@sha256:23b58091ffb81581a508e213c2ff3b4e0401f56460a5183226a706185912c902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:11` - linux; amd64

```console
$ docker pull sapmachine@sha256:1b561a0ee1eb9d4bd8f63b203eaba26efcdd450262637b87f8c36c357ef3a1bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234334243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59c33f11bfb58a6d1ddf28a5269917efdace41b7854a3778e9f85698ef6ab168`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:38:36 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.15.0.1     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:38:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Tue, 03 May 2022 19:38:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc4eda0a38b883dcce4c7c5d68392f244854397ca2f0cfe2a80481822fecc6`  
		Last Modified: Sat, 30 Apr 2022 02:32:08 GMT  
		Size: 7.9 MB (7925575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1ab907437207ea298c496468a3a7baefc0d032c26d763c4a10e7b317993438`  
		Last Modified: Tue, 03 May 2022 19:39:40 GMT  
		Size: 197.8 MB (197842438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:11.0.15.0.1`

```console
$ docker pull sapmachine@sha256:23b58091ffb81581a508e213c2ff3b4e0401f56460a5183226a706185912c902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:11.0.15.0.1` - linux; amd64

```console
$ docker pull sapmachine@sha256:1b561a0ee1eb9d4bd8f63b203eaba26efcdd450262637b87f8c36c357ef3a1bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234334243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59c33f11bfb58a6d1ddf28a5269917efdace41b7854a3778e9f85698ef6ab168`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:38:36 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.15.0.1     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:38:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Tue, 03 May 2022 19:38:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc4eda0a38b883dcce4c7c5d68392f244854397ca2f0cfe2a80481822fecc6`  
		Last Modified: Sat, 30 Apr 2022 02:32:08 GMT  
		Size: 7.9 MB (7925575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1ab907437207ea298c496468a3a7baefc0d032c26d763c4a10e7b317993438`  
		Last Modified: Tue, 03 May 2022 19:39:40 GMT  
		Size: 197.8 MB (197842438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:17`

```console
$ docker pull sapmachine@sha256:3d4106c8ba4586163985a8d565768253299a871a785bc07f256d50a2ea27fb32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:17` - linux; amd64

```console
$ docker pull sapmachine@sha256:21bf4581ae2ccbdbbe1c5501d28ffd7c776cb79b74a11f59a44a8fc1defd626f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234270123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ded1fd173fc5d75f891d4c8ffae5d6183b75fcd42c44a12c14f9819adc2e6d1`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:39:09 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.3.0.1     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:39:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Tue, 03 May 2022 19:39:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc4eda0a38b883dcce4c7c5d68392f244854397ca2f0cfe2a80481822fecc6`  
		Last Modified: Sat, 30 Apr 2022 02:32:08 GMT  
		Size: 7.9 MB (7925575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9535065da1a83b57cd131e4b194a9acbd8512df02ff46edda09de190143145b7`  
		Last Modified: Tue, 03 May 2022 19:40:04 GMT  
		Size: 197.8 MB (197778318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:17.0.3.0.1`

```console
$ docker pull sapmachine@sha256:3d4106c8ba4586163985a8d565768253299a871a785bc07f256d50a2ea27fb32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:17.0.3.0.1` - linux; amd64

```console
$ docker pull sapmachine@sha256:21bf4581ae2ccbdbbe1c5501d28ffd7c776cb79b74a11f59a44a8fc1defd626f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234270123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ded1fd173fc5d75f891d4c8ffae5d6183b75fcd42c44a12c14f9819adc2e6d1`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:39:09 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.3.0.1     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:39:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Tue, 03 May 2022 19:39:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc4eda0a38b883dcce4c7c5d68392f244854397ca2f0cfe2a80481822fecc6`  
		Last Modified: Sat, 30 Apr 2022 02:32:08 GMT  
		Size: 7.9 MB (7925575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9535065da1a83b57cd131e4b194a9acbd8512df02ff46edda09de190143145b7`  
		Last Modified: Tue, 03 May 2022 19:40:04 GMT  
		Size: 197.8 MB (197778318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:18`

```console
$ docker pull sapmachine@sha256:f699d758e5870179290f253c61efc93ea91d3609c43cd22df5a5ad49daac9f9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:18` - linux; amd64

```console
$ docker pull sapmachine@sha256:72414f375beec69b293ad0d8d4605d426c8734141d3a991d6c549aeae1399822
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235239028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa956e139326b1243ff767eefed5e875946f35b357466036e09a86e6dc373446`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:51 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-18-jdk=18.0.1     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-18
# Sat, 30 Apr 2022 02:31:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc4eda0a38b883dcce4c7c5d68392f244854397ca2f0cfe2a80481822fecc6`  
		Last Modified: Sat, 30 Apr 2022 02:32:08 GMT  
		Size: 7.9 MB (7925575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a801e465bd3b79b92cdca8e249ee1037092233426d01992f9377ce16d9b0a3d`  
		Last Modified: Sat, 30 Apr 2022 02:33:13 GMT  
		Size: 198.7 MB (198747223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:18.0.1.1`

```console
$ docker pull sapmachine@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:f699d758e5870179290f253c61efc93ea91d3609c43cd22df5a5ad49daac9f9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:72414f375beec69b293ad0d8d4605d426c8734141d3a991d6c549aeae1399822
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235239028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa956e139326b1243ff767eefed5e875946f35b357466036e09a86e6dc373446`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:51 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-18-jdk=18.0.1     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-18
# Sat, 30 Apr 2022 02:31:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc4eda0a38b883dcce4c7c5d68392f244854397ca2f0cfe2a80481822fecc6`  
		Last Modified: Sat, 30 Apr 2022 02:32:08 GMT  
		Size: 7.9 MB (7925575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a801e465bd3b79b92cdca8e249ee1037092233426d01992f9377ce16d9b0a3d`  
		Last Modified: Sat, 30 Apr 2022 02:33:13 GMT  
		Size: 198.7 MB (198747223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:3d4106c8ba4586163985a8d565768253299a871a785bc07f256d50a2ea27fb32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:21bf4581ae2ccbdbbe1c5501d28ffd7c776cb79b74a11f59a44a8fc1defd626f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234270123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ded1fd173fc5d75f891d4c8ffae5d6183b75fcd42c44a12c14f9819adc2e6d1`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:39:09 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.3.0.1     && rm -rf /var/lib/apt/lists/*
# Tue, 03 May 2022 19:39:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Tue, 03 May 2022 19:39:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc4eda0a38b883dcce4c7c5d68392f244854397ca2f0cfe2a80481822fecc6`  
		Last Modified: Sat, 30 Apr 2022 02:32:08 GMT  
		Size: 7.9 MB (7925575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9535065da1a83b57cd131e4b194a9acbd8512df02ff46edda09de190143145b7`  
		Last Modified: Tue, 03 May 2022 19:40:04 GMT  
		Size: 197.8 MB (197778318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
