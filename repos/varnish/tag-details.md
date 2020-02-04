<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6`](#varnish6)
-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.5`](#varnish605)
-	[`varnish:6.0.5-1`](#varnish605-1)
-	[`varnish:6.3`](#varnish63)
-	[`varnish:6.3.1`](#varnish631)
-	[`varnish:6.3.1-1`](#varnish631-1)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:stable`](#varnishstable)

## `varnish:6`

```console
$ docker pull varnish@sha256:3669ea06ee7e0f47bfc8feb58f735603e45c5f6558c32e133cfeecc6c829f61f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:2696746f50c4d78b0ed14dbf5ca38f72b1491cd1e0da35c9f5beb7066ac6b548
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67423387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b81057c246da9ad3dd0a29a45c69826d0c7b14b7a78a10f090c42fee3c15c9`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Tue, 04 Feb 2020 15:30:04 GMT
ENV VARNISH_VERSION=6.3.2-1~stretch
# Tue, 04 Feb 2020 15:30:26 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=920A8A7AA7120A8604BCCD294A42CD6EB810E55D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish63/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Feb 2020 15:30:27 GMT
WORKDIR /etc/varnish
# Tue, 04 Feb 2020 15:30:27 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Tue, 04 Feb 2020 15:30:27 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 04 Feb 2020 15:30:27 GMT
EXPOSE 80
# Tue, 04 Feb 2020 15:30:27 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc291c73df31fab402d8b605314fffbcd5003e58fc59e7a7b167cc08d21dd29`  
		Last Modified: Tue, 04 Feb 2020 15:31:16 GMT  
		Size: 44.9 MB (44898291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715baf7fed4ff9a026e19a74045bd47e94949f6e01531565f76b8d55a3648ace`  
		Last Modified: Tue, 04 Feb 2020 15:31:07 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:bb6edcc0c06577a23825fdf6fc41a67d2b48a0bf92d7127c582b1165d4705a81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:54f3120e54c08bdd7ced18a79532c59bfc51e0175e3b4850eb61e4f5eb215ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67219539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f97cf5984fca6b4fa6410da855c4dfa856f8c276d6d339eca86cd554bf0c2`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Tue, 04 Feb 2020 15:30:32 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 04 Feb 2020 15:30:54 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Feb 2020 15:30:54 GMT
WORKDIR /etc/varnish
# Tue, 04 Feb 2020 15:30:54 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Tue, 04 Feb 2020 15:30:55 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 04 Feb 2020 15:30:55 GMT
EXPOSE 80
# Tue, 04 Feb 2020 15:30:55 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8737e60add224d9031379d210507baccecee4d94e428316a8a0acabe28ab6c13`  
		Last Modified: Tue, 04 Feb 2020 15:31:31 GMT  
		Size: 44.7 MB (44694444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d4db90dbc4f2e6053ff6971a862a60dba660127bdfe1e394b5b15cd43783e0`  
		Last Modified: Tue, 04 Feb 2020 15:31:22 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.5`

```console
$ docker pull varnish@sha256:f0c639a79703b7d6536be7211bbea9dbe9232c2e5446e57ae17b497d93009fa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.5` - linux; amd64

```console
$ docker pull varnish@sha256:bf8c888b26e18ca1a4475626dfa4a442f33dfb311ac13e4c4f885d35d92b53f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67212491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c113b275d6230db15226492bd6d721cad5d140c3d6b669f4eb4839caf6e021a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:53:26 GMT
ENV VARNISH_VERSION=6.0.5-1~stretch
# Sat, 01 Feb 2020 17:53:51 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:53:51 GMT
WORKDIR /etc/varnish
# Sat, 01 Feb 2020 17:53:52 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:53:52 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 01 Feb 2020 17:53:52 GMT
EXPOSE 80
# Sat, 01 Feb 2020 17:53:52 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e370e8f41efeaa3210db0b43f45daea45dd419aefc62d003ae806b4fe24541e0`  
		Last Modified: Sat, 01 Feb 2020 17:54:30 GMT  
		Size: 44.7 MB (44687396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d134e536b7aa0d6d3042e185640e19258122ecc2de2f60f3266d870faa6ff3c3`  
		Last Modified: Sat, 01 Feb 2020 17:54:20 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.5-1`

```console
$ docker pull varnish@sha256:f0c639a79703b7d6536be7211bbea9dbe9232c2e5446e57ae17b497d93009fa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.5-1` - linux; amd64

```console
$ docker pull varnish@sha256:bf8c888b26e18ca1a4475626dfa4a442f33dfb311ac13e4c4f885d35d92b53f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67212491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c113b275d6230db15226492bd6d721cad5d140c3d6b669f4eb4839caf6e021a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:53:26 GMT
ENV VARNISH_VERSION=6.0.5-1~stretch
# Sat, 01 Feb 2020 17:53:51 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:53:51 GMT
WORKDIR /etc/varnish
# Sat, 01 Feb 2020 17:53:52 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:53:52 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 01 Feb 2020 17:53:52 GMT
EXPOSE 80
# Sat, 01 Feb 2020 17:53:52 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e370e8f41efeaa3210db0b43f45daea45dd419aefc62d003ae806b4fe24541e0`  
		Last Modified: Sat, 01 Feb 2020 17:54:30 GMT  
		Size: 44.7 MB (44687396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d134e536b7aa0d6d3042e185640e19258122ecc2de2f60f3266d870faa6ff3c3`  
		Last Modified: Sat, 01 Feb 2020 17:54:20 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.3`

```console
$ docker pull varnish@sha256:3669ea06ee7e0f47bfc8feb58f735603e45c5f6558c32e133cfeecc6c829f61f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.3` - linux; amd64

```console
$ docker pull varnish@sha256:2696746f50c4d78b0ed14dbf5ca38f72b1491cd1e0da35c9f5beb7066ac6b548
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67423387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b81057c246da9ad3dd0a29a45c69826d0c7b14b7a78a10f090c42fee3c15c9`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Tue, 04 Feb 2020 15:30:04 GMT
ENV VARNISH_VERSION=6.3.2-1~stretch
# Tue, 04 Feb 2020 15:30:26 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=920A8A7AA7120A8604BCCD294A42CD6EB810E55D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish63/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Feb 2020 15:30:27 GMT
WORKDIR /etc/varnish
# Tue, 04 Feb 2020 15:30:27 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Tue, 04 Feb 2020 15:30:27 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 04 Feb 2020 15:30:27 GMT
EXPOSE 80
# Tue, 04 Feb 2020 15:30:27 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc291c73df31fab402d8b605314fffbcd5003e58fc59e7a7b167cc08d21dd29`  
		Last Modified: Tue, 04 Feb 2020 15:31:16 GMT  
		Size: 44.9 MB (44898291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715baf7fed4ff9a026e19a74045bd47e94949f6e01531565f76b8d55a3648ace`  
		Last Modified: Tue, 04 Feb 2020 15:31:07 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.3.1`

```console
$ docker pull varnish@sha256:bd2b2fddc066ceb9bfd915e9af0cbcbe225c5e93c4bf711f54aadaf295f89dab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.3.1` - linux; amd64

```console
$ docker pull varnish@sha256:27fab5187252a3c67c00a0d92aff6e60ee404d9478abc6c6928578c6cfe3d8f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67422144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ce7778df455b78ce3d04d6234c8eddee16de8eba02eb804b24b7db8dd90fed`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:52:53 GMT
ENV VARNISH_VERSION=6.3.1-1~stretch
# Sat, 01 Feb 2020 17:53:18 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=920A8A7AA7120A8604BCCD294A42CD6EB810E55D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish63/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:53:18 GMT
WORKDIR /etc/varnish
# Sat, 01 Feb 2020 17:53:19 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:53:19 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 01 Feb 2020 17:53:19 GMT
EXPOSE 80
# Sat, 01 Feb 2020 17:53:19 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bce57584ceb0ab38a8c6aba55db91047868bc7acca421fd183db5cb48a4e7af`  
		Last Modified: Sat, 01 Feb 2020 17:54:13 GMT  
		Size: 44.9 MB (44897048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bd4833ace7b4db638f363e7111bde358e4a018c2a730bbe3c144f9484316c0`  
		Last Modified: Sat, 01 Feb 2020 17:54:03 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.3.1-1`

```console
$ docker pull varnish@sha256:bd2b2fddc066ceb9bfd915e9af0cbcbe225c5e93c4bf711f54aadaf295f89dab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.3.1-1` - linux; amd64

```console
$ docker pull varnish@sha256:27fab5187252a3c67c00a0d92aff6e60ee404d9478abc6c6928578c6cfe3d8f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67422144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ce7778df455b78ce3d04d6234c8eddee16de8eba02eb804b24b7db8dd90fed`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:52:53 GMT
ENV VARNISH_VERSION=6.3.1-1~stretch
# Sat, 01 Feb 2020 17:53:18 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=920A8A7AA7120A8604BCCD294A42CD6EB810E55D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish63/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:53:18 GMT
WORKDIR /etc/varnish
# Sat, 01 Feb 2020 17:53:19 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:53:19 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 01 Feb 2020 17:53:19 GMT
EXPOSE 80
# Sat, 01 Feb 2020 17:53:19 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bce57584ceb0ab38a8c6aba55db91047868bc7acca421fd183db5cb48a4e7af`  
		Last Modified: Sat, 01 Feb 2020 17:54:13 GMT  
		Size: 44.9 MB (44897048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bd4833ace7b4db638f363e7111bde358e4a018c2a730bbe3c144f9484316c0`  
		Last Modified: Sat, 01 Feb 2020 17:54:03 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:3669ea06ee7e0f47bfc8feb58f735603e45c5f6558c32e133cfeecc6c829f61f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:2696746f50c4d78b0ed14dbf5ca38f72b1491cd1e0da35c9f5beb7066ac6b548
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67423387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b81057c246da9ad3dd0a29a45c69826d0c7b14b7a78a10f090c42fee3c15c9`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Tue, 04 Feb 2020 15:30:04 GMT
ENV VARNISH_VERSION=6.3.2-1~stretch
# Tue, 04 Feb 2020 15:30:26 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=920A8A7AA7120A8604BCCD294A42CD6EB810E55D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish63/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Feb 2020 15:30:27 GMT
WORKDIR /etc/varnish
# Tue, 04 Feb 2020 15:30:27 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Tue, 04 Feb 2020 15:30:27 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 04 Feb 2020 15:30:27 GMT
EXPOSE 80
# Tue, 04 Feb 2020 15:30:27 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc291c73df31fab402d8b605314fffbcd5003e58fc59e7a7b167cc08d21dd29`  
		Last Modified: Tue, 04 Feb 2020 15:31:16 GMT  
		Size: 44.9 MB (44898291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715baf7fed4ff9a026e19a74045bd47e94949f6e01531565f76b8d55a3648ace`  
		Last Modified: Tue, 04 Feb 2020 15:31:07 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:3669ea06ee7e0f47bfc8feb58f735603e45c5f6558c32e133cfeecc6c829f61f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:2696746f50c4d78b0ed14dbf5ca38f72b1491cd1e0da35c9f5beb7066ac6b548
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67423387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b81057c246da9ad3dd0a29a45c69826d0c7b14b7a78a10f090c42fee3c15c9`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Tue, 04 Feb 2020 15:30:04 GMT
ENV VARNISH_VERSION=6.3.2-1~stretch
# Tue, 04 Feb 2020 15:30:26 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=920A8A7AA7120A8604BCCD294A42CD6EB810E55D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish63/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Feb 2020 15:30:27 GMT
WORKDIR /etc/varnish
# Tue, 04 Feb 2020 15:30:27 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Tue, 04 Feb 2020 15:30:27 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 04 Feb 2020 15:30:27 GMT
EXPOSE 80
# Tue, 04 Feb 2020 15:30:27 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc291c73df31fab402d8b605314fffbcd5003e58fc59e7a7b167cc08d21dd29`  
		Last Modified: Tue, 04 Feb 2020 15:31:16 GMT  
		Size: 44.9 MB (44898291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715baf7fed4ff9a026e19a74045bd47e94949f6e01531565f76b8d55a3648ace`  
		Last Modified: Tue, 04 Feb 2020 15:31:07 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:bb6edcc0c06577a23825fdf6fc41a67d2b48a0bf92d7127c582b1165d4705a81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:54f3120e54c08bdd7ced18a79532c59bfc51e0175e3b4850eb61e4f5eb215ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67219539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f97cf5984fca6b4fa6410da855c4dfa856f8c276d6d339eca86cd554bf0c2`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Tue, 04 Feb 2020 15:30:32 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 04 Feb 2020 15:30:54 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Feb 2020 15:30:54 GMT
WORKDIR /etc/varnish
# Tue, 04 Feb 2020 15:30:54 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Tue, 04 Feb 2020 15:30:55 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 04 Feb 2020 15:30:55 GMT
EXPOSE 80
# Tue, 04 Feb 2020 15:30:55 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8737e60add224d9031379d210507baccecee4d94e428316a8a0acabe28ab6c13`  
		Last Modified: Tue, 04 Feb 2020 15:31:31 GMT  
		Size: 44.7 MB (44694444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d4db90dbc4f2e6053ff6971a862a60dba660127bdfe1e394b5b15cd43783e0`  
		Last Modified: Tue, 04 Feb 2020 15:31:22 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
