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
$ docker pull varnish@sha256:8cf38287c290c9d68300b5b396c6a8db796a55a5fdb8a912dfab5eae709c854f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:abbe9f98f1c26796a2014fc559d30be444b9039f5035f8e6dd96bfe07f872343
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f88e08735c4645e54cb279987d3b4dabe6a2d25f125da671e007bbb4eb337e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Mar 2021 01:30:38 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Mar 2021 01:30:38 GMT
WORKDIR /etc/varnish
# Tue, 23 Mar 2021 01:30:39 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 23 Mar 2021 01:30:39 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 23 Mar 2021 01:30:39 GMT
EXPOSE 80 8443
# Tue, 23 Mar 2021 01:30:39 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05740eb791f9a263fc983f531f772cc92536f0f328e8ed09069136937c7dab00`  
		Last Modified: Tue, 23 Mar 2021 01:31:08 GMT  
		Size: 49.9 MB (49919058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ad7f3b793d6b86898063f4a21a5d5112c25af58e5c71368f95f5f0344409b`  
		Last Modified: Tue, 23 Mar 2021 01:30:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:a70a468921ac85e0e06444e9ce25c0f82309ed0fb1db1d7aa3e6a14bb656a32f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:591464b58aa1c8ae4751be624c27183b6953e5ecc1ff56565920f79b231c7017
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76436404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ddb990c77eb5996ec93594336d258dd4bbeed91104b1d360ad6087f0cee7500`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:25:50 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Fri, 12 Mar 2021 13:25:50 GMT
ENV VARNISH_SIZE=100M
# Fri, 12 Mar 2021 13:26:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:26:11 GMT
WORKDIR /etc/varnish
# Fri, 12 Mar 2021 13:26:11 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:26:11 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 12 Mar 2021 13:26:11 GMT
EXPOSE 80 8443
# Fri, 12 Mar 2021 13:26:11 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9721349da7a0563c16e4e23a5fe2eb51a0251dddba34a34e4ccc2ba91612fa4a`  
		Last Modified: Fri, 12 Mar 2021 13:27:03 GMT  
		Size: 49.3 MB (49334930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e9d59fffbb7967db9eb5679f4e1453cf0dfe704ca15f59a1557e7b54ed646e`  
		Last Modified: Fri, 12 Mar 2021 13:26:54 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7`

```console
$ docker pull varnish@sha256:a70a468921ac85e0e06444e9ce25c0f82309ed0fb1db1d7aa3e6a14bb656a32f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.7` - linux; amd64

```console
$ docker pull varnish@sha256:591464b58aa1c8ae4751be624c27183b6953e5ecc1ff56565920f79b231c7017
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76436404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ddb990c77eb5996ec93594336d258dd4bbeed91104b1d360ad6087f0cee7500`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:25:50 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Fri, 12 Mar 2021 13:25:50 GMT
ENV VARNISH_SIZE=100M
# Fri, 12 Mar 2021 13:26:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:26:11 GMT
WORKDIR /etc/varnish
# Fri, 12 Mar 2021 13:26:11 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:26:11 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 12 Mar 2021 13:26:11 GMT
EXPOSE 80 8443
# Fri, 12 Mar 2021 13:26:11 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9721349da7a0563c16e4e23a5fe2eb51a0251dddba34a34e4ccc2ba91612fa4a`  
		Last Modified: Fri, 12 Mar 2021 13:27:03 GMT  
		Size: 49.3 MB (49334930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e9d59fffbb7967db9eb5679f4e1453cf0dfe704ca15f59a1557e7b54ed646e`  
		Last Modified: Fri, 12 Mar 2021 13:26:54 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.7-1`

```console
$ docker pull varnish@sha256:a70a468921ac85e0e06444e9ce25c0f82309ed0fb1db1d7aa3e6a14bb656a32f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.7-1` - linux; amd64

```console
$ docker pull varnish@sha256:591464b58aa1c8ae4751be624c27183b6953e5ecc1ff56565920f79b231c7017
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76436404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ddb990c77eb5996ec93594336d258dd4bbeed91104b1d360ad6087f0cee7500`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:25:50 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Fri, 12 Mar 2021 13:25:50 GMT
ENV VARNISH_SIZE=100M
# Fri, 12 Mar 2021 13:26:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:26:11 GMT
WORKDIR /etc/varnish
# Fri, 12 Mar 2021 13:26:11 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:26:11 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 12 Mar 2021 13:26:11 GMT
EXPOSE 80 8443
# Fri, 12 Mar 2021 13:26:11 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9721349da7a0563c16e4e23a5fe2eb51a0251dddba34a34e4ccc2ba91612fa4a`  
		Last Modified: Fri, 12 Mar 2021 13:27:03 GMT  
		Size: 49.3 MB (49334930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e9d59fffbb7967db9eb5679f4e1453cf0dfe704ca15f59a1557e7b54ed646e`  
		Last Modified: Fri, 12 Mar 2021 13:26:54 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5`

```console
$ docker pull varnish@sha256:9f1c24b270e55593b90fe1df8d9d6c362b2245920d4b333f78884c750132a2bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5` - linux; amd64

```console
$ docker pull varnish@sha256:a380432303cb98600baa08631bf02dc86851b9ef041b99e082d298917b758632
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76888069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7981e048587a3dc4de75b2784c69ff5527e013a6e94e344fd2d6cc909b55e3`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:26:16 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Fri, 12 Mar 2021 13:26:16 GMT
ENV VARNISH_SIZE=100M
# Fri, 12 Mar 2021 13:26:35 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:26:35 GMT
WORKDIR /etc/varnish
# Fri, 12 Mar 2021 13:26:36 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:26:36 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 12 Mar 2021 13:26:36 GMT
EXPOSE 80 8443
# Fri, 12 Mar 2021 13:26:36 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079d8de6a483fd51ca3aad58d60d5051eea62daac4bb34349db218d9e0a93a5d`  
		Last Modified: Fri, 12 Mar 2021 13:27:28 GMT  
		Size: 49.8 MB (49786594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8bfd49ee0a64d81548dcf9b7fa07bc62ca78c158e19e2c1a1379188a1d9ebe`  
		Last Modified: Fri, 12 Mar 2021 13:27:18 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1`

```console
$ docker pull varnish@sha256:9f1c24b270e55593b90fe1df8d9d6c362b2245920d4b333f78884c750132a2bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1` - linux; amd64

```console
$ docker pull varnish@sha256:a380432303cb98600baa08631bf02dc86851b9ef041b99e082d298917b758632
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76888069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7981e048587a3dc4de75b2784c69ff5527e013a6e94e344fd2d6cc909b55e3`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:26:16 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Fri, 12 Mar 2021 13:26:16 GMT
ENV VARNISH_SIZE=100M
# Fri, 12 Mar 2021 13:26:35 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:26:35 GMT
WORKDIR /etc/varnish
# Fri, 12 Mar 2021 13:26:36 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:26:36 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 12 Mar 2021 13:26:36 GMT
EXPOSE 80 8443
# Fri, 12 Mar 2021 13:26:36 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079d8de6a483fd51ca3aad58d60d5051eea62daac4bb34349db218d9e0a93a5d`  
		Last Modified: Fri, 12 Mar 2021 13:27:28 GMT  
		Size: 49.8 MB (49786594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8bfd49ee0a64d81548dcf9b7fa07bc62ca78c158e19e2c1a1379188a1d9ebe`  
		Last Modified: Fri, 12 Mar 2021 13:27:18 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.5.1-1`

```console
$ docker pull varnish@sha256:9f1c24b270e55593b90fe1df8d9d6c362b2245920d4b333f78884c750132a2bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.5.1-1` - linux; amd64

```console
$ docker pull varnish@sha256:a380432303cb98600baa08631bf02dc86851b9ef041b99e082d298917b758632
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76888069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7981e048587a3dc4de75b2784c69ff5527e013a6e94e344fd2d6cc909b55e3`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:26:16 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Fri, 12 Mar 2021 13:26:16 GMT
ENV VARNISH_SIZE=100M
# Fri, 12 Mar 2021 13:26:35 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:26:35 GMT
WORKDIR /etc/varnish
# Fri, 12 Mar 2021 13:26:36 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:26:36 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 12 Mar 2021 13:26:36 GMT
EXPOSE 80 8443
# Fri, 12 Mar 2021 13:26:36 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079d8de6a483fd51ca3aad58d60d5051eea62daac4bb34349db218d9e0a93a5d`  
		Last Modified: Fri, 12 Mar 2021 13:27:28 GMT  
		Size: 49.8 MB (49786594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8bfd49ee0a64d81548dcf9b7fa07bc62ca78c158e19e2c1a1379188a1d9ebe`  
		Last Modified: Fri, 12 Mar 2021 13:27:18 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6`

```console
$ docker pull varnish@sha256:8cf38287c290c9d68300b5b396c6a8db796a55a5fdb8a912dfab5eae709c854f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.6` - linux; amd64

```console
$ docker pull varnish@sha256:abbe9f98f1c26796a2014fc559d30be444b9039f5035f8e6dd96bfe07f872343
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f88e08735c4645e54cb279987d3b4dabe6a2d25f125da671e007bbb4eb337e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Mar 2021 01:30:38 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Mar 2021 01:30:38 GMT
WORKDIR /etc/varnish
# Tue, 23 Mar 2021 01:30:39 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 23 Mar 2021 01:30:39 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 23 Mar 2021 01:30:39 GMT
EXPOSE 80 8443
# Tue, 23 Mar 2021 01:30:39 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05740eb791f9a263fc983f531f772cc92536f0f328e8ed09069136937c7dab00`  
		Last Modified: Tue, 23 Mar 2021 01:31:08 GMT  
		Size: 49.9 MB (49919058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ad7f3b793d6b86898063f4a21a5d5112c25af58e5c71368f95f5f0344409b`  
		Last Modified: Tue, 23 Mar 2021 01:30:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.0`

```console
$ docker pull varnish@sha256:8cf38287c290c9d68300b5b396c6a8db796a55a5fdb8a912dfab5eae709c854f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.6.0` - linux; amd64

```console
$ docker pull varnish@sha256:abbe9f98f1c26796a2014fc559d30be444b9039f5035f8e6dd96bfe07f872343
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f88e08735c4645e54cb279987d3b4dabe6a2d25f125da671e007bbb4eb337e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Mar 2021 01:30:38 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Mar 2021 01:30:38 GMT
WORKDIR /etc/varnish
# Tue, 23 Mar 2021 01:30:39 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 23 Mar 2021 01:30:39 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 23 Mar 2021 01:30:39 GMT
EXPOSE 80 8443
# Tue, 23 Mar 2021 01:30:39 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05740eb791f9a263fc983f531f772cc92536f0f328e8ed09069136937c7dab00`  
		Last Modified: Tue, 23 Mar 2021 01:31:08 GMT  
		Size: 49.9 MB (49919058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ad7f3b793d6b86898063f4a21a5d5112c25af58e5c71368f95f5f0344409b`  
		Last Modified: Tue, 23 Mar 2021 01:30:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.0-1`

```console
$ docker pull varnish@sha256:8cf38287c290c9d68300b5b396c6a8db796a55a5fdb8a912dfab5eae709c854f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.6.0-1` - linux; amd64

```console
$ docker pull varnish@sha256:abbe9f98f1c26796a2014fc559d30be444b9039f5035f8e6dd96bfe07f872343
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f88e08735c4645e54cb279987d3b4dabe6a2d25f125da671e007bbb4eb337e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Mar 2021 01:30:38 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Mar 2021 01:30:38 GMT
WORKDIR /etc/varnish
# Tue, 23 Mar 2021 01:30:39 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 23 Mar 2021 01:30:39 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 23 Mar 2021 01:30:39 GMT
EXPOSE 80 8443
# Tue, 23 Mar 2021 01:30:39 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05740eb791f9a263fc983f531f772cc92536f0f328e8ed09069136937c7dab00`  
		Last Modified: Tue, 23 Mar 2021 01:31:08 GMT  
		Size: 49.9 MB (49919058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ad7f3b793d6b86898063f4a21a5d5112c25af58e5c71368f95f5f0344409b`  
		Last Modified: Tue, 23 Mar 2021 01:30:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:8cf38287c290c9d68300b5b396c6a8db796a55a5fdb8a912dfab5eae709c854f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:abbe9f98f1c26796a2014fc559d30be444b9039f5035f8e6dd96bfe07f872343
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f88e08735c4645e54cb279987d3b4dabe6a2d25f125da671e007bbb4eb337e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Mar 2021 01:30:38 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Mar 2021 01:30:38 GMT
WORKDIR /etc/varnish
# Tue, 23 Mar 2021 01:30:39 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 23 Mar 2021 01:30:39 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 23 Mar 2021 01:30:39 GMT
EXPOSE 80 8443
# Tue, 23 Mar 2021 01:30:39 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05740eb791f9a263fc983f531f772cc92536f0f328e8ed09069136937c7dab00`  
		Last Modified: Tue, 23 Mar 2021 01:31:08 GMT  
		Size: 49.9 MB (49919058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ad7f3b793d6b86898063f4a21a5d5112c25af58e5c71368f95f5f0344409b`  
		Last Modified: Tue, 23 Mar 2021 01:30:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:8cf38287c290c9d68300b5b396c6a8db796a55a5fdb8a912dfab5eae709c854f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:abbe9f98f1c26796a2014fc559d30be444b9039f5035f8e6dd96bfe07f872343
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f88e08735c4645e54cb279987d3b4dabe6a2d25f125da671e007bbb4eb337e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Mar 2021 01:30:38 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Mar 2021 01:30:38 GMT
WORKDIR /etc/varnish
# Tue, 23 Mar 2021 01:30:39 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 23 Mar 2021 01:30:39 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 23 Mar 2021 01:30:39 GMT
EXPOSE 80 8443
# Tue, 23 Mar 2021 01:30:39 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05740eb791f9a263fc983f531f772cc92536f0f328e8ed09069136937c7dab00`  
		Last Modified: Tue, 23 Mar 2021 01:31:08 GMT  
		Size: 49.9 MB (49919058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ad7f3b793d6b86898063f4a21a5d5112c25af58e5c71368f95f5f0344409b`  
		Last Modified: Tue, 23 Mar 2021 01:30:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:a70a468921ac85e0e06444e9ce25c0f82309ed0fb1db1d7aa3e6a14bb656a32f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:591464b58aa1c8ae4751be624c27183b6953e5ecc1ff56565920f79b231c7017
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76436404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ddb990c77eb5996ec93594336d258dd4bbeed91104b1d360ad6087f0cee7500`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:25:50 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Fri, 12 Mar 2021 13:25:50 GMT
ENV VARNISH_SIZE=100M
# Fri, 12 Mar 2021 13:26:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:26:11 GMT
WORKDIR /etc/varnish
# Fri, 12 Mar 2021 13:26:11 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:26:11 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 12 Mar 2021 13:26:11 GMT
EXPOSE 80 8443
# Fri, 12 Mar 2021 13:26:11 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9721349da7a0563c16e4e23a5fe2eb51a0251dddba34a34e4ccc2ba91612fa4a`  
		Last Modified: Fri, 12 Mar 2021 13:27:03 GMT  
		Size: 49.3 MB (49334930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e9d59fffbb7967db9eb5679f4e1453cf0dfe704ca15f59a1557e7b54ed646e`  
		Last Modified: Fri, 12 Mar 2021 13:26:54 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
