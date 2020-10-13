<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6`](#varnish6)
-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.6`](#varnish606)
-	[`varnish:6.0.6-1`](#varnish606-1)
-	[`varnish:6.5`](#varnish65)
-	[`varnish:6.5.1`](#varnish651)
-	[`varnish:6.5.1-1`](#varnish651-1)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:stable`](#varnishstable)

## `varnish:6`

```console
$ docker pull varnish@sha256:00632161a7cda1b40d211875daf3ebf171541fb33ef5c9b2a112f32194afe125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:3059c2077201fc5cd6363f3f81c44ae8adad93f2c154f1c89276f24d50f5ac14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76857008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e72a4600a0e93dd7b07513236c622ef06a4acdc0519ccbc25688d961cf5c40ea`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:27 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:28 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:28 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:28 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:28 GMT
CMD []
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2098ab260e42414bf98043b9205e06f62b960b988a9e48247dade07c5a7db72`  
		Last Modified: Tue, 13 Oct 2020 22:19:17 GMT  
		Size: 49.8 MB (49764306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce057018ac767118d0da6a6bd0fadd5e4338a2eed1a481590c859badbb92e790`  
		Last Modified: Tue, 13 Oct 2020 22:19:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:d28c75dbe76f5d3635ce57bfaa01daffefcb381003a09763d75cc74f8117ff49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:cf76ae9945c025e1577943e3b5fba164059499b27a0f104e35790df8af2a1538
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67185645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f74bb83cb1dfefe8c129467971bd6179c7f703b3bafde000f33e3bb12003f22`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:17:36 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 13 Oct 2020 22:17:36 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:00 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:00 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:00 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:01 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:01 GMT
CMD []
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b4a9f788701036eec8d88bfc775a65d78a0ef4d0400e59b8b5a61bb1301983`  
		Last Modified: Tue, 13 Oct 2020 22:18:51 GMT  
		Size: 44.7 MB (44663071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8f0e043d548f453a96c131e536ba650caa2a6e203906ea6d2c65bd20dc388e`  
		Last Modified: Tue, 13 Oct 2020 22:18:41 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6`

```console
$ docker pull varnish@sha256:d28c75dbe76f5d3635ce57bfaa01daffefcb381003a09763d75cc74f8117ff49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6` - linux; amd64

```console
$ docker pull varnish@sha256:cf76ae9945c025e1577943e3b5fba164059499b27a0f104e35790df8af2a1538
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67185645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f74bb83cb1dfefe8c129467971bd6179c7f703b3bafde000f33e3bb12003f22`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:17:36 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 13 Oct 2020 22:17:36 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:00 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:00 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:00 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:01 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:01 GMT
CMD []
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b4a9f788701036eec8d88bfc775a65d78a0ef4d0400e59b8b5a61bb1301983`  
		Last Modified: Tue, 13 Oct 2020 22:18:51 GMT  
		Size: 44.7 MB (44663071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8f0e043d548f453a96c131e536ba650caa2a6e203906ea6d2c65bd20dc388e`  
		Last Modified: Tue, 13 Oct 2020 22:18:41 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6-1`

```console
$ docker pull varnish@sha256:d28c75dbe76f5d3635ce57bfaa01daffefcb381003a09763d75cc74f8117ff49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6-1` - linux; amd64

```console
$ docker pull varnish@sha256:cf76ae9945c025e1577943e3b5fba164059499b27a0f104e35790df8af2a1538
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67185645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f74bb83cb1dfefe8c129467971bd6179c7f703b3bafde000f33e3bb12003f22`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:17:36 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 13 Oct 2020 22:17:36 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:00 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:00 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:00 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:01 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:01 GMT
CMD []
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b4a9f788701036eec8d88bfc775a65d78a0ef4d0400e59b8b5a61bb1301983`  
		Last Modified: Tue, 13 Oct 2020 22:18:51 GMT  
		Size: 44.7 MB (44663071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8f0e043d548f453a96c131e536ba650caa2a6e203906ea6d2c65bd20dc388e`  
		Last Modified: Tue, 13 Oct 2020 22:18:41 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5`

```console
$ docker pull varnish@sha256:00632161a7cda1b40d211875daf3ebf171541fb33ef5c9b2a112f32194afe125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5` - linux; amd64

```console
$ docker pull varnish@sha256:3059c2077201fc5cd6363f3f81c44ae8adad93f2c154f1c89276f24d50f5ac14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76857008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e72a4600a0e93dd7b07513236c622ef06a4acdc0519ccbc25688d961cf5c40ea`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:27 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:28 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:28 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:28 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:28 GMT
CMD []
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2098ab260e42414bf98043b9205e06f62b960b988a9e48247dade07c5a7db72`  
		Last Modified: Tue, 13 Oct 2020 22:19:17 GMT  
		Size: 49.8 MB (49764306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce057018ac767118d0da6a6bd0fadd5e4338a2eed1a481590c859badbb92e790`  
		Last Modified: Tue, 13 Oct 2020 22:19:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1`

```console
$ docker pull varnish@sha256:00632161a7cda1b40d211875daf3ebf171541fb33ef5c9b2a112f32194afe125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1` - linux; amd64

```console
$ docker pull varnish@sha256:3059c2077201fc5cd6363f3f81c44ae8adad93f2c154f1c89276f24d50f5ac14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76857008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e72a4600a0e93dd7b07513236c622ef06a4acdc0519ccbc25688d961cf5c40ea`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:27 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:28 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:28 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:28 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:28 GMT
CMD []
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2098ab260e42414bf98043b9205e06f62b960b988a9e48247dade07c5a7db72`  
		Last Modified: Tue, 13 Oct 2020 22:19:17 GMT  
		Size: 49.8 MB (49764306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce057018ac767118d0da6a6bd0fadd5e4338a2eed1a481590c859badbb92e790`  
		Last Modified: Tue, 13 Oct 2020 22:19:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1-1`

```console
$ docker pull varnish@sha256:00632161a7cda1b40d211875daf3ebf171541fb33ef5c9b2a112f32194afe125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1-1` - linux; amd64

```console
$ docker pull varnish@sha256:3059c2077201fc5cd6363f3f81c44ae8adad93f2c154f1c89276f24d50f5ac14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76857008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e72a4600a0e93dd7b07513236c622ef06a4acdc0519ccbc25688d961cf5c40ea`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:27 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:28 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:28 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:28 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:28 GMT
CMD []
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2098ab260e42414bf98043b9205e06f62b960b988a9e48247dade07c5a7db72`  
		Last Modified: Tue, 13 Oct 2020 22:19:17 GMT  
		Size: 49.8 MB (49764306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce057018ac767118d0da6a6bd0fadd5e4338a2eed1a481590c859badbb92e790`  
		Last Modified: Tue, 13 Oct 2020 22:19:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:00632161a7cda1b40d211875daf3ebf171541fb33ef5c9b2a112f32194afe125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:3059c2077201fc5cd6363f3f81c44ae8adad93f2c154f1c89276f24d50f5ac14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76857008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e72a4600a0e93dd7b07513236c622ef06a4acdc0519ccbc25688d961cf5c40ea`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:27 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:28 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:28 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:28 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:28 GMT
CMD []
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2098ab260e42414bf98043b9205e06f62b960b988a9e48247dade07c5a7db72`  
		Last Modified: Tue, 13 Oct 2020 22:19:17 GMT  
		Size: 49.8 MB (49764306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce057018ac767118d0da6a6bd0fadd5e4338a2eed1a481590c859badbb92e790`  
		Last Modified: Tue, 13 Oct 2020 22:19:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:00632161a7cda1b40d211875daf3ebf171541fb33ef5c9b2a112f32194afe125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:3059c2077201fc5cd6363f3f81c44ae8adad93f2c154f1c89276f24d50f5ac14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76857008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e72a4600a0e93dd7b07513236c622ef06a4acdc0519ccbc25688d961cf5c40ea`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:27 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:28 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:28 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:28 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:28 GMT
CMD []
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2098ab260e42414bf98043b9205e06f62b960b988a9e48247dade07c5a7db72`  
		Last Modified: Tue, 13 Oct 2020 22:19:17 GMT  
		Size: 49.8 MB (49764306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce057018ac767118d0da6a6bd0fadd5e4338a2eed1a481590c859badbb92e790`  
		Last Modified: Tue, 13 Oct 2020 22:19:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:d28c75dbe76f5d3635ce57bfaa01daffefcb381003a09763d75cc74f8117ff49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:cf76ae9945c025e1577943e3b5fba164059499b27a0f104e35790df8af2a1538
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67185645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f74bb83cb1dfefe8c129467971bd6179c7f703b3bafde000f33e3bb12003f22`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:17:36 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 13 Oct 2020 22:17:36 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:00 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:00 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:00 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:01 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:01 GMT
CMD []
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b4a9f788701036eec8d88bfc775a65d78a0ef4d0400e59b8b5a61bb1301983`  
		Last Modified: Tue, 13 Oct 2020 22:18:51 GMT  
		Size: 44.7 MB (44663071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8f0e043d548f453a96c131e536ba650caa2a6e203906ea6d2c65bd20dc388e`  
		Last Modified: Tue, 13 Oct 2020 22:18:41 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
