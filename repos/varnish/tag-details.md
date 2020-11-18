<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6`](#varnish6)
-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.7`](#varnish607)
-	[`varnish:6.0.7-1`](#varnish607-1)
-	[`varnish:6.5`](#varnish65)
-	[`varnish:6.5.1`](#varnish651)
-	[`varnish:6.5.1-1`](#varnish651-1)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:stable`](#varnishstable)

## `varnish:6`

```console
$ docker pull varnish@sha256:0d3d51af397f0f3848591c2dbbb736acc87e376a3d27db245ff37a371463d316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:ffd69fa9b3b809b2972af274842032ab6b58d56b106f4763836d4b98082d52bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76870734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f44daab011883ee4ae43c2898e2c499d42331b10f1e4c59da97eba173d71ed8`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:13:17 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:13:17 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:13:17 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:13:18 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:13:18 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:13:18 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b38d803296357b4e6196ec35794232b586096ed5572b04b1c953fde10fe5f72`  
		Last Modified: Wed, 18 Nov 2020 12:13:57 GMT  
		Size: 49.8 MB (49764776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc68174d224e30120ec4434da43cca86f85809543996a0b467fb5b42e5d1720e`  
		Last Modified: Wed, 18 Nov 2020 12:13:46 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:b4315de7d49cd68a72810fd637f5586f42632857dcfc22736660ce8d05bfc9a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:a195f1c303e0102e0026fc5f5d20cf737c9335822698a4ed1b66663cf2849f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76417976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49f9c54e7b31bb0001eeec678cea99557e93e8292732a4bd8091585423e9f44`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:11:55 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 18 Nov 2020 12:11:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:12:29 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:12:29 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:12:30 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:12:30 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:12:31 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:12:31 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47198ca4ce2f0366a4729255c249a5c6473befdf944e585618f512cd13c1f931`  
		Last Modified: Wed, 18 Nov 2020 12:13:40 GMT  
		Size: 49.3 MB (49312018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6cecd5e3167f9257fb6660755da7aa6dcd48615f431b1370998f9fbc3b17e4`  
		Last Modified: Wed, 18 Nov 2020 12:13:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7`

```console
$ docker pull varnish@sha256:b4315de7d49cd68a72810fd637f5586f42632857dcfc22736660ce8d05bfc9a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.7` - linux; amd64

```console
$ docker pull varnish@sha256:a195f1c303e0102e0026fc5f5d20cf737c9335822698a4ed1b66663cf2849f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76417976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49f9c54e7b31bb0001eeec678cea99557e93e8292732a4bd8091585423e9f44`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:11:55 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 18 Nov 2020 12:11:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:12:29 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:12:29 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:12:30 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:12:30 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:12:31 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:12:31 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47198ca4ce2f0366a4729255c249a5c6473befdf944e585618f512cd13c1f931`  
		Last Modified: Wed, 18 Nov 2020 12:13:40 GMT  
		Size: 49.3 MB (49312018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6cecd5e3167f9257fb6660755da7aa6dcd48615f431b1370998f9fbc3b17e4`  
		Last Modified: Wed, 18 Nov 2020 12:13:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7-1`

```console
$ docker pull varnish@sha256:b4315de7d49cd68a72810fd637f5586f42632857dcfc22736660ce8d05bfc9a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.7-1` - linux; amd64

```console
$ docker pull varnish@sha256:a195f1c303e0102e0026fc5f5d20cf737c9335822698a4ed1b66663cf2849f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76417976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49f9c54e7b31bb0001eeec678cea99557e93e8292732a4bd8091585423e9f44`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:11:55 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 18 Nov 2020 12:11:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:12:29 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:12:29 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:12:30 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:12:30 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:12:31 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:12:31 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47198ca4ce2f0366a4729255c249a5c6473befdf944e585618f512cd13c1f931`  
		Last Modified: Wed, 18 Nov 2020 12:13:40 GMT  
		Size: 49.3 MB (49312018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6cecd5e3167f9257fb6660755da7aa6dcd48615f431b1370998f9fbc3b17e4`  
		Last Modified: Wed, 18 Nov 2020 12:13:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5`

```console
$ docker pull varnish@sha256:0d3d51af397f0f3848591c2dbbb736acc87e376a3d27db245ff37a371463d316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5` - linux; amd64

```console
$ docker pull varnish@sha256:ffd69fa9b3b809b2972af274842032ab6b58d56b106f4763836d4b98082d52bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76870734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f44daab011883ee4ae43c2898e2c499d42331b10f1e4c59da97eba173d71ed8`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:13:17 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:13:17 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:13:17 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:13:18 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:13:18 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:13:18 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b38d803296357b4e6196ec35794232b586096ed5572b04b1c953fde10fe5f72`  
		Last Modified: Wed, 18 Nov 2020 12:13:57 GMT  
		Size: 49.8 MB (49764776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc68174d224e30120ec4434da43cca86f85809543996a0b467fb5b42e5d1720e`  
		Last Modified: Wed, 18 Nov 2020 12:13:46 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1`

```console
$ docker pull varnish@sha256:0d3d51af397f0f3848591c2dbbb736acc87e376a3d27db245ff37a371463d316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1` - linux; amd64

```console
$ docker pull varnish@sha256:ffd69fa9b3b809b2972af274842032ab6b58d56b106f4763836d4b98082d52bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76870734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f44daab011883ee4ae43c2898e2c499d42331b10f1e4c59da97eba173d71ed8`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:13:17 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:13:17 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:13:17 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:13:18 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:13:18 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:13:18 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b38d803296357b4e6196ec35794232b586096ed5572b04b1c953fde10fe5f72`  
		Last Modified: Wed, 18 Nov 2020 12:13:57 GMT  
		Size: 49.8 MB (49764776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc68174d224e30120ec4434da43cca86f85809543996a0b467fb5b42e5d1720e`  
		Last Modified: Wed, 18 Nov 2020 12:13:46 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1-1`

```console
$ docker pull varnish@sha256:0d3d51af397f0f3848591c2dbbb736acc87e376a3d27db245ff37a371463d316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1-1` - linux; amd64

```console
$ docker pull varnish@sha256:ffd69fa9b3b809b2972af274842032ab6b58d56b106f4763836d4b98082d52bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76870734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f44daab011883ee4ae43c2898e2c499d42331b10f1e4c59da97eba173d71ed8`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:13:17 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:13:17 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:13:17 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:13:18 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:13:18 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:13:18 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b38d803296357b4e6196ec35794232b586096ed5572b04b1c953fde10fe5f72`  
		Last Modified: Wed, 18 Nov 2020 12:13:57 GMT  
		Size: 49.8 MB (49764776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc68174d224e30120ec4434da43cca86f85809543996a0b467fb5b42e5d1720e`  
		Last Modified: Wed, 18 Nov 2020 12:13:46 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:0d3d51af397f0f3848591c2dbbb736acc87e376a3d27db245ff37a371463d316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:ffd69fa9b3b809b2972af274842032ab6b58d56b106f4763836d4b98082d52bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76870734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f44daab011883ee4ae43c2898e2c499d42331b10f1e4c59da97eba173d71ed8`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:13:17 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:13:17 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:13:17 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:13:18 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:13:18 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:13:18 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b38d803296357b4e6196ec35794232b586096ed5572b04b1c953fde10fe5f72`  
		Last Modified: Wed, 18 Nov 2020 12:13:57 GMT  
		Size: 49.8 MB (49764776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc68174d224e30120ec4434da43cca86f85809543996a0b467fb5b42e5d1720e`  
		Last Modified: Wed, 18 Nov 2020 12:13:46 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:0d3d51af397f0f3848591c2dbbb736acc87e376a3d27db245ff37a371463d316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:ffd69fa9b3b809b2972af274842032ab6b58d56b106f4763836d4b98082d52bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76870734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f44daab011883ee4ae43c2898e2c499d42331b10f1e4c59da97eba173d71ed8`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Wed, 18 Nov 2020 12:12:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:13:17 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:13:17 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:13:17 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:13:18 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:13:18 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:13:18 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b38d803296357b4e6196ec35794232b586096ed5572b04b1c953fde10fe5f72`  
		Last Modified: Wed, 18 Nov 2020 12:13:57 GMT  
		Size: 49.8 MB (49764776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc68174d224e30120ec4434da43cca86f85809543996a0b467fb5b42e5d1720e`  
		Last Modified: Wed, 18 Nov 2020 12:13:46 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:b4315de7d49cd68a72810fd637f5586f42632857dcfc22736660ce8d05bfc9a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:a195f1c303e0102e0026fc5f5d20cf737c9335822698a4ed1b66663cf2849f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76417976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49f9c54e7b31bb0001eeec678cea99557e93e8292732a4bd8091585423e9f44`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:11:55 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 18 Nov 2020 12:11:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 18 Nov 2020 12:12:29 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:12:29 GMT
WORKDIR /etc/varnish
# Wed, 18 Nov 2020 12:12:30 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 18 Nov 2020 12:12:30 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 18 Nov 2020 12:12:31 GMT
EXPOSE 80 8443
# Wed, 18 Nov 2020 12:12:31 GMT
CMD []
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47198ca4ce2f0366a4729255c249a5c6473befdf944e585618f512cd13c1f931`  
		Last Modified: Wed, 18 Nov 2020 12:13:40 GMT  
		Size: 49.3 MB (49312018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6cecd5e3167f9257fb6660755da7aa6dcd48615f431b1370998f9fbc3b17e4`  
		Last Modified: Wed, 18 Nov 2020 12:13:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
