<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6`](#varnish6)
-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.7`](#varnish607)
-	[`varnish:6.0.7-1`](#varnish607-1)
-	[`varnish:6.5`](#varnish65)
-	[`varnish:6.5.1`](#varnish651)
-	[`varnish:6.5.1-1`](#varnish651-1)
-	[`varnish:6.6`](#varnish66)
-	[`varnish:6.6.0`](#varnish660)
-	[`varnish:6.6.0-1`](#varnish660-1)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:stable`](#varnishstable)

## `varnish:6`

```console
$ docker pull varnish@sha256:f0e3813783a6824c60bf1becb1adbb8cd8d64d3b65dc8e221f6d6059499faf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:01ec18ab5334fc63a8ef318a3926eb26f7bfc3576888153c53eff5d9f1074542
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223dd593d1188c57ecea403179d4c64b7a0a55c6805b2aa9704d79b96b449b92`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:56 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:56 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:56 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:57 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:57 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f948e9bf95e4d0f40c6cbfdecc4ac83a7455c9d8463b5b123e32a660eb25f1`  
		Last Modified: Sat, 27 Mar 2021 10:18:17 GMT  
		Size: 49.9 MB (49919183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b089b2959d04b32d37a9f9f060c27cee667b73a4d10782cce87a258479b5cb7`  
		Last Modified: Sat, 27 Mar 2021 10:18:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:957807c4e02d0c33385f19a9d5095d4147127c53cd5ede7e9485347401c976d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:fbf80ec71ece3271b7b87872b1bde1271db99786ad568e9c734b333d9cebca6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76436759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77668bae4795f04befdc105189d713cd48fb938874dc00886c040c212b188b2`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:11 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Sat, 27 Mar 2021 10:16:12 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:30 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:30 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:30 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:31 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:31 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:31 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c937c76920eabaacdd92359cc4d6c972e16c157279b8169969d8f54efb7f5d1`  
		Last Modified: Sat, 27 Mar 2021 10:17:53 GMT  
		Size: 49.3 MB (49335288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8811b6f861fa73a0edac0430ae8ab98617e74c8f2cd18a18f82fe991182bbf`  
		Last Modified: Sat, 27 Mar 2021 10:17:45 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7`

```console
$ docker pull varnish@sha256:957807c4e02d0c33385f19a9d5095d4147127c53cd5ede7e9485347401c976d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.7` - linux; amd64

```console
$ docker pull varnish@sha256:fbf80ec71ece3271b7b87872b1bde1271db99786ad568e9c734b333d9cebca6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76436759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77668bae4795f04befdc105189d713cd48fb938874dc00886c040c212b188b2`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:11 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Sat, 27 Mar 2021 10:16:12 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:30 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:30 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:30 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:31 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:31 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:31 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c937c76920eabaacdd92359cc4d6c972e16c157279b8169969d8f54efb7f5d1`  
		Last Modified: Sat, 27 Mar 2021 10:17:53 GMT  
		Size: 49.3 MB (49335288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8811b6f861fa73a0edac0430ae8ab98617e74c8f2cd18a18f82fe991182bbf`  
		Last Modified: Sat, 27 Mar 2021 10:17:45 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7-1`

```console
$ docker pull varnish@sha256:957807c4e02d0c33385f19a9d5095d4147127c53cd5ede7e9485347401c976d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.7-1` - linux; amd64

```console
$ docker pull varnish@sha256:fbf80ec71ece3271b7b87872b1bde1271db99786ad568e9c734b333d9cebca6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76436759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77668bae4795f04befdc105189d713cd48fb938874dc00886c040c212b188b2`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:11 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Sat, 27 Mar 2021 10:16:12 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:30 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:30 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:30 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:31 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:31 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:31 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c937c76920eabaacdd92359cc4d6c972e16c157279b8169969d8f54efb7f5d1`  
		Last Modified: Sat, 27 Mar 2021 10:17:53 GMT  
		Size: 49.3 MB (49335288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8811b6f861fa73a0edac0430ae8ab98617e74c8f2cd18a18f82fe991182bbf`  
		Last Modified: Sat, 27 Mar 2021 10:17:45 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5`

```console
$ docker pull varnish@sha256:cbd83d264d8671254d6939dbe0f88a873a2da2e965841bb82ae35573df84292b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5` - linux; amd64

```console
$ docker pull varnish@sha256:2950bab1ec733b8877aaf23fb78be7cedcc65d42ec77a89c4ba60cdd3c8c9683
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76888016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:310005d15946c9a8c10da662873080a8db8340322e4a7ee9b3e634dd524e3962`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:17:03 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Sat, 27 Mar 2021 10:17:03 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:17:21 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:17:22 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:17:22 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:17:22 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:17:22 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:17:23 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942c1d956f8637e34665630efd6779b8e2390853e14ec78f82e09644f89c5706`  
		Last Modified: Sat, 27 Mar 2021 10:18:45 GMT  
		Size: 49.8 MB (49786546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53ce1b2b4132d16c679e5411167973db7696d7ef5246727199652eac26d1f6b`  
		Last Modified: Sat, 27 Mar 2021 10:18:37 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1`

```console
$ docker pull varnish@sha256:cbd83d264d8671254d6939dbe0f88a873a2da2e965841bb82ae35573df84292b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1` - linux; amd64

```console
$ docker pull varnish@sha256:2950bab1ec733b8877aaf23fb78be7cedcc65d42ec77a89c4ba60cdd3c8c9683
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76888016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:310005d15946c9a8c10da662873080a8db8340322e4a7ee9b3e634dd524e3962`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:17:03 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Sat, 27 Mar 2021 10:17:03 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:17:21 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:17:22 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:17:22 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:17:22 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:17:22 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:17:23 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942c1d956f8637e34665630efd6779b8e2390853e14ec78f82e09644f89c5706`  
		Last Modified: Sat, 27 Mar 2021 10:18:45 GMT  
		Size: 49.8 MB (49786546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53ce1b2b4132d16c679e5411167973db7696d7ef5246727199652eac26d1f6b`  
		Last Modified: Sat, 27 Mar 2021 10:18:37 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1-1`

```console
$ docker pull varnish@sha256:cbd83d264d8671254d6939dbe0f88a873a2da2e965841bb82ae35573df84292b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1-1` - linux; amd64

```console
$ docker pull varnish@sha256:2950bab1ec733b8877aaf23fb78be7cedcc65d42ec77a89c4ba60cdd3c8c9683
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76888016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:310005d15946c9a8c10da662873080a8db8340322e4a7ee9b3e634dd524e3962`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:17:03 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Sat, 27 Mar 2021 10:17:03 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:17:21 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:17:22 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:17:22 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:17:22 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:17:22 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:17:23 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942c1d956f8637e34665630efd6779b8e2390853e14ec78f82e09644f89c5706`  
		Last Modified: Sat, 27 Mar 2021 10:18:45 GMT  
		Size: 49.8 MB (49786546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53ce1b2b4132d16c679e5411167973db7696d7ef5246727199652eac26d1f6b`  
		Last Modified: Sat, 27 Mar 2021 10:18:37 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6`

```console
$ docker pull varnish@sha256:f0e3813783a6824c60bf1becb1adbb8cd8d64d3b65dc8e221f6d6059499faf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.6` - linux; amd64

```console
$ docker pull varnish@sha256:01ec18ab5334fc63a8ef318a3926eb26f7bfc3576888153c53eff5d9f1074542
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223dd593d1188c57ecea403179d4c64b7a0a55c6805b2aa9704d79b96b449b92`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:56 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:56 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:56 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:57 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:57 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f948e9bf95e4d0f40c6cbfdecc4ac83a7455c9d8463b5b123e32a660eb25f1`  
		Last Modified: Sat, 27 Mar 2021 10:18:17 GMT  
		Size: 49.9 MB (49919183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b089b2959d04b32d37a9f9f060c27cee667b73a4d10782cce87a258479b5cb7`  
		Last Modified: Sat, 27 Mar 2021 10:18:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.0`

```console
$ docker pull varnish@sha256:f0e3813783a6824c60bf1becb1adbb8cd8d64d3b65dc8e221f6d6059499faf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.6.0` - linux; amd64

```console
$ docker pull varnish@sha256:01ec18ab5334fc63a8ef318a3926eb26f7bfc3576888153c53eff5d9f1074542
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223dd593d1188c57ecea403179d4c64b7a0a55c6805b2aa9704d79b96b449b92`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:56 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:56 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:56 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:57 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:57 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f948e9bf95e4d0f40c6cbfdecc4ac83a7455c9d8463b5b123e32a660eb25f1`  
		Last Modified: Sat, 27 Mar 2021 10:18:17 GMT  
		Size: 49.9 MB (49919183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b089b2959d04b32d37a9f9f060c27cee667b73a4d10782cce87a258479b5cb7`  
		Last Modified: Sat, 27 Mar 2021 10:18:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.0-1`

```console
$ docker pull varnish@sha256:f0e3813783a6824c60bf1becb1adbb8cd8d64d3b65dc8e221f6d6059499faf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.6.0-1` - linux; amd64

```console
$ docker pull varnish@sha256:01ec18ab5334fc63a8ef318a3926eb26f7bfc3576888153c53eff5d9f1074542
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223dd593d1188c57ecea403179d4c64b7a0a55c6805b2aa9704d79b96b449b92`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:56 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:56 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:56 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:57 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:57 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f948e9bf95e4d0f40c6cbfdecc4ac83a7455c9d8463b5b123e32a660eb25f1`  
		Last Modified: Sat, 27 Mar 2021 10:18:17 GMT  
		Size: 49.9 MB (49919183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b089b2959d04b32d37a9f9f060c27cee667b73a4d10782cce87a258479b5cb7`  
		Last Modified: Sat, 27 Mar 2021 10:18:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:f0e3813783a6824c60bf1becb1adbb8cd8d64d3b65dc8e221f6d6059499faf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:01ec18ab5334fc63a8ef318a3926eb26f7bfc3576888153c53eff5d9f1074542
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223dd593d1188c57ecea403179d4c64b7a0a55c6805b2aa9704d79b96b449b92`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:56 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:56 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:56 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:57 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:57 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f948e9bf95e4d0f40c6cbfdecc4ac83a7455c9d8463b5b123e32a660eb25f1`  
		Last Modified: Sat, 27 Mar 2021 10:18:17 GMT  
		Size: 49.9 MB (49919183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b089b2959d04b32d37a9f9f060c27cee667b73a4d10782cce87a258479b5cb7`  
		Last Modified: Sat, 27 Mar 2021 10:18:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:f0e3813783a6824c60bf1becb1adbb8cd8d64d3b65dc8e221f6d6059499faf16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:01ec18ab5334fc63a8ef318a3926eb26f7bfc3576888153c53eff5d9f1074542
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223dd593d1188c57ecea403179d4c64b7a0a55c6805b2aa9704d79b96b449b92`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Sat, 27 Mar 2021 10:16:37 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:56 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:56 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:56 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:57 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:57 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f948e9bf95e4d0f40c6cbfdecc4ac83a7455c9d8463b5b123e32a660eb25f1`  
		Last Modified: Sat, 27 Mar 2021 10:18:17 GMT  
		Size: 49.9 MB (49919183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b089b2959d04b32d37a9f9f060c27cee667b73a4d10782cce87a258479b5cb7`  
		Last Modified: Sat, 27 Mar 2021 10:18:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:957807c4e02d0c33385f19a9d5095d4147127c53cd5ede7e9485347401c976d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:fbf80ec71ece3271b7b87872b1bde1271db99786ad568e9c734b333d9cebca6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76436759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77668bae4795f04befdc105189d713cd48fb938874dc00886c040c212b188b2`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:11 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Sat, 27 Mar 2021 10:16:12 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:30 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:30 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:30 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:31 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:31 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:31 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c937c76920eabaacdd92359cc4d6c972e16c157279b8169969d8f54efb7f5d1`  
		Last Modified: Sat, 27 Mar 2021 10:17:53 GMT  
		Size: 49.3 MB (49335288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8811b6f861fa73a0edac0430ae8ab98617e74c8f2cd18a18f82fe991182bbf`  
		Last Modified: Sat, 27 Mar 2021 10:17:45 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
