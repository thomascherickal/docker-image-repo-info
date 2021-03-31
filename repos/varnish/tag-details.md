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
$ docker pull varnish@sha256:5487e5e58e759161e312012a6462d44f8dab8d213b0603fdb2fa4cb70698f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:d4abd66ef8b965ad4cb096eeebdd75d08c0a4aef6117f30e31c23163c1c81a3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77059798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67b0a95f13ffdef60c680f96ed61e2e6b3751a58f4c0e175864fe5a754bf950`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:59 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:59 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:52:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:52:00 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:52:00 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112696cbcf76aafbed649fd17dbfa0f080e4d359e61aaf1ddcf827383495c48`  
		Last Modified: Wed, 31 Mar 2021 14:53:23 GMT  
		Size: 49.9 MB (49920031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6713d4822b777a4866e15acf049c80365d48446086028f5c4b074a922e0d0eb3`  
		Last Modified: Wed, 31 Mar 2021 14:53:12 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:624274b979dfdeac99282c8554f8ccd6d5a1dd632f8f2ad34b24ac842810424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:d2044aeaf884d0b82f37eeb0090782bd1db1c2c3fbd211226869a0afb2962603
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76475169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c770719f0f812ac70fd0136322ff72f316da9e9cb9fb95cfc335ef4d4e1130b`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:09 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 31 Mar 2021 14:51:09 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:32 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:33 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:33 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:51:33 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:51:33 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:51:34 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa58409cf19198895096d632959a96f0d681a94bb34765b872de0770863954`  
		Last Modified: Wed, 31 Mar 2021 14:52:57 GMT  
		Size: 49.3 MB (49335404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bacb4bec39431045e9289ccc4f82e05a5f3425589cdd689a1db527c204aaf1`  
		Last Modified: Wed, 31 Mar 2021 14:52:48 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7`

```console
$ docker pull varnish@sha256:624274b979dfdeac99282c8554f8ccd6d5a1dd632f8f2ad34b24ac842810424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.7` - linux; amd64

```console
$ docker pull varnish@sha256:d2044aeaf884d0b82f37eeb0090782bd1db1c2c3fbd211226869a0afb2962603
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76475169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c770719f0f812ac70fd0136322ff72f316da9e9cb9fb95cfc335ef4d4e1130b`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:09 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 31 Mar 2021 14:51:09 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:32 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:33 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:33 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:51:33 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:51:33 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:51:34 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa58409cf19198895096d632959a96f0d681a94bb34765b872de0770863954`  
		Last Modified: Wed, 31 Mar 2021 14:52:57 GMT  
		Size: 49.3 MB (49335404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bacb4bec39431045e9289ccc4f82e05a5f3425589cdd689a1db527c204aaf1`  
		Last Modified: Wed, 31 Mar 2021 14:52:48 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7-1`

```console
$ docker pull varnish@sha256:624274b979dfdeac99282c8554f8ccd6d5a1dd632f8f2ad34b24ac842810424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.7-1` - linux; amd64

```console
$ docker pull varnish@sha256:d2044aeaf884d0b82f37eeb0090782bd1db1c2c3fbd211226869a0afb2962603
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76475169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c770719f0f812ac70fd0136322ff72f316da9e9cb9fb95cfc335ef4d4e1130b`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:09 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 31 Mar 2021 14:51:09 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:32 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:33 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:33 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:51:33 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:51:33 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:51:34 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa58409cf19198895096d632959a96f0d681a94bb34765b872de0770863954`  
		Last Modified: Wed, 31 Mar 2021 14:52:57 GMT  
		Size: 49.3 MB (49335404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bacb4bec39431045e9289ccc4f82e05a5f3425589cdd689a1db527c204aaf1`  
		Last Modified: Wed, 31 Mar 2021 14:52:48 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5`

```console
$ docker pull varnish@sha256:a8f5d2888b51c5acacce9e9cb8896cae4266ff452a3c460c5af7fcbc9ded1cd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5` - linux; amd64

```console
$ docker pull varnish@sha256:45b78b0eb3c27588535d92b1628bf0cc6513f946ab7bd99db7b4a4ae912d7e66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76926527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557218e15151320561686872f30ad0f6327438e5816a29ae23141c6c033f5156`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:52:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Wed, 31 Mar 2021 14:52:05 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:52:24 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:52:24 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:52:24 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:52:25 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:52:25 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:52:25 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0af2de2805b663d5d321919d5a9d79d40698204892837adf1344168e0670a3`  
		Last Modified: Wed, 31 Mar 2021 14:53:55 GMT  
		Size: 49.8 MB (49786762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ec8a9c1f642e113fb9115d2b209b1e424e2174ac29a494d9dc9e83807c11e6`  
		Last Modified: Wed, 31 Mar 2021 14:53:46 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1`

```console
$ docker pull varnish@sha256:a8f5d2888b51c5acacce9e9cb8896cae4266ff452a3c460c5af7fcbc9ded1cd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1` - linux; amd64

```console
$ docker pull varnish@sha256:45b78b0eb3c27588535d92b1628bf0cc6513f946ab7bd99db7b4a4ae912d7e66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76926527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557218e15151320561686872f30ad0f6327438e5816a29ae23141c6c033f5156`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:52:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Wed, 31 Mar 2021 14:52:05 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:52:24 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:52:24 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:52:24 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:52:25 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:52:25 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:52:25 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0af2de2805b663d5d321919d5a9d79d40698204892837adf1344168e0670a3`  
		Last Modified: Wed, 31 Mar 2021 14:53:55 GMT  
		Size: 49.8 MB (49786762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ec8a9c1f642e113fb9115d2b209b1e424e2174ac29a494d9dc9e83807c11e6`  
		Last Modified: Wed, 31 Mar 2021 14:53:46 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1-1`

```console
$ docker pull varnish@sha256:a8f5d2888b51c5acacce9e9cb8896cae4266ff452a3c460c5af7fcbc9ded1cd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1-1` - linux; amd64

```console
$ docker pull varnish@sha256:45b78b0eb3c27588535d92b1628bf0cc6513f946ab7bd99db7b4a4ae912d7e66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76926527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557218e15151320561686872f30ad0f6327438e5816a29ae23141c6c033f5156`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:52:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Wed, 31 Mar 2021 14:52:05 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:52:24 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:52:24 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:52:24 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:52:25 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:52:25 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:52:25 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0af2de2805b663d5d321919d5a9d79d40698204892837adf1344168e0670a3`  
		Last Modified: Wed, 31 Mar 2021 14:53:55 GMT  
		Size: 49.8 MB (49786762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ec8a9c1f642e113fb9115d2b209b1e424e2174ac29a494d9dc9e83807c11e6`  
		Last Modified: Wed, 31 Mar 2021 14:53:46 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6`

```console
$ docker pull varnish@sha256:5487e5e58e759161e312012a6462d44f8dab8d213b0603fdb2fa4cb70698f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.6` - linux; amd64

```console
$ docker pull varnish@sha256:d4abd66ef8b965ad4cb096eeebdd75d08c0a4aef6117f30e31c23163c1c81a3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77059798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67b0a95f13ffdef60c680f96ed61e2e6b3751a58f4c0e175864fe5a754bf950`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:59 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:59 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:52:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:52:00 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:52:00 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112696cbcf76aafbed649fd17dbfa0f080e4d359e61aaf1ddcf827383495c48`  
		Last Modified: Wed, 31 Mar 2021 14:53:23 GMT  
		Size: 49.9 MB (49920031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6713d4822b777a4866e15acf049c80365d48446086028f5c4b074a922e0d0eb3`  
		Last Modified: Wed, 31 Mar 2021 14:53:12 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.0`

```console
$ docker pull varnish@sha256:5487e5e58e759161e312012a6462d44f8dab8d213b0603fdb2fa4cb70698f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.6.0` - linux; amd64

```console
$ docker pull varnish@sha256:d4abd66ef8b965ad4cb096eeebdd75d08c0a4aef6117f30e31c23163c1c81a3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77059798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67b0a95f13ffdef60c680f96ed61e2e6b3751a58f4c0e175864fe5a754bf950`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:59 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:59 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:52:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:52:00 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:52:00 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112696cbcf76aafbed649fd17dbfa0f080e4d359e61aaf1ddcf827383495c48`  
		Last Modified: Wed, 31 Mar 2021 14:53:23 GMT  
		Size: 49.9 MB (49920031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6713d4822b777a4866e15acf049c80365d48446086028f5c4b074a922e0d0eb3`  
		Last Modified: Wed, 31 Mar 2021 14:53:12 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.0-1`

```console
$ docker pull varnish@sha256:5487e5e58e759161e312012a6462d44f8dab8d213b0603fdb2fa4cb70698f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.6.0-1` - linux; amd64

```console
$ docker pull varnish@sha256:d4abd66ef8b965ad4cb096eeebdd75d08c0a4aef6117f30e31c23163c1c81a3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77059798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67b0a95f13ffdef60c680f96ed61e2e6b3751a58f4c0e175864fe5a754bf950`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:59 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:59 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:52:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:52:00 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:52:00 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112696cbcf76aafbed649fd17dbfa0f080e4d359e61aaf1ddcf827383495c48`  
		Last Modified: Wed, 31 Mar 2021 14:53:23 GMT  
		Size: 49.9 MB (49920031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6713d4822b777a4866e15acf049c80365d48446086028f5c4b074a922e0d0eb3`  
		Last Modified: Wed, 31 Mar 2021 14:53:12 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:5487e5e58e759161e312012a6462d44f8dab8d213b0603fdb2fa4cb70698f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:d4abd66ef8b965ad4cb096eeebdd75d08c0a4aef6117f30e31c23163c1c81a3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77059798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67b0a95f13ffdef60c680f96ed61e2e6b3751a58f4c0e175864fe5a754bf950`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:59 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:59 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:52:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:52:00 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:52:00 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112696cbcf76aafbed649fd17dbfa0f080e4d359e61aaf1ddcf827383495c48`  
		Last Modified: Wed, 31 Mar 2021 14:53:23 GMT  
		Size: 49.9 MB (49920031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6713d4822b777a4866e15acf049c80365d48446086028f5c4b074a922e0d0eb3`  
		Last Modified: Wed, 31 Mar 2021 14:53:12 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:5487e5e58e759161e312012a6462d44f8dab8d213b0603fdb2fa4cb70698f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:d4abd66ef8b965ad4cb096eeebdd75d08c0a4aef6117f30e31c23163c1c81a3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77059798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67b0a95f13ffdef60c680f96ed61e2e6b3751a58f4c0e175864fe5a754bf950`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Wed, 31 Mar 2021 14:51:39 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:58 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:59 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:59 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:52:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:52:00 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:52:00 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112696cbcf76aafbed649fd17dbfa0f080e4d359e61aaf1ddcf827383495c48`  
		Last Modified: Wed, 31 Mar 2021 14:53:23 GMT  
		Size: 49.9 MB (49920031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6713d4822b777a4866e15acf049c80365d48446086028f5c4b074a922e0d0eb3`  
		Last Modified: Wed, 31 Mar 2021 14:53:12 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:624274b979dfdeac99282c8554f8ccd6d5a1dd632f8f2ad34b24ac842810424d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:d2044aeaf884d0b82f37eeb0090782bd1db1c2c3fbd211226869a0afb2962603
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76475169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c770719f0f812ac70fd0136322ff72f316da9e9cb9fb95cfc335ef4d4e1130b`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:51:09 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 31 Mar 2021 14:51:09 GMT
ENV VARNISH_SIZE=100M
# Wed, 31 Mar 2021 14:51:32 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:33 GMT
WORKDIR /etc/varnish
# Wed, 31 Mar 2021 14:51:33 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Wed, 31 Mar 2021 14:51:33 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 31 Mar 2021 14:51:33 GMT
EXPOSE 80 8443
# Wed, 31 Mar 2021 14:51:34 GMT
CMD []
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa58409cf19198895096d632959a96f0d681a94bb34765b872de0770863954`  
		Last Modified: Wed, 31 Mar 2021 14:52:57 GMT  
		Size: 49.3 MB (49335404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bacb4bec39431045e9289ccc4f82e05a5f3425589cdd689a1db527c204aaf1`  
		Last Modified: Wed, 31 Mar 2021 14:52:48 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
