<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6`](#varnish6)
-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.6`](#varnish606)
-	[`varnish:6.0.6-1`](#varnish606-1)
-	[`varnish:6.4`](#varnish64)
-	[`varnish:6.4.0`](#varnish640)
-	[`varnish:6.4.0-1`](#varnish640-1)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:stable`](#varnishstable)

## `varnish:6`

```console
$ docker pull varnish@sha256:09a2a01d6d41c5cc88c9d85e750c2b031dce4c909a1b4865cf25f01a12b6f213
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:d7878aa0cbbdca4a33883edb7daa259de272e809cb8018f1fe99a9451735591c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce9bdf363596a6e335f526f99de9bfdcd5598ccb05b9e47de9a9b62d09cb432`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:46 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:46 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:47 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:47 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:47 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:47 GMT
CMD []
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed80e2c033a5c92c8910b2d74a0913592f80017f593e9b46be2274e7cdad48`  
		Last Modified: Fri, 15 May 2020 17:30:07 GMT  
		Size: 49.7 MB (49675645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1f398e3c208fd74434937915d6c020fb90dcee00d6298697ef141aa79fbec4`  
		Last Modified: Fri, 15 May 2020 17:29:36 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:b7b270277f7ff1fa624059e1633a29f54f1a8200b7279871445e906213e6475e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:5b58787ad119856832a61a3a637f19053fad2fdf0effcd5373bf73d1e08aad91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67214871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c48be5f3e59649ba57eb98fcda534688e21e5aceec599425539d5ffcdd1d242`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:27:46 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Fri, 15 May 2020 17:27:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:14 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:14 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:14 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:14 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:14 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:15 GMT
CMD []
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4087ef1fd116ce07f37e775b8d4983e407e50af521422c81f313f3918447cfc`  
		Last Modified: Fri, 15 May 2020 17:29:31 GMT  
		Size: 44.7 MB (44694524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ec0e52db2a9fae3c11c57297845112c9237ca26199a1f2c30e13ccadfb26a9`  
		Last Modified: Fri, 15 May 2020 17:28:58 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6`

```console
$ docker pull varnish@sha256:b7b270277f7ff1fa624059e1633a29f54f1a8200b7279871445e906213e6475e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6` - linux; amd64

```console
$ docker pull varnish@sha256:5b58787ad119856832a61a3a637f19053fad2fdf0effcd5373bf73d1e08aad91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67214871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c48be5f3e59649ba57eb98fcda534688e21e5aceec599425539d5ffcdd1d242`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:27:46 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Fri, 15 May 2020 17:27:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:14 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:14 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:14 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:14 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:14 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:15 GMT
CMD []
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4087ef1fd116ce07f37e775b8d4983e407e50af521422c81f313f3918447cfc`  
		Last Modified: Fri, 15 May 2020 17:29:31 GMT  
		Size: 44.7 MB (44694524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ec0e52db2a9fae3c11c57297845112c9237ca26199a1f2c30e13ccadfb26a9`  
		Last Modified: Fri, 15 May 2020 17:28:58 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6-1`

```console
$ docker pull varnish@sha256:b7b270277f7ff1fa624059e1633a29f54f1a8200b7279871445e906213e6475e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6-1` - linux; amd64

```console
$ docker pull varnish@sha256:5b58787ad119856832a61a3a637f19053fad2fdf0effcd5373bf73d1e08aad91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67214871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c48be5f3e59649ba57eb98fcda534688e21e5aceec599425539d5ffcdd1d242`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:27:46 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Fri, 15 May 2020 17:27:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:14 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:14 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:14 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:14 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:14 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:15 GMT
CMD []
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4087ef1fd116ce07f37e775b8d4983e407e50af521422c81f313f3918447cfc`  
		Last Modified: Fri, 15 May 2020 17:29:31 GMT  
		Size: 44.7 MB (44694524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ec0e52db2a9fae3c11c57297845112c9237ca26199a1f2c30e13ccadfb26a9`  
		Last Modified: Fri, 15 May 2020 17:28:58 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4`

```console
$ docker pull varnish@sha256:09a2a01d6d41c5cc88c9d85e750c2b031dce4c909a1b4865cf25f01a12b6f213
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4` - linux; amd64

```console
$ docker pull varnish@sha256:d7878aa0cbbdca4a33883edb7daa259de272e809cb8018f1fe99a9451735591c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce9bdf363596a6e335f526f99de9bfdcd5598ccb05b9e47de9a9b62d09cb432`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:46 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:46 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:47 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:47 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:47 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:47 GMT
CMD []
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed80e2c033a5c92c8910b2d74a0913592f80017f593e9b46be2274e7cdad48`  
		Last Modified: Fri, 15 May 2020 17:30:07 GMT  
		Size: 49.7 MB (49675645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1f398e3c208fd74434937915d6c020fb90dcee00d6298697ef141aa79fbec4`  
		Last Modified: Fri, 15 May 2020 17:29:36 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4.0`

```console
$ docker pull varnish@sha256:09a2a01d6d41c5cc88c9d85e750c2b031dce4c909a1b4865cf25f01a12b6f213
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4.0` - linux; amd64

```console
$ docker pull varnish@sha256:d7878aa0cbbdca4a33883edb7daa259de272e809cb8018f1fe99a9451735591c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce9bdf363596a6e335f526f99de9bfdcd5598ccb05b9e47de9a9b62d09cb432`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:46 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:46 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:47 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:47 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:47 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:47 GMT
CMD []
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed80e2c033a5c92c8910b2d74a0913592f80017f593e9b46be2274e7cdad48`  
		Last Modified: Fri, 15 May 2020 17:30:07 GMT  
		Size: 49.7 MB (49675645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1f398e3c208fd74434937915d6c020fb90dcee00d6298697ef141aa79fbec4`  
		Last Modified: Fri, 15 May 2020 17:29:36 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4.0-1`

```console
$ docker pull varnish@sha256:09a2a01d6d41c5cc88c9d85e750c2b031dce4c909a1b4865cf25f01a12b6f213
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4.0-1` - linux; amd64

```console
$ docker pull varnish@sha256:d7878aa0cbbdca4a33883edb7daa259de272e809cb8018f1fe99a9451735591c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce9bdf363596a6e335f526f99de9bfdcd5598ccb05b9e47de9a9b62d09cb432`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:46 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:46 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:47 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:47 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:47 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:47 GMT
CMD []
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed80e2c033a5c92c8910b2d74a0913592f80017f593e9b46be2274e7cdad48`  
		Last Modified: Fri, 15 May 2020 17:30:07 GMT  
		Size: 49.7 MB (49675645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1f398e3c208fd74434937915d6c020fb90dcee00d6298697ef141aa79fbec4`  
		Last Modified: Fri, 15 May 2020 17:29:36 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:09a2a01d6d41c5cc88c9d85e750c2b031dce4c909a1b4865cf25f01a12b6f213
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:d7878aa0cbbdca4a33883edb7daa259de272e809cb8018f1fe99a9451735591c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce9bdf363596a6e335f526f99de9bfdcd5598ccb05b9e47de9a9b62d09cb432`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:46 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:46 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:47 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:47 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:47 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:47 GMT
CMD []
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed80e2c033a5c92c8910b2d74a0913592f80017f593e9b46be2274e7cdad48`  
		Last Modified: Fri, 15 May 2020 17:30:07 GMT  
		Size: 49.7 MB (49675645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1f398e3c208fd74434937915d6c020fb90dcee00d6298697ef141aa79fbec4`  
		Last Modified: Fri, 15 May 2020 17:29:36 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:09a2a01d6d41c5cc88c9d85e750c2b031dce4c909a1b4865cf25f01a12b6f213
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:d7878aa0cbbdca4a33883edb7daa259de272e809cb8018f1fe99a9451735591c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce9bdf363596a6e335f526f99de9bfdcd5598ccb05b9e47de9a9b62d09cb432`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:46 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:46 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:47 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:47 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:47 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:47 GMT
CMD []
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed80e2c033a5c92c8910b2d74a0913592f80017f593e9b46be2274e7cdad48`  
		Last Modified: Fri, 15 May 2020 17:30:07 GMT  
		Size: 49.7 MB (49675645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1f398e3c208fd74434937915d6c020fb90dcee00d6298697ef141aa79fbec4`  
		Last Modified: Fri, 15 May 2020 17:29:36 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:b7b270277f7ff1fa624059e1633a29f54f1a8200b7279871445e906213e6475e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:5b58787ad119856832a61a3a637f19053fad2fdf0effcd5373bf73d1e08aad91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67214871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c48be5f3e59649ba57eb98fcda534688e21e5aceec599425539d5ffcdd1d242`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:27:46 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Fri, 15 May 2020 17:27:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:14 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:14 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:14 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:14 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:14 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:15 GMT
CMD []
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4087ef1fd116ce07f37e775b8d4983e407e50af521422c81f313f3918447cfc`  
		Last Modified: Fri, 15 May 2020 17:29:31 GMT  
		Size: 44.7 MB (44694524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ec0e52db2a9fae3c11c57297845112c9237ca26199a1f2c30e13ccadfb26a9`  
		Last Modified: Fri, 15 May 2020 17:28:58 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
