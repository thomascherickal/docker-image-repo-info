<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6`](#varnish6)
-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.8`](#varnish608)
-	[`varnish:6.0.8-1`](#varnish608-1)
-	[`varnish:6.6`](#varnish66)
-	[`varnish:6.6.1`](#varnish661)
-	[`varnish:6.6.1-1`](#varnish661-1)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:stable`](#varnishstable)

## `varnish:6`

```console
$ docker pull varnish@sha256:7361a7ba9cca13fc4786d26994bc37bd59e8fe449cb772d052db250476c96212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:c333a4834a55237ccb476da1b38ef8145fdfb915878ee659ae1aec36053efb68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77067671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cec6fafe5f4bb23bb8b7044ec76de6ffc7411dd6be4685d202fd2935bb7d08a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:40:06 GMT
ENV VARNISH_VERSION=6.6.1-1~buster
# Thu, 22 Jul 2021 14:40:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:40:45 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:40:46 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:40:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:40:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:40:47 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:40:48 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0e487938d5f9dea43f192b931a5eb65ec30ba9e7177d5c332c70ebda5645`  
		Last Modified: Thu, 22 Jul 2021 14:41:56 GMT  
		Size: 49.9 MB (49921177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672ff1a28e3a93efb98a9898a5ff8f19112a536cb2c1003b353a4a0133e42a9`  
		Last Modified: Thu, 22 Jul 2021 14:41:46 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:bdb9ef92c82697407ec199b2904193fd3228b2250fa0170bf27e70dac0a2856d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:7a74c2554680378a2472be151c8bb4824d7633c58b9a7ebf5cba6edb6fdcb222
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76488368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6085ae335c1359f698a4d3ce17c2ff3a25b4f408b20eb765e81d36ecd8cc3f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:36 GMT
ENV VARNISH_VERSION=6.0.8-1~buster
# Thu, 22 Jul 2021 14:39:36 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:39:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:58 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:39:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:39:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:39:59 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:39:59 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29973d6c24cb9984c2b3bf777d847fea53998b94a00c9c591fb6f796b9be7ef1`  
		Last Modified: Thu, 22 Jul 2021 14:41:29 GMT  
		Size: 49.3 MB (49341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fc63e290f7ddb29f150b8a3dc7f7ff896a4ba697cdeefd3c82219b485b7d5a`  
		Last Modified: Thu, 22 Jul 2021 14:41:20 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.8`

```console
$ docker pull varnish@sha256:bdb9ef92c82697407ec199b2904193fd3228b2250fa0170bf27e70dac0a2856d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.0.8` - linux; amd64

```console
$ docker pull varnish@sha256:7a74c2554680378a2472be151c8bb4824d7633c58b9a7ebf5cba6edb6fdcb222
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76488368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6085ae335c1359f698a4d3ce17c2ff3a25b4f408b20eb765e81d36ecd8cc3f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:36 GMT
ENV VARNISH_VERSION=6.0.8-1~buster
# Thu, 22 Jul 2021 14:39:36 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:39:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:58 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:39:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:39:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:39:59 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:39:59 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29973d6c24cb9984c2b3bf777d847fea53998b94a00c9c591fb6f796b9be7ef1`  
		Last Modified: Thu, 22 Jul 2021 14:41:29 GMT  
		Size: 49.3 MB (49341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fc63e290f7ddb29f150b8a3dc7f7ff896a4ba697cdeefd3c82219b485b7d5a`  
		Last Modified: Thu, 22 Jul 2021 14:41:20 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.8-1`

```console
$ docker pull varnish@sha256:bdb9ef92c82697407ec199b2904193fd3228b2250fa0170bf27e70dac0a2856d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.0.8-1` - linux; amd64

```console
$ docker pull varnish@sha256:7a74c2554680378a2472be151c8bb4824d7633c58b9a7ebf5cba6edb6fdcb222
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76488368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6085ae335c1359f698a4d3ce17c2ff3a25b4f408b20eb765e81d36ecd8cc3f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:36 GMT
ENV VARNISH_VERSION=6.0.8-1~buster
# Thu, 22 Jul 2021 14:39:36 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:39:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:58 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:39:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:39:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:39:59 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:39:59 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29973d6c24cb9984c2b3bf777d847fea53998b94a00c9c591fb6f796b9be7ef1`  
		Last Modified: Thu, 22 Jul 2021 14:41:29 GMT  
		Size: 49.3 MB (49341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fc63e290f7ddb29f150b8a3dc7f7ff896a4ba697cdeefd3c82219b485b7d5a`  
		Last Modified: Thu, 22 Jul 2021 14:41:20 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6`

```console
$ docker pull varnish@sha256:7361a7ba9cca13fc4786d26994bc37bd59e8fe449cb772d052db250476c96212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.6` - linux; amd64

```console
$ docker pull varnish@sha256:c333a4834a55237ccb476da1b38ef8145fdfb915878ee659ae1aec36053efb68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77067671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cec6fafe5f4bb23bb8b7044ec76de6ffc7411dd6be4685d202fd2935bb7d08a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:40:06 GMT
ENV VARNISH_VERSION=6.6.1-1~buster
# Thu, 22 Jul 2021 14:40:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:40:45 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:40:46 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:40:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:40:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:40:47 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:40:48 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0e487938d5f9dea43f192b931a5eb65ec30ba9e7177d5c332c70ebda5645`  
		Last Modified: Thu, 22 Jul 2021 14:41:56 GMT  
		Size: 49.9 MB (49921177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672ff1a28e3a93efb98a9898a5ff8f19112a536cb2c1003b353a4a0133e42a9`  
		Last Modified: Thu, 22 Jul 2021 14:41:46 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.1`

```console
$ docker pull varnish@sha256:7361a7ba9cca13fc4786d26994bc37bd59e8fe449cb772d052db250476c96212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.6.1` - linux; amd64

```console
$ docker pull varnish@sha256:c333a4834a55237ccb476da1b38ef8145fdfb915878ee659ae1aec36053efb68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77067671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cec6fafe5f4bb23bb8b7044ec76de6ffc7411dd6be4685d202fd2935bb7d08a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:40:06 GMT
ENV VARNISH_VERSION=6.6.1-1~buster
# Thu, 22 Jul 2021 14:40:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:40:45 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:40:46 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:40:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:40:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:40:47 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:40:48 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0e487938d5f9dea43f192b931a5eb65ec30ba9e7177d5c332c70ebda5645`  
		Last Modified: Thu, 22 Jul 2021 14:41:56 GMT  
		Size: 49.9 MB (49921177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672ff1a28e3a93efb98a9898a5ff8f19112a536cb2c1003b353a4a0133e42a9`  
		Last Modified: Thu, 22 Jul 2021 14:41:46 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.1-1`

```console
$ docker pull varnish@sha256:7361a7ba9cca13fc4786d26994bc37bd59e8fe449cb772d052db250476c96212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.6.1-1` - linux; amd64

```console
$ docker pull varnish@sha256:c333a4834a55237ccb476da1b38ef8145fdfb915878ee659ae1aec36053efb68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77067671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cec6fafe5f4bb23bb8b7044ec76de6ffc7411dd6be4685d202fd2935bb7d08a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:40:06 GMT
ENV VARNISH_VERSION=6.6.1-1~buster
# Thu, 22 Jul 2021 14:40:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:40:45 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:40:46 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:40:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:40:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:40:47 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:40:48 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0e487938d5f9dea43f192b931a5eb65ec30ba9e7177d5c332c70ebda5645`  
		Last Modified: Thu, 22 Jul 2021 14:41:56 GMT  
		Size: 49.9 MB (49921177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672ff1a28e3a93efb98a9898a5ff8f19112a536cb2c1003b353a4a0133e42a9`  
		Last Modified: Thu, 22 Jul 2021 14:41:46 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:7361a7ba9cca13fc4786d26994bc37bd59e8fe449cb772d052db250476c96212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:c333a4834a55237ccb476da1b38ef8145fdfb915878ee659ae1aec36053efb68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77067671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cec6fafe5f4bb23bb8b7044ec76de6ffc7411dd6be4685d202fd2935bb7d08a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:40:06 GMT
ENV VARNISH_VERSION=6.6.1-1~buster
# Thu, 22 Jul 2021 14:40:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:40:45 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:40:46 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:40:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:40:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:40:47 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:40:48 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0e487938d5f9dea43f192b931a5eb65ec30ba9e7177d5c332c70ebda5645`  
		Last Modified: Thu, 22 Jul 2021 14:41:56 GMT  
		Size: 49.9 MB (49921177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672ff1a28e3a93efb98a9898a5ff8f19112a536cb2c1003b353a4a0133e42a9`  
		Last Modified: Thu, 22 Jul 2021 14:41:46 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:7361a7ba9cca13fc4786d26994bc37bd59e8fe449cb772d052db250476c96212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:c333a4834a55237ccb476da1b38ef8145fdfb915878ee659ae1aec36053efb68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77067671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cec6fafe5f4bb23bb8b7044ec76de6ffc7411dd6be4685d202fd2935bb7d08a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:40:06 GMT
ENV VARNISH_VERSION=6.6.1-1~buster
# Thu, 22 Jul 2021 14:40:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:40:45 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:40:46 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:40:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:40:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:40:47 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:40:48 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0e487938d5f9dea43f192b931a5eb65ec30ba9e7177d5c332c70ebda5645`  
		Last Modified: Thu, 22 Jul 2021 14:41:56 GMT  
		Size: 49.9 MB (49921177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672ff1a28e3a93efb98a9898a5ff8f19112a536cb2c1003b353a4a0133e42a9`  
		Last Modified: Thu, 22 Jul 2021 14:41:46 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:bdb9ef92c82697407ec199b2904193fd3228b2250fa0170bf27e70dac0a2856d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:7a74c2554680378a2472be151c8bb4824d7633c58b9a7ebf5cba6edb6fdcb222
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76488368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6085ae335c1359f698a4d3ce17c2ff3a25b4f408b20eb765e81d36ecd8cc3f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:36 GMT
ENV VARNISH_VERSION=6.0.8-1~buster
# Thu, 22 Jul 2021 14:39:36 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:39:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:58 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:39:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:39:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:39:59 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:39:59 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29973d6c24cb9984c2b3bf777d847fea53998b94a00c9c591fb6f796b9be7ef1`  
		Last Modified: Thu, 22 Jul 2021 14:41:29 GMT  
		Size: 49.3 MB (49341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fc63e290f7ddb29f150b8a3dc7f7ff896a4ba697cdeefd3c82219b485b7d5a`  
		Last Modified: Thu, 22 Jul 2021 14:41:20 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
