<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sapmachine`

-	[`sapmachine:11`](#sapmachine11)
-	[`sapmachine:11.0.15`](#sapmachine11015)
-	[`sapmachine:17`](#sapmachine17)
-	[`sapmachine:17.0.3`](#sapmachine1703)
-	[`sapmachine:18`](#sapmachine18)
-	[`sapmachine:18.0.1`](#sapmachine1801)
-	[`sapmachine:latest`](#sapmachinelatest)
-	[`sapmachine:lts`](#sapmachinelts)

## `sapmachine:11`

```console
$ docker pull sapmachine@sha256:13a0b3326471d8b10258cc64c732583d2e638704cb239ee410a8186f063c5cff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:11` - linux; amd64

```console
$ docker pull sapmachine@sha256:3d371ba6dcec5a3f27ff869abc7690975757ff021041ad50f008600a41c7f9da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234335560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f1e9afc34d2d0bb30e5c50477d32eedb17e62e54102aec88f2f851d30377df`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:30:42 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.15     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:30:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Sat, 30 Apr 2022 02:30:43 GMT
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
	-	`sha256:0240455bf78f176e973152594213b539d9d1d3b5dae47a48c1f3ff0650bd9313`  
		Last Modified: Sat, 30 Apr 2022 02:32:21 GMT  
		Size: 197.8 MB (197843755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:11.0.15`

```console
$ docker pull sapmachine@sha256:13a0b3326471d8b10258cc64c732583d2e638704cb239ee410a8186f063c5cff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:11.0.15` - linux; amd64

```console
$ docker pull sapmachine@sha256:3d371ba6dcec5a3f27ff869abc7690975757ff021041ad50f008600a41c7f9da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234335560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f1e9afc34d2d0bb30e5c50477d32eedb17e62e54102aec88f2f851d30377df`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:30:42 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.15     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:30:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Sat, 30 Apr 2022 02:30:43 GMT
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
	-	`sha256:0240455bf78f176e973152594213b539d9d1d3b5dae47a48c1f3ff0650bd9313`  
		Last Modified: Sat, 30 Apr 2022 02:32:21 GMT  
		Size: 197.8 MB (197843755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:17`

```console
$ docker pull sapmachine@sha256:77de521e810b5e718a0a4ccf38c4ac3e131149e960979d16d5b65ef3f7b7c9ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:17` - linux; amd64

```console
$ docker pull sapmachine@sha256:ddab9afc9608acb12755de08b3b85df859878ed3bd9758af3a2f1d2b3fc83639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234261919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06283a66d4d0867d3dd15507e66e3db2fd864de9bbacaa5cd4419ad2fd294ffc`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:17 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.3     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Sat, 30 Apr 2022 02:31:18 GMT
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
	-	`sha256:5535b1f22dcc4e54d805ff57601dd240bbc9f8b034a1c7dab9d54feb804895f3`  
		Last Modified: Sat, 30 Apr 2022 02:32:46 GMT  
		Size: 197.8 MB (197770114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:17.0.3`

```console
$ docker pull sapmachine@sha256:77de521e810b5e718a0a4ccf38c4ac3e131149e960979d16d5b65ef3f7b7c9ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:17.0.3` - linux; amd64

```console
$ docker pull sapmachine@sha256:ddab9afc9608acb12755de08b3b85df859878ed3bd9758af3a2f1d2b3fc83639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234261919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06283a66d4d0867d3dd15507e66e3db2fd864de9bbacaa5cd4419ad2fd294ffc`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:17 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.3     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Sat, 30 Apr 2022 02:31:18 GMT
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
	-	`sha256:5535b1f22dcc4e54d805ff57601dd240bbc9f8b034a1c7dab9d54feb804895f3`  
		Last Modified: Sat, 30 Apr 2022 02:32:46 GMT  
		Size: 197.8 MB (197770114 bytes)  
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

## `sapmachine:18.0.1`

```console
$ docker pull sapmachine@sha256:f699d758e5870179290f253c61efc93ea91d3609c43cd22df5a5ad49daac9f9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:18.0.1` - linux; amd64

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
$ docker pull sapmachine@sha256:77de521e810b5e718a0a4ccf38c4ac3e131149e960979d16d5b65ef3f7b7c9ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:ddab9afc9608acb12755de08b3b85df859878ed3bd9758af3a2f1d2b3fc83639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234261919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06283a66d4d0867d3dd15507e66e3db2fd864de9bbacaa5cd4419ad2fd294ffc`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:17 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.3     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Sat, 30 Apr 2022 02:31:18 GMT
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
	-	`sha256:5535b1f22dcc4e54d805ff57601dd240bbc9f8b034a1c7dab9d54feb804895f3`  
		Last Modified: Sat, 30 Apr 2022 02:32:46 GMT  
		Size: 197.8 MB (197770114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
