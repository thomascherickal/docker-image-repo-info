<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6`](#varnish6)
-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.7`](#varnish607)
-	[`varnish:6.0.7-1`](#varnish607-1)
-	[`varnish:6.6`](#varnish66)
-	[`varnish:6.6.0`](#varnish660)
-	[`varnish:6.6.0-1`](#varnish660-1)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:stable`](#varnishstable)

## `varnish:6`

```console
$ docker pull varnish@sha256:5b41623edd338ef6bb3b456fdfb79a1b60aba64d6d07b9ca5daeb2210f2dc03c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:6c62ea95b142a9edc53f1ded46db96e5f20545c45d0229c922ac63369bf53a29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77066494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e85f5f69a863438e951dee58348e40e869baf7f39fd8383af29ec4133b679`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:43:33 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 12 May 2021 14:43:34 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 May 2021 14:44:03 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:44:04 GMT
WORKDIR /etc/varnish
# Wed, 12 May 2021 14:44:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 May 2021 14:44:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 May 2021 14:44:05 GMT
EXPOSE 80 8443
# Wed, 12 May 2021 14:44:05 GMT
CMD []
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224ea214330d2e152e48627cea86bd9428d64d20c1f8849f762cb47bfa9bdf56`  
		Last Modified: Wed, 12 May 2021 14:44:57 GMT  
		Size: 49.9 MB (49919878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0344adcc19d810ad7826bcf920f21337390c5bab0ca7dea8cc5aac8e88c6c8`  
		Last Modified: Wed, 12 May 2021 14:44:49 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:9308b1705476a5fe67b659e8d3250a66fc9fc6c868e7ed13268d8ffa56eb9e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:772332d6a1d82a34c2f33b90de602d70563f23869db23f100302cef9b6f4b49e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76482138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f8ee11ac6ce7b70dbb30c1cc1e4d3005686bbbb9a7263b26c0e14a01c5a3090`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_SIZE=100M
# Wed, 23 Jun 2021 18:28:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 18:28:11 GMT
WORKDIR /etc/varnish
# Wed, 23 Jun 2021 18:28:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 23 Jun 2021 18:28:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 23 Jun 2021 18:28:11 GMT
EXPOSE 80 8443
# Wed, 23 Jun 2021 18:28:12 GMT
CMD []
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc52b1199388d019eb0f4cf5b62f00b50d816a2fcec674487c20e73e2738c6d`  
		Last Modified: Wed, 23 Jun 2021 18:29:28 GMT  
		Size: 49.3 MB (49335585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e87b33fddabbe2bf5003d04073075a36b0c3a24661cb3cad7bb8bc9d100dd72`  
		Last Modified: Wed, 23 Jun 2021 18:29:19 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7`

```console
$ docker pull varnish@sha256:9308b1705476a5fe67b659e8d3250a66fc9fc6c868e7ed13268d8ffa56eb9e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.0.7` - linux; amd64

```console
$ docker pull varnish@sha256:772332d6a1d82a34c2f33b90de602d70563f23869db23f100302cef9b6f4b49e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76482138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f8ee11ac6ce7b70dbb30c1cc1e4d3005686bbbb9a7263b26c0e14a01c5a3090`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_SIZE=100M
# Wed, 23 Jun 2021 18:28:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 18:28:11 GMT
WORKDIR /etc/varnish
# Wed, 23 Jun 2021 18:28:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 23 Jun 2021 18:28:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 23 Jun 2021 18:28:11 GMT
EXPOSE 80 8443
# Wed, 23 Jun 2021 18:28:12 GMT
CMD []
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc52b1199388d019eb0f4cf5b62f00b50d816a2fcec674487c20e73e2738c6d`  
		Last Modified: Wed, 23 Jun 2021 18:29:28 GMT  
		Size: 49.3 MB (49335585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e87b33fddabbe2bf5003d04073075a36b0c3a24661cb3cad7bb8bc9d100dd72`  
		Last Modified: Wed, 23 Jun 2021 18:29:19 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7-1`

```console
$ docker pull varnish@sha256:9308b1705476a5fe67b659e8d3250a66fc9fc6c868e7ed13268d8ffa56eb9e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.0.7-1` - linux; amd64

```console
$ docker pull varnish@sha256:772332d6a1d82a34c2f33b90de602d70563f23869db23f100302cef9b6f4b49e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76482138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f8ee11ac6ce7b70dbb30c1cc1e4d3005686bbbb9a7263b26c0e14a01c5a3090`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_SIZE=100M
# Wed, 23 Jun 2021 18:28:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 18:28:11 GMT
WORKDIR /etc/varnish
# Wed, 23 Jun 2021 18:28:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 23 Jun 2021 18:28:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 23 Jun 2021 18:28:11 GMT
EXPOSE 80 8443
# Wed, 23 Jun 2021 18:28:12 GMT
CMD []
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc52b1199388d019eb0f4cf5b62f00b50d816a2fcec674487c20e73e2738c6d`  
		Last Modified: Wed, 23 Jun 2021 18:29:28 GMT  
		Size: 49.3 MB (49335585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e87b33fddabbe2bf5003d04073075a36b0c3a24661cb3cad7bb8bc9d100dd72`  
		Last Modified: Wed, 23 Jun 2021 18:29:19 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6`

```console
$ docker pull varnish@sha256:5b41623edd338ef6bb3b456fdfb79a1b60aba64d6d07b9ca5daeb2210f2dc03c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.6` - linux; amd64

```console
$ docker pull varnish@sha256:6c62ea95b142a9edc53f1ded46db96e5f20545c45d0229c922ac63369bf53a29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77066494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e85f5f69a863438e951dee58348e40e869baf7f39fd8383af29ec4133b679`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:43:33 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 12 May 2021 14:43:34 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 May 2021 14:44:03 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:44:04 GMT
WORKDIR /etc/varnish
# Wed, 12 May 2021 14:44:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 May 2021 14:44:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 May 2021 14:44:05 GMT
EXPOSE 80 8443
# Wed, 12 May 2021 14:44:05 GMT
CMD []
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224ea214330d2e152e48627cea86bd9428d64d20c1f8849f762cb47bfa9bdf56`  
		Last Modified: Wed, 12 May 2021 14:44:57 GMT  
		Size: 49.9 MB (49919878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0344adcc19d810ad7826bcf920f21337390c5bab0ca7dea8cc5aac8e88c6c8`  
		Last Modified: Wed, 12 May 2021 14:44:49 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.0`

```console
$ docker pull varnish@sha256:5b41623edd338ef6bb3b456fdfb79a1b60aba64d6d07b9ca5daeb2210f2dc03c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.6.0` - linux; amd64

```console
$ docker pull varnish@sha256:6c62ea95b142a9edc53f1ded46db96e5f20545c45d0229c922ac63369bf53a29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77066494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e85f5f69a863438e951dee58348e40e869baf7f39fd8383af29ec4133b679`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:43:33 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 12 May 2021 14:43:34 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 May 2021 14:44:03 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:44:04 GMT
WORKDIR /etc/varnish
# Wed, 12 May 2021 14:44:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 May 2021 14:44:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 May 2021 14:44:05 GMT
EXPOSE 80 8443
# Wed, 12 May 2021 14:44:05 GMT
CMD []
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224ea214330d2e152e48627cea86bd9428d64d20c1f8849f762cb47bfa9bdf56`  
		Last Modified: Wed, 12 May 2021 14:44:57 GMT  
		Size: 49.9 MB (49919878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0344adcc19d810ad7826bcf920f21337390c5bab0ca7dea8cc5aac8e88c6c8`  
		Last Modified: Wed, 12 May 2021 14:44:49 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.0-1`

```console
$ docker pull varnish@sha256:5b41623edd338ef6bb3b456fdfb79a1b60aba64d6d07b9ca5daeb2210f2dc03c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:6.6.0-1` - linux; amd64

```console
$ docker pull varnish@sha256:6c62ea95b142a9edc53f1ded46db96e5f20545c45d0229c922ac63369bf53a29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77066494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e85f5f69a863438e951dee58348e40e869baf7f39fd8383af29ec4133b679`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:43:33 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 12 May 2021 14:43:34 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 May 2021 14:44:03 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:44:04 GMT
WORKDIR /etc/varnish
# Wed, 12 May 2021 14:44:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 May 2021 14:44:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 May 2021 14:44:05 GMT
EXPOSE 80 8443
# Wed, 12 May 2021 14:44:05 GMT
CMD []
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224ea214330d2e152e48627cea86bd9428d64d20c1f8849f762cb47bfa9bdf56`  
		Last Modified: Wed, 12 May 2021 14:44:57 GMT  
		Size: 49.9 MB (49919878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0344adcc19d810ad7826bcf920f21337390c5bab0ca7dea8cc5aac8e88c6c8`  
		Last Modified: Wed, 12 May 2021 14:44:49 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:5b41623edd338ef6bb3b456fdfb79a1b60aba64d6d07b9ca5daeb2210f2dc03c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:6c62ea95b142a9edc53f1ded46db96e5f20545c45d0229c922ac63369bf53a29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77066494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e85f5f69a863438e951dee58348e40e869baf7f39fd8383af29ec4133b679`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:43:33 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 12 May 2021 14:43:34 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 May 2021 14:44:03 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:44:04 GMT
WORKDIR /etc/varnish
# Wed, 12 May 2021 14:44:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 May 2021 14:44:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 May 2021 14:44:05 GMT
EXPOSE 80 8443
# Wed, 12 May 2021 14:44:05 GMT
CMD []
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224ea214330d2e152e48627cea86bd9428d64d20c1f8849f762cb47bfa9bdf56`  
		Last Modified: Wed, 12 May 2021 14:44:57 GMT  
		Size: 49.9 MB (49919878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0344adcc19d810ad7826bcf920f21337390c5bab0ca7dea8cc5aac8e88c6c8`  
		Last Modified: Wed, 12 May 2021 14:44:49 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:5b41623edd338ef6bb3b456fdfb79a1b60aba64d6d07b9ca5daeb2210f2dc03c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:6c62ea95b142a9edc53f1ded46db96e5f20545c45d0229c922ac63369bf53a29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77066494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e85f5f69a863438e951dee58348e40e869baf7f39fd8383af29ec4133b679`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:43:33 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 12 May 2021 14:43:34 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 May 2021 14:44:03 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:44:04 GMT
WORKDIR /etc/varnish
# Wed, 12 May 2021 14:44:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 May 2021 14:44:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 May 2021 14:44:05 GMT
EXPOSE 80 8443
# Wed, 12 May 2021 14:44:05 GMT
CMD []
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224ea214330d2e152e48627cea86bd9428d64d20c1f8849f762cb47bfa9bdf56`  
		Last Modified: Wed, 12 May 2021 14:44:57 GMT  
		Size: 49.9 MB (49919878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0344adcc19d810ad7826bcf920f21337390c5bab0ca7dea8cc5aac8e88c6c8`  
		Last Modified: Wed, 12 May 2021 14:44:49 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:9308b1705476a5fe67b659e8d3250a66fc9fc6c868e7ed13268d8ffa56eb9e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:772332d6a1d82a34c2f33b90de602d70563f23869db23f100302cef9b6f4b49e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76482138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f8ee11ac6ce7b70dbb30c1cc1e4d3005686bbbb9a7263b26c0e14a01c5a3090`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_SIZE=100M
# Wed, 23 Jun 2021 18:28:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 18:28:11 GMT
WORKDIR /etc/varnish
# Wed, 23 Jun 2021 18:28:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 23 Jun 2021 18:28:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 23 Jun 2021 18:28:11 GMT
EXPOSE 80 8443
# Wed, 23 Jun 2021 18:28:12 GMT
CMD []
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc52b1199388d019eb0f4cf5b62f00b50d816a2fcec674487c20e73e2738c6d`  
		Last Modified: Wed, 23 Jun 2021 18:29:28 GMT  
		Size: 49.3 MB (49335585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e87b33fddabbe2bf5003d04073075a36b0c3a24661cb3cad7bb8bc9d100dd72`  
		Last Modified: Wed, 23 Jun 2021 18:29:19 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
