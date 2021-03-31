<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1.6.1`](#spiped161)
-	[`spiped:1.6.1-alpine`](#spiped161-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:dc5f5f896cc7441fb4676b3aa5a911dac58aca8762ebbfb936e79ede5e376367
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:280bdf816a8f0ce321d66c5a765695190a9c3edbbd8af313d70b5fd047cf0cce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36268964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:177e254b3165eba26156c945f4dd0bcb1294728c43424187b5216211524d404e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:33:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 09:33:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:33:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 09:33:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 09:33:35 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 09:33:35 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 09:33:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 09:33:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 09:33:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372a623e820848080246423f9522d76632fd56ebd9e7cbcc3e2667c4b0379a88`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791b1741aa3b0fd443ebcc5a2f2a6b735a3ea18414dec574b0c61762a240137`  
		Last Modified: Sat, 27 Mar 2021 09:33:54 GMT  
		Size: 2.1 MB (2128524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44955b5b9fc6dbfc59ba93dc9add40129c020cf760eb35202c7bc09a7975985`  
		Last Modified: Sat, 27 Mar 2021 09:33:57 GMT  
		Size: 7.0 MB (7037245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed155aee7ced703085049efda143c0b629962d415f08d6e885d66fd6b4c4eb61`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8de1bcbffcf9f5c4958ddb3025efacc91c14296edb9b078aa73fcc2f011de14`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2e00324da21253f7f0beedc1d2a123fa5efbc0e732f32044159d733abe700a17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1314e5a5cb457b2a8772a9ab8d7b1c83e9190f6c1b920601a114714ef5b080e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:36:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 01:37:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:37:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 01:37:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 01:38:00 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 01:38:02 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 01:38:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 01:38:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28182091d78cadb3063bdd9ce75c263b768f3a24453ab10eeef8d29081a26b52`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa81838cd994f801fc7d925cf1700aa43b15f134a749eac7d4a4da60a15a175e`  
		Last Modified: Wed, 31 Mar 2021 01:38:24 GMT  
		Size: 1.8 MB (1839326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b00960d8e0c9e05dc7343b699974e653177c263af4f99f3f849b4062226ddf`  
		Last Modified: Wed, 31 Mar 2021 01:38:23 GMT  
		Size: 5.5 MB (5479910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0df0d7972be414ec17fc2d27808177f0e968261e2abc699a4ddea72869042`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed60abb976ac8333612b838e368cffd3ccb982d68fed535f5b555d86cb0e6ed`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b32775847daf03e28d6505b2efe6e3f13e6c861418c1d19cb03953193dfd095
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29756781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c71a26ce499550c85d6ff57d5bc1454d0cd7582bf67d215918c27ef2b87fcf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 11:17:38 GMT
ADD file:911acc83e6d3d4b00ecc59effce9e5ab69d62aa3e77a24db76e270db8cedce5f in / 
# Fri, 26 Mar 2021 11:17:39 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:35:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 05:35:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:35:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 05:36:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 05:36:09 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 05:36:10 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 05:36:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 05:36:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:36:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05a8be0db5eb6dbb349e49a01211d3a11adc23881f696760a058c0c8ae8e39b7`  
		Last Modified: Fri, 26 Mar 2021 11:27:34 GMT  
		Size: 22.7 MB (22709509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8740734e875c6119761eaa450ddf86492e161c3ba189bb7a553228675739490a`  
		Last Modified: Sat, 27 Mar 2021 05:36:37 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41322223cb0db7b2f85b4ce782bded120e746ec956a59b711c3a94efefb21201`  
		Last Modified: Sat, 27 Mar 2021 05:36:38 GMT  
		Size: 1.8 MB (1759472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4fc89e05f2e726a42d86b61ece624ed80a3325daa509925e7af84d886284ab`  
		Last Modified: Sat, 27 Mar 2021 05:36:40 GMT  
		Size: 5.3 MB (5285595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3fb1951ae5521b62f63897078966f06bbd4b671a84e23feb40b9ed8ed2a51`  
		Last Modified: Sat, 27 Mar 2021 05:36:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca730b0805353a00e92749eb1dcf1b63bf134359024f20d27a2d5ec0e5a574e`  
		Last Modified: Sat, 27 Mar 2021 05:36:38 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0e3bf42a5f79b5c00bf96b4263f861de2095043a5af73c8973a8d9a12edd7401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117933bd3e53f5572f06d07dc3be9201199feebe0e59f35880fb08d848df320f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:05:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 09:05:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:05:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 09:06:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 09:06:18 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 09:06:19 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 09:06:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 09:06:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 09:06:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73432000cbf913494b2dd2895431780fb24c5de87b4116dc4120208afeb895d4`  
		Last Modified: Sat, 27 Mar 2021 09:06:48 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca8b7a8ebcb36d0f266af5caa12326b78384982ff7b407c5bbb184588ea191`  
		Last Modified: Sat, 27 Mar 2021 09:06:49 GMT  
		Size: 2.0 MB (2007872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7978c28ef3edd4ebe57f3893e93deb88a5383143db5999487fb12384ce0996a7`  
		Last Modified: Sat, 27 Mar 2021 09:06:50 GMT  
		Size: 5.9 MB (5905343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd38d1ecd49b461de15549f7b257a299e4c9f1a13dbb15adcdf758c44dafd7e`  
		Last Modified: Sat, 27 Mar 2021 09:06:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2530fb66cc23163412987920279774b1da7169ab73501a343e24c3b797fa4c`  
		Last Modified: Sat, 27 Mar 2021 09:06:48 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:c7b62ea34691dc2c5a699b708d4a0582923a757ad9b41a6b5c9ed012455e6aba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bd5250a469ba27b4d7a5c6f483a6dec8e967d14cad2362ce98bfbd924ae446`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 00:27:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:27:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 00:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:28:18 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 00:28:18 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 00:28:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:28:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 00:28:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db59fb742889351c8257d71d9af7f8ab754780dfdb80e60bb34a5488afc26249`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2479ba868a69059ce8416072149d301726c919056b2d354373c241954b855dab`  
		Last Modified: Wed, 31 Mar 2021 00:29:13 GMT  
		Size: 2.1 MB (2132647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7d122183831a8ed76e681eeb8ead7cf5f075914d4386bf5fb20dcf081064fa`  
		Last Modified: Wed, 31 Mar 2021 00:29:20 GMT  
		Size: 11.6 MB (11633214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdfcb59f4fbfed086e7dc5075c6db916e00188a042b7612c5f03252f5eda4f6`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645a8c57aa0c862e9773fc2240ce6dcc565e9100a5223a0f67eb77140507ccf`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:7c7c058360198a6cdf1c0c5de4c7536b662d0aadb492a39eb71da1745ec6ead9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2e30091907d1d9785d74152c96711b6ea697670f5b2e51c2fef7e50032815e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:56 GMT
ADD file:74d504a9a34f47729165ef4ceedc9f0eaa2e91bfb6a24ebfc3ceed0248267a27 in / 
# Fri, 26 Mar 2021 08:09:57 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:56:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:56:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:57:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:57:54 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:57:54 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:57:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:57:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f863e006c40853ec8c23aa5b7a0e95918001f96878fb45770410ac4df51cf88`  
		Last Modified: Fri, 26 Mar 2021 08:16:29 GMT  
		Size: 25.8 MB (25772487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920815f459af869c2bafde850a4833f2c0af39a10540924371f7c810a2740698`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecefc467b0208174c90913c171e0635fc983fe0271e56d94814d9365402d9a`  
		Last Modified: Fri, 26 Mar 2021 18:58:21 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946d42bf9e7b59ba6752c87e806b5dfbcaab31bb0b4c62ad64e1106e2806bb5`  
		Last Modified: Fri, 26 Mar 2021 18:58:26 GMT  
		Size: 6.4 MB (6416271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bca10ef1481bbdde6f3709e04eb5245089e289de05b36095d3c0b7cd7d5a32`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbf9a1588f37aee944ed6e518b80a6c1c787fe4b75da67bfd3b3f191544931e`  
		Last Modified: Fri, 26 Mar 2021 18:58:23 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:9f6d20d1daa6cd853c2829541ecbd642ac3de0a47b6ba6d09aec3b064a882007
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccb828b29ef1c5d8e88d454ac3307b2607e7d07a516b3a6028fe00e30aea8116`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:14:22 GMT
ADD file:feb26657639018f8f43408e43e8ecec7e84632f33b42d5521241b842b58747d5 in / 
# Fri, 26 Mar 2021 15:14:28 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 16:36:00 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 16:36:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 16:36:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 16:40:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 16:40:38 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 16:40:41 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 16:40:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 16:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 16:40:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:035681ea37d9aab4545aa2211af3bf79addea316f71afde84412406734ef8a85`  
		Last Modified: Fri, 26 Mar 2021 15:22:05 GMT  
		Size: 30.5 MB (30525677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3001f02c630196b6d34866a51640bb423722404e58e6ec0dd89623c69ddc5f`  
		Last Modified: Sat, 27 Mar 2021 16:41:14 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2204248b5fcb9625e734191b9113a495608d92eca33cf00bd9b4d1d7a5ca8e5`  
		Last Modified: Sat, 27 Mar 2021 16:41:15 GMT  
		Size: 2.2 MB (2225167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08edb758e4fd44b9b6c53de4bc3867a35c3611d94678664bb443687ffdc898f3`  
		Last Modified: Sat, 27 Mar 2021 16:41:17 GMT  
		Size: 6.7 MB (6743526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc132087dda4152235c0aac9f32757e35db7c6e3958fee5627a67a81d573e214`  
		Last Modified: Sat, 27 Mar 2021 16:41:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676f92e18e0d0b6e112f621b4f69817f837335a26a2852bc7fddafeed10f56`  
		Last Modified: Sat, 27 Mar 2021 16:41:14 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:97d3bd125ab186461612f5227612b8bed1b7cdf339597a848150b8abb1df9748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11acca930a3acc9f10aec0e92255da2f3d7782c440d9ebe986775b5d784b5f7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 02:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 02:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 02:25:46 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 02:25:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 02:25:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 02:25:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 02:25:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c742a04892cc406ec636d3b61ae8b30ea2be9d8094b04a3e6fa844006600bb`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee293ba212f1e0d102b980847b925882c507858cf70dd83eca37c45fb14d8fb6`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 1.8 MB (1821969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048c0826dbbe30eb38c444743a578a8400ca9bb488e6dd498c2ae0c74a524ba`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 5.9 MB (5943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8fc932e810d22ad352fd6f592c4c76a7e0fc36211bb96549e2044049a0ae6c`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd24c1b830fe7b47376748fdbcf9a99c29e655cc7047927ab24e2aad8d1cf83`  
		Last Modified: Wed, 31 Mar 2021 02:26:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:19684fbf0023be921667a91a92d2cf6e979393817c9e69f7062aa2bb5bd5d5e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:da8bf89069f02c44e64a52cd3c311da57833ba52c0dfd401bf5b400bcba42fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6928a48d8b494975b09a73ff31d4ec85bbf1a70eb5240a267316a1495d85c91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:26:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 10:26:10 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 10:26:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 10:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 10:26:43 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 10:26:44 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 10:26:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:26:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05731027fa533b4ddfd5253b33af7f2e6329040d608478a1cf595d3594e504fd`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c330cdff7f6294e87be781c7a86aac39a7e7d2431c24def9e8af9476e2c7da`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7422b39d0efd63a811763e22eb91fcaa0ea348b8a13c6a2afd70562f5cb9bb89`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641ca636eaa042a42ed82a4494fe4030af9725300ffdc103faa9e12ce1a3816a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f1740d604bc2886348af7061a47d9a4343057827419e05f23191d5b911a3a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6d4e4fe6948e5a7992c124e61fa437b6e0413a5bb3401654fb248eb3cb12d114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c19db803961bd8dcd8229779fef2771123c1e74079d8339d813fcec140a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:35:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 11:35:31 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 11:35:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 11:35:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 11:35:53 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 11:35:53 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 11:35:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:35:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:35:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e02a3b4bec768000b32f6cd554e24e6c8494cbd013299b945dfba9976453`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be889af3bc0980bb5b61ae0b456dbd90907f154b74b796a26046e96f70c4f6`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a408cdd7892cb9e528cde840b9bf4c2457e6b9540f7b3eeba4b75bb22d5729`  
		Last Modified: Fri, 26 Mar 2021 11:36:26 GMT  
		Size: 223.3 KB (223278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb962d5a258d79b6a952f2eb3e3c6f8e4497529c9b722d855f051a120a68c0`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c91539d601c2ba091818f38b8b0b17362626aca4e30ca053825d5b4920cbe`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:90360f53f918820e5f6a844dee0754fa75b275607dbe5c71293fd0e7af7797c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f4df11bdbbf450f4e6fbf2b9bd4b57d9432205d415896d1ec7179a79658764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:46:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 05:47:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 05:47:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 05:47:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 05:47:57 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 05:48:02 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 05:48:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 05:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:48:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ade0bad869d6db8a4e76203a6dfe3818480c33c407956be758da40b7da8e87`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6878fc6b1c7c9ff2cb9cd6603daa1608abf9847d920dbc2a975313b81d54d09`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e8e86fc5762fedfcc865b9618a77f7c27214bf2068e2bdb0f7151d8964030`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 221.0 KB (220985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956adc5bd10550d52ee7f60d1d249008d2ca8b414e697b229923777c89fffae`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dac4482b42db1364dec4448343ae95036dd4f7b02440507ae3e40da8dc0d43`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c1f0c63244642a743f32f026370285292f3dae250a308e6364fc3de8ab05effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d526ff26ded3a191cd728d6ee4458ac19061aadfef60a349e786aab31ba72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:56:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 25 Mar 2021 23:56:54 GMT
RUN apk add --no-cache libssl1.1
# Thu, 25 Mar 2021 23:56:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 25 Mar 2021 23:57:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 25 Mar 2021 23:57:06 GMT
VOLUME [/spiped]
# Thu, 25 Mar 2021 23:57:06 GMT
WORKDIR /spiped
# Thu, 25 Mar 2021 23:57:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:57:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d211148772ab04d0ac7d6a254412fe1f42c1e2e7015b60b873a95da6f14a452`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9963e2f655c56703f1a6c0ddfe5ddd34f7f2725e4b4dadfe50a44dccb3fabbef`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd16cb6da0cae4c5ecfe500cf635456f5c13193987be355c858e78a57bf1150`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463e1d0912abda7c19a7c110819c8a1b49e67d57f21ab80715f4a0ee1664927a`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48866150c20dea94d44784f072b65bdf6f2292cc61d11de364bbe2d47f21ecce`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:dc5f5f896cc7441fb4676b3aa5a911dac58aca8762ebbfb936e79ede5e376367
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:280bdf816a8f0ce321d66c5a765695190a9c3edbbd8af313d70b5fd047cf0cce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36268964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:177e254b3165eba26156c945f4dd0bcb1294728c43424187b5216211524d404e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:33:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 09:33:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:33:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 09:33:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 09:33:35 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 09:33:35 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 09:33:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 09:33:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 09:33:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372a623e820848080246423f9522d76632fd56ebd9e7cbcc3e2667c4b0379a88`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791b1741aa3b0fd443ebcc5a2f2a6b735a3ea18414dec574b0c61762a240137`  
		Last Modified: Sat, 27 Mar 2021 09:33:54 GMT  
		Size: 2.1 MB (2128524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44955b5b9fc6dbfc59ba93dc9add40129c020cf760eb35202c7bc09a7975985`  
		Last Modified: Sat, 27 Mar 2021 09:33:57 GMT  
		Size: 7.0 MB (7037245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed155aee7ced703085049efda143c0b629962d415f08d6e885d66fd6b4c4eb61`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8de1bcbffcf9f5c4958ddb3025efacc91c14296edb9b078aa73fcc2f011de14`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2e00324da21253f7f0beedc1d2a123fa5efbc0e732f32044159d733abe700a17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1314e5a5cb457b2a8772a9ab8d7b1c83e9190f6c1b920601a114714ef5b080e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:36:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 01:37:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:37:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 01:37:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 01:38:00 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 01:38:02 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 01:38:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 01:38:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28182091d78cadb3063bdd9ce75c263b768f3a24453ab10eeef8d29081a26b52`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa81838cd994f801fc7d925cf1700aa43b15f134a749eac7d4a4da60a15a175e`  
		Last Modified: Wed, 31 Mar 2021 01:38:24 GMT  
		Size: 1.8 MB (1839326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b00960d8e0c9e05dc7343b699974e653177c263af4f99f3f849b4062226ddf`  
		Last Modified: Wed, 31 Mar 2021 01:38:23 GMT  
		Size: 5.5 MB (5479910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0df0d7972be414ec17fc2d27808177f0e968261e2abc699a4ddea72869042`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed60abb976ac8333612b838e368cffd3ccb982d68fed535f5b555d86cb0e6ed`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b32775847daf03e28d6505b2efe6e3f13e6c861418c1d19cb03953193dfd095
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29756781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c71a26ce499550c85d6ff57d5bc1454d0cd7582bf67d215918c27ef2b87fcf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 11:17:38 GMT
ADD file:911acc83e6d3d4b00ecc59effce9e5ab69d62aa3e77a24db76e270db8cedce5f in / 
# Fri, 26 Mar 2021 11:17:39 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:35:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 05:35:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:35:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 05:36:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 05:36:09 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 05:36:10 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 05:36:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 05:36:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:36:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05a8be0db5eb6dbb349e49a01211d3a11adc23881f696760a058c0c8ae8e39b7`  
		Last Modified: Fri, 26 Mar 2021 11:27:34 GMT  
		Size: 22.7 MB (22709509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8740734e875c6119761eaa450ddf86492e161c3ba189bb7a553228675739490a`  
		Last Modified: Sat, 27 Mar 2021 05:36:37 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41322223cb0db7b2f85b4ce782bded120e746ec956a59b711c3a94efefb21201`  
		Last Modified: Sat, 27 Mar 2021 05:36:38 GMT  
		Size: 1.8 MB (1759472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4fc89e05f2e726a42d86b61ece624ed80a3325daa509925e7af84d886284ab`  
		Last Modified: Sat, 27 Mar 2021 05:36:40 GMT  
		Size: 5.3 MB (5285595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3fb1951ae5521b62f63897078966f06bbd4b671a84e23feb40b9ed8ed2a51`  
		Last Modified: Sat, 27 Mar 2021 05:36:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca730b0805353a00e92749eb1dcf1b63bf134359024f20d27a2d5ec0e5a574e`  
		Last Modified: Sat, 27 Mar 2021 05:36:38 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0e3bf42a5f79b5c00bf96b4263f861de2095043a5af73c8973a8d9a12edd7401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117933bd3e53f5572f06d07dc3be9201199feebe0e59f35880fb08d848df320f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:05:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 09:05:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:05:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 09:06:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 09:06:18 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 09:06:19 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 09:06:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 09:06:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 09:06:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73432000cbf913494b2dd2895431780fb24c5de87b4116dc4120208afeb895d4`  
		Last Modified: Sat, 27 Mar 2021 09:06:48 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca8b7a8ebcb36d0f266af5caa12326b78384982ff7b407c5bbb184588ea191`  
		Last Modified: Sat, 27 Mar 2021 09:06:49 GMT  
		Size: 2.0 MB (2007872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7978c28ef3edd4ebe57f3893e93deb88a5383143db5999487fb12384ce0996a7`  
		Last Modified: Sat, 27 Mar 2021 09:06:50 GMT  
		Size: 5.9 MB (5905343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd38d1ecd49b461de15549f7b257a299e4c9f1a13dbb15adcdf758c44dafd7e`  
		Last Modified: Sat, 27 Mar 2021 09:06:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2530fb66cc23163412987920279774b1da7169ab73501a343e24c3b797fa4c`  
		Last Modified: Sat, 27 Mar 2021 09:06:48 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:c7b62ea34691dc2c5a699b708d4a0582923a757ad9b41a6b5c9ed012455e6aba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bd5250a469ba27b4d7a5c6f483a6dec8e967d14cad2362ce98bfbd924ae446`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 00:27:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:27:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 00:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:28:18 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 00:28:18 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 00:28:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:28:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 00:28:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db59fb742889351c8257d71d9af7f8ab754780dfdb80e60bb34a5488afc26249`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2479ba868a69059ce8416072149d301726c919056b2d354373c241954b855dab`  
		Last Modified: Wed, 31 Mar 2021 00:29:13 GMT  
		Size: 2.1 MB (2132647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7d122183831a8ed76e681eeb8ead7cf5f075914d4386bf5fb20dcf081064fa`  
		Last Modified: Wed, 31 Mar 2021 00:29:20 GMT  
		Size: 11.6 MB (11633214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdfcb59f4fbfed086e7dc5075c6db916e00188a042b7612c5f03252f5eda4f6`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645a8c57aa0c862e9773fc2240ce6dcc565e9100a5223a0f67eb77140507ccf`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:7c7c058360198a6cdf1c0c5de4c7536b662d0aadb492a39eb71da1745ec6ead9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2e30091907d1d9785d74152c96711b6ea697670f5b2e51c2fef7e50032815e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:56 GMT
ADD file:74d504a9a34f47729165ef4ceedc9f0eaa2e91bfb6a24ebfc3ceed0248267a27 in / 
# Fri, 26 Mar 2021 08:09:57 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:56:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:56:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:57:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:57:54 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:57:54 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:57:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:57:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f863e006c40853ec8c23aa5b7a0e95918001f96878fb45770410ac4df51cf88`  
		Last Modified: Fri, 26 Mar 2021 08:16:29 GMT  
		Size: 25.8 MB (25772487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920815f459af869c2bafde850a4833f2c0af39a10540924371f7c810a2740698`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecefc467b0208174c90913c171e0635fc983fe0271e56d94814d9365402d9a`  
		Last Modified: Fri, 26 Mar 2021 18:58:21 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946d42bf9e7b59ba6752c87e806b5dfbcaab31bb0b4c62ad64e1106e2806bb5`  
		Last Modified: Fri, 26 Mar 2021 18:58:26 GMT  
		Size: 6.4 MB (6416271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bca10ef1481bbdde6f3709e04eb5245089e289de05b36095d3c0b7cd7d5a32`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbf9a1588f37aee944ed6e518b80a6c1c787fe4b75da67bfd3b3f191544931e`  
		Last Modified: Fri, 26 Mar 2021 18:58:23 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:9f6d20d1daa6cd853c2829541ecbd642ac3de0a47b6ba6d09aec3b064a882007
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccb828b29ef1c5d8e88d454ac3307b2607e7d07a516b3a6028fe00e30aea8116`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:14:22 GMT
ADD file:feb26657639018f8f43408e43e8ecec7e84632f33b42d5521241b842b58747d5 in / 
# Fri, 26 Mar 2021 15:14:28 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 16:36:00 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 16:36:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 16:36:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 16:40:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 16:40:38 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 16:40:41 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 16:40:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 16:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 16:40:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:035681ea37d9aab4545aa2211af3bf79addea316f71afde84412406734ef8a85`  
		Last Modified: Fri, 26 Mar 2021 15:22:05 GMT  
		Size: 30.5 MB (30525677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3001f02c630196b6d34866a51640bb423722404e58e6ec0dd89623c69ddc5f`  
		Last Modified: Sat, 27 Mar 2021 16:41:14 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2204248b5fcb9625e734191b9113a495608d92eca33cf00bd9b4d1d7a5ca8e5`  
		Last Modified: Sat, 27 Mar 2021 16:41:15 GMT  
		Size: 2.2 MB (2225167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08edb758e4fd44b9b6c53de4bc3867a35c3611d94678664bb443687ffdc898f3`  
		Last Modified: Sat, 27 Mar 2021 16:41:17 GMT  
		Size: 6.7 MB (6743526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc132087dda4152235c0aac9f32757e35db7c6e3958fee5627a67a81d573e214`  
		Last Modified: Sat, 27 Mar 2021 16:41:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676f92e18e0d0b6e112f621b4f69817f837335a26a2852bc7fddafeed10f56`  
		Last Modified: Sat, 27 Mar 2021 16:41:14 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:97d3bd125ab186461612f5227612b8bed1b7cdf339597a848150b8abb1df9748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11acca930a3acc9f10aec0e92255da2f3d7782c440d9ebe986775b5d784b5f7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 02:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 02:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 02:25:46 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 02:25:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 02:25:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 02:25:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 02:25:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c742a04892cc406ec636d3b61ae8b30ea2be9d8094b04a3e6fa844006600bb`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee293ba212f1e0d102b980847b925882c507858cf70dd83eca37c45fb14d8fb6`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 1.8 MB (1821969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048c0826dbbe30eb38c444743a578a8400ca9bb488e6dd498c2ae0c74a524ba`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 5.9 MB (5943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8fc932e810d22ad352fd6f592c4c76a7e0fc36211bb96549e2044049a0ae6c`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd24c1b830fe7b47376748fdbcf9a99c29e655cc7047927ab24e2aad8d1cf83`  
		Last Modified: Wed, 31 Mar 2021 02:26:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:19684fbf0023be921667a91a92d2cf6e979393817c9e69f7062aa2bb5bd5d5e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:da8bf89069f02c44e64a52cd3c311da57833ba52c0dfd401bf5b400bcba42fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6928a48d8b494975b09a73ff31d4ec85bbf1a70eb5240a267316a1495d85c91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:26:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 10:26:10 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 10:26:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 10:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 10:26:43 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 10:26:44 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 10:26:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:26:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05731027fa533b4ddfd5253b33af7f2e6329040d608478a1cf595d3594e504fd`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c330cdff7f6294e87be781c7a86aac39a7e7d2431c24def9e8af9476e2c7da`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7422b39d0efd63a811763e22eb91fcaa0ea348b8a13c6a2afd70562f5cb9bb89`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641ca636eaa042a42ed82a4494fe4030af9725300ffdc103faa9e12ce1a3816a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f1740d604bc2886348af7061a47d9a4343057827419e05f23191d5b911a3a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6d4e4fe6948e5a7992c124e61fa437b6e0413a5bb3401654fb248eb3cb12d114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c19db803961bd8dcd8229779fef2771123c1e74079d8339d813fcec140a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:35:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 11:35:31 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 11:35:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 11:35:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 11:35:53 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 11:35:53 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 11:35:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:35:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:35:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e02a3b4bec768000b32f6cd554e24e6c8494cbd013299b945dfba9976453`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be889af3bc0980bb5b61ae0b456dbd90907f154b74b796a26046e96f70c4f6`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a408cdd7892cb9e528cde840b9bf4c2457e6b9540f7b3eeba4b75bb22d5729`  
		Last Modified: Fri, 26 Mar 2021 11:36:26 GMT  
		Size: 223.3 KB (223278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb962d5a258d79b6a952f2eb3e3c6f8e4497529c9b722d855f051a120a68c0`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c91539d601c2ba091818f38b8b0b17362626aca4e30ca053825d5b4920cbe`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:90360f53f918820e5f6a844dee0754fa75b275607dbe5c71293fd0e7af7797c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f4df11bdbbf450f4e6fbf2b9bd4b57d9432205d415896d1ec7179a79658764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:46:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 05:47:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 05:47:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 05:47:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 05:47:57 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 05:48:02 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 05:48:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 05:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:48:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ade0bad869d6db8a4e76203a6dfe3818480c33c407956be758da40b7da8e87`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6878fc6b1c7c9ff2cb9cd6603daa1608abf9847d920dbc2a975313b81d54d09`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e8e86fc5762fedfcc865b9618a77f7c27214bf2068e2bdb0f7151d8964030`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 221.0 KB (220985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956adc5bd10550d52ee7f60d1d249008d2ca8b414e697b229923777c89fffae`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dac4482b42db1364dec4448343ae95036dd4f7b02440507ae3e40da8dc0d43`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c1f0c63244642a743f32f026370285292f3dae250a308e6364fc3de8ab05effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d526ff26ded3a191cd728d6ee4458ac19061aadfef60a349e786aab31ba72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:56:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 25 Mar 2021 23:56:54 GMT
RUN apk add --no-cache libssl1.1
# Thu, 25 Mar 2021 23:56:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 25 Mar 2021 23:57:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 25 Mar 2021 23:57:06 GMT
VOLUME [/spiped]
# Thu, 25 Mar 2021 23:57:06 GMT
WORKDIR /spiped
# Thu, 25 Mar 2021 23:57:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:57:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d211148772ab04d0ac7d6a254412fe1f42c1e2e7015b60b873a95da6f14a452`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9963e2f655c56703f1a6c0ddfe5ddd34f7f2725e4b4dadfe50a44dccb3fabbef`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd16cb6da0cae4c5ecfe500cf635456f5c13193987be355c858e78a57bf1150`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463e1d0912abda7c19a7c110819c8a1b49e67d57f21ab80715f4a0ee1664927a`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48866150c20dea94d44784f072b65bdf6f2292cc61d11de364bbe2d47f21ecce`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:dc5f5f896cc7441fb4676b3aa5a911dac58aca8762ebbfb936e79ede5e376367
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:280bdf816a8f0ce321d66c5a765695190a9c3edbbd8af313d70b5fd047cf0cce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36268964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:177e254b3165eba26156c945f4dd0bcb1294728c43424187b5216211524d404e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:33:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 09:33:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:33:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 09:33:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 09:33:35 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 09:33:35 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 09:33:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 09:33:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 09:33:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372a623e820848080246423f9522d76632fd56ebd9e7cbcc3e2667c4b0379a88`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791b1741aa3b0fd443ebcc5a2f2a6b735a3ea18414dec574b0c61762a240137`  
		Last Modified: Sat, 27 Mar 2021 09:33:54 GMT  
		Size: 2.1 MB (2128524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44955b5b9fc6dbfc59ba93dc9add40129c020cf760eb35202c7bc09a7975985`  
		Last Modified: Sat, 27 Mar 2021 09:33:57 GMT  
		Size: 7.0 MB (7037245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed155aee7ced703085049efda143c0b629962d415f08d6e885d66fd6b4c4eb61`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8de1bcbffcf9f5c4958ddb3025efacc91c14296edb9b078aa73fcc2f011de14`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2e00324da21253f7f0beedc1d2a123fa5efbc0e732f32044159d733abe700a17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1314e5a5cb457b2a8772a9ab8d7b1c83e9190f6c1b920601a114714ef5b080e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:36:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 01:37:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:37:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 01:37:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 01:38:00 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 01:38:02 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 01:38:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 01:38:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28182091d78cadb3063bdd9ce75c263b768f3a24453ab10eeef8d29081a26b52`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa81838cd994f801fc7d925cf1700aa43b15f134a749eac7d4a4da60a15a175e`  
		Last Modified: Wed, 31 Mar 2021 01:38:24 GMT  
		Size: 1.8 MB (1839326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b00960d8e0c9e05dc7343b699974e653177c263af4f99f3f849b4062226ddf`  
		Last Modified: Wed, 31 Mar 2021 01:38:23 GMT  
		Size: 5.5 MB (5479910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0df0d7972be414ec17fc2d27808177f0e968261e2abc699a4ddea72869042`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed60abb976ac8333612b838e368cffd3ccb982d68fed535f5b555d86cb0e6ed`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b32775847daf03e28d6505b2efe6e3f13e6c861418c1d19cb03953193dfd095
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29756781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c71a26ce499550c85d6ff57d5bc1454d0cd7582bf67d215918c27ef2b87fcf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 11:17:38 GMT
ADD file:911acc83e6d3d4b00ecc59effce9e5ab69d62aa3e77a24db76e270db8cedce5f in / 
# Fri, 26 Mar 2021 11:17:39 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:35:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 05:35:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:35:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 05:36:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 05:36:09 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 05:36:10 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 05:36:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 05:36:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:36:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05a8be0db5eb6dbb349e49a01211d3a11adc23881f696760a058c0c8ae8e39b7`  
		Last Modified: Fri, 26 Mar 2021 11:27:34 GMT  
		Size: 22.7 MB (22709509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8740734e875c6119761eaa450ddf86492e161c3ba189bb7a553228675739490a`  
		Last Modified: Sat, 27 Mar 2021 05:36:37 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41322223cb0db7b2f85b4ce782bded120e746ec956a59b711c3a94efefb21201`  
		Last Modified: Sat, 27 Mar 2021 05:36:38 GMT  
		Size: 1.8 MB (1759472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4fc89e05f2e726a42d86b61ece624ed80a3325daa509925e7af84d886284ab`  
		Last Modified: Sat, 27 Mar 2021 05:36:40 GMT  
		Size: 5.3 MB (5285595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3fb1951ae5521b62f63897078966f06bbd4b671a84e23feb40b9ed8ed2a51`  
		Last Modified: Sat, 27 Mar 2021 05:36:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca730b0805353a00e92749eb1dcf1b63bf134359024f20d27a2d5ec0e5a574e`  
		Last Modified: Sat, 27 Mar 2021 05:36:38 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0e3bf42a5f79b5c00bf96b4263f861de2095043a5af73c8973a8d9a12edd7401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117933bd3e53f5572f06d07dc3be9201199feebe0e59f35880fb08d848df320f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:05:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 09:05:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:05:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 09:06:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 09:06:18 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 09:06:19 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 09:06:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 09:06:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 09:06:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73432000cbf913494b2dd2895431780fb24c5de87b4116dc4120208afeb895d4`  
		Last Modified: Sat, 27 Mar 2021 09:06:48 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca8b7a8ebcb36d0f266af5caa12326b78384982ff7b407c5bbb184588ea191`  
		Last Modified: Sat, 27 Mar 2021 09:06:49 GMT  
		Size: 2.0 MB (2007872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7978c28ef3edd4ebe57f3893e93deb88a5383143db5999487fb12384ce0996a7`  
		Last Modified: Sat, 27 Mar 2021 09:06:50 GMT  
		Size: 5.9 MB (5905343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd38d1ecd49b461de15549f7b257a299e4c9f1a13dbb15adcdf758c44dafd7e`  
		Last Modified: Sat, 27 Mar 2021 09:06:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2530fb66cc23163412987920279774b1da7169ab73501a343e24c3b797fa4c`  
		Last Modified: Sat, 27 Mar 2021 09:06:48 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:c7b62ea34691dc2c5a699b708d4a0582923a757ad9b41a6b5c9ed012455e6aba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bd5250a469ba27b4d7a5c6f483a6dec8e967d14cad2362ce98bfbd924ae446`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 00:27:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:27:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 00:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:28:18 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 00:28:18 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 00:28:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:28:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 00:28:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db59fb742889351c8257d71d9af7f8ab754780dfdb80e60bb34a5488afc26249`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2479ba868a69059ce8416072149d301726c919056b2d354373c241954b855dab`  
		Last Modified: Wed, 31 Mar 2021 00:29:13 GMT  
		Size: 2.1 MB (2132647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7d122183831a8ed76e681eeb8ead7cf5f075914d4386bf5fb20dcf081064fa`  
		Last Modified: Wed, 31 Mar 2021 00:29:20 GMT  
		Size: 11.6 MB (11633214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdfcb59f4fbfed086e7dc5075c6db916e00188a042b7612c5f03252f5eda4f6`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645a8c57aa0c862e9773fc2240ce6dcc565e9100a5223a0f67eb77140507ccf`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:7c7c058360198a6cdf1c0c5de4c7536b662d0aadb492a39eb71da1745ec6ead9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2e30091907d1d9785d74152c96711b6ea697670f5b2e51c2fef7e50032815e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:56 GMT
ADD file:74d504a9a34f47729165ef4ceedc9f0eaa2e91bfb6a24ebfc3ceed0248267a27 in / 
# Fri, 26 Mar 2021 08:09:57 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:56:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:56:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:57:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:57:54 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:57:54 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:57:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:57:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f863e006c40853ec8c23aa5b7a0e95918001f96878fb45770410ac4df51cf88`  
		Last Modified: Fri, 26 Mar 2021 08:16:29 GMT  
		Size: 25.8 MB (25772487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920815f459af869c2bafde850a4833f2c0af39a10540924371f7c810a2740698`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecefc467b0208174c90913c171e0635fc983fe0271e56d94814d9365402d9a`  
		Last Modified: Fri, 26 Mar 2021 18:58:21 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946d42bf9e7b59ba6752c87e806b5dfbcaab31bb0b4c62ad64e1106e2806bb5`  
		Last Modified: Fri, 26 Mar 2021 18:58:26 GMT  
		Size: 6.4 MB (6416271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bca10ef1481bbdde6f3709e04eb5245089e289de05b36095d3c0b7cd7d5a32`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbf9a1588f37aee944ed6e518b80a6c1c787fe4b75da67bfd3b3f191544931e`  
		Last Modified: Fri, 26 Mar 2021 18:58:23 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:9f6d20d1daa6cd853c2829541ecbd642ac3de0a47b6ba6d09aec3b064a882007
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccb828b29ef1c5d8e88d454ac3307b2607e7d07a516b3a6028fe00e30aea8116`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:14:22 GMT
ADD file:feb26657639018f8f43408e43e8ecec7e84632f33b42d5521241b842b58747d5 in / 
# Fri, 26 Mar 2021 15:14:28 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 16:36:00 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 16:36:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 16:36:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 16:40:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 16:40:38 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 16:40:41 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 16:40:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 16:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 16:40:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:035681ea37d9aab4545aa2211af3bf79addea316f71afde84412406734ef8a85`  
		Last Modified: Fri, 26 Mar 2021 15:22:05 GMT  
		Size: 30.5 MB (30525677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3001f02c630196b6d34866a51640bb423722404e58e6ec0dd89623c69ddc5f`  
		Last Modified: Sat, 27 Mar 2021 16:41:14 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2204248b5fcb9625e734191b9113a495608d92eca33cf00bd9b4d1d7a5ca8e5`  
		Last Modified: Sat, 27 Mar 2021 16:41:15 GMT  
		Size: 2.2 MB (2225167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08edb758e4fd44b9b6c53de4bc3867a35c3611d94678664bb443687ffdc898f3`  
		Last Modified: Sat, 27 Mar 2021 16:41:17 GMT  
		Size: 6.7 MB (6743526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc132087dda4152235c0aac9f32757e35db7c6e3958fee5627a67a81d573e214`  
		Last Modified: Sat, 27 Mar 2021 16:41:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676f92e18e0d0b6e112f621b4f69817f837335a26a2852bc7fddafeed10f56`  
		Last Modified: Sat, 27 Mar 2021 16:41:14 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:97d3bd125ab186461612f5227612b8bed1b7cdf339597a848150b8abb1df9748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11acca930a3acc9f10aec0e92255da2f3d7782c440d9ebe986775b5d784b5f7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 02:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 02:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 02:25:46 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 02:25:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 02:25:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 02:25:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 02:25:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c742a04892cc406ec636d3b61ae8b30ea2be9d8094b04a3e6fa844006600bb`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee293ba212f1e0d102b980847b925882c507858cf70dd83eca37c45fb14d8fb6`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 1.8 MB (1821969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048c0826dbbe30eb38c444743a578a8400ca9bb488e6dd498c2ae0c74a524ba`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 5.9 MB (5943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8fc932e810d22ad352fd6f592c4c76a7e0fc36211bb96549e2044049a0ae6c`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd24c1b830fe7b47376748fdbcf9a99c29e655cc7047927ab24e2aad8d1cf83`  
		Last Modified: Wed, 31 Mar 2021 02:26:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:19684fbf0023be921667a91a92d2cf6e979393817c9e69f7062aa2bb5bd5d5e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:da8bf89069f02c44e64a52cd3c311da57833ba52c0dfd401bf5b400bcba42fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6928a48d8b494975b09a73ff31d4ec85bbf1a70eb5240a267316a1495d85c91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:26:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 10:26:10 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 10:26:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 10:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 10:26:43 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 10:26:44 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 10:26:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:26:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05731027fa533b4ddfd5253b33af7f2e6329040d608478a1cf595d3594e504fd`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c330cdff7f6294e87be781c7a86aac39a7e7d2431c24def9e8af9476e2c7da`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7422b39d0efd63a811763e22eb91fcaa0ea348b8a13c6a2afd70562f5cb9bb89`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641ca636eaa042a42ed82a4494fe4030af9725300ffdc103faa9e12ce1a3816a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f1740d604bc2886348af7061a47d9a4343057827419e05f23191d5b911a3a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6d4e4fe6948e5a7992c124e61fa437b6e0413a5bb3401654fb248eb3cb12d114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c19db803961bd8dcd8229779fef2771123c1e74079d8339d813fcec140a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:35:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 11:35:31 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 11:35:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 11:35:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 11:35:53 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 11:35:53 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 11:35:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:35:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:35:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e02a3b4bec768000b32f6cd554e24e6c8494cbd013299b945dfba9976453`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be889af3bc0980bb5b61ae0b456dbd90907f154b74b796a26046e96f70c4f6`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a408cdd7892cb9e528cde840b9bf4c2457e6b9540f7b3eeba4b75bb22d5729`  
		Last Modified: Fri, 26 Mar 2021 11:36:26 GMT  
		Size: 223.3 KB (223278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb962d5a258d79b6a952f2eb3e3c6f8e4497529c9b722d855f051a120a68c0`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c91539d601c2ba091818f38b8b0b17362626aca4e30ca053825d5b4920cbe`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:90360f53f918820e5f6a844dee0754fa75b275607dbe5c71293fd0e7af7797c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f4df11bdbbf450f4e6fbf2b9bd4b57d9432205d415896d1ec7179a79658764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:46:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 05:47:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 05:47:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 05:47:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 05:47:57 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 05:48:02 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 05:48:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 05:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:48:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ade0bad869d6db8a4e76203a6dfe3818480c33c407956be758da40b7da8e87`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6878fc6b1c7c9ff2cb9cd6603daa1608abf9847d920dbc2a975313b81d54d09`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e8e86fc5762fedfcc865b9618a77f7c27214bf2068e2bdb0f7151d8964030`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 221.0 KB (220985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956adc5bd10550d52ee7f60d1d249008d2ca8b414e697b229923777c89fffae`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dac4482b42db1364dec4448343ae95036dd4f7b02440507ae3e40da8dc0d43`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c1f0c63244642a743f32f026370285292f3dae250a308e6364fc3de8ab05effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d526ff26ded3a191cd728d6ee4458ac19061aadfef60a349e786aab31ba72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:56:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 25 Mar 2021 23:56:54 GMT
RUN apk add --no-cache libssl1.1
# Thu, 25 Mar 2021 23:56:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 25 Mar 2021 23:57:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 25 Mar 2021 23:57:06 GMT
VOLUME [/spiped]
# Thu, 25 Mar 2021 23:57:06 GMT
WORKDIR /spiped
# Thu, 25 Mar 2021 23:57:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:57:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d211148772ab04d0ac7d6a254412fe1f42c1e2e7015b60b873a95da6f14a452`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9963e2f655c56703f1a6c0ddfe5ddd34f7f2725e4b4dadfe50a44dccb3fabbef`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd16cb6da0cae4c5ecfe500cf635456f5c13193987be355c858e78a57bf1150`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463e1d0912abda7c19a7c110819c8a1b49e67d57f21ab80715f4a0ee1664927a`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48866150c20dea94d44784f072b65bdf6f2292cc61d11de364bbe2d47f21ecce`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:19684fbf0023be921667a91a92d2cf6e979393817c9e69f7062aa2bb5bd5d5e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:da8bf89069f02c44e64a52cd3c311da57833ba52c0dfd401bf5b400bcba42fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6928a48d8b494975b09a73ff31d4ec85bbf1a70eb5240a267316a1495d85c91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:26:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 10:26:10 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 10:26:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 10:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 10:26:43 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 10:26:44 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 10:26:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:26:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05731027fa533b4ddfd5253b33af7f2e6329040d608478a1cf595d3594e504fd`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c330cdff7f6294e87be781c7a86aac39a7e7d2431c24def9e8af9476e2c7da`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7422b39d0efd63a811763e22eb91fcaa0ea348b8a13c6a2afd70562f5cb9bb89`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641ca636eaa042a42ed82a4494fe4030af9725300ffdc103faa9e12ce1a3816a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f1740d604bc2886348af7061a47d9a4343057827419e05f23191d5b911a3a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:6d4e4fe6948e5a7992c124e61fa437b6e0413a5bb3401654fb248eb3cb12d114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c19db803961bd8dcd8229779fef2771123c1e74079d8339d813fcec140a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:35:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 11:35:31 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 11:35:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 11:35:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 11:35:53 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 11:35:53 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 11:35:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:35:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:35:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e02a3b4bec768000b32f6cd554e24e6c8494cbd013299b945dfba9976453`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be889af3bc0980bb5b61ae0b456dbd90907f154b74b796a26046e96f70c4f6`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a408cdd7892cb9e528cde840b9bf4c2457e6b9540f7b3eeba4b75bb22d5729`  
		Last Modified: Fri, 26 Mar 2021 11:36:26 GMT  
		Size: 223.3 KB (223278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb962d5a258d79b6a952f2eb3e3c6f8e4497529c9b722d855f051a120a68c0`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c91539d601c2ba091818f38b8b0b17362626aca4e30ca053825d5b4920cbe`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:90360f53f918820e5f6a844dee0754fa75b275607dbe5c71293fd0e7af7797c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f4df11bdbbf450f4e6fbf2b9bd4b57d9432205d415896d1ec7179a79658764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:46:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 05:47:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 05:47:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 05:47:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 05:47:57 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 05:48:02 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 05:48:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 05:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:48:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ade0bad869d6db8a4e76203a6dfe3818480c33c407956be758da40b7da8e87`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6878fc6b1c7c9ff2cb9cd6603daa1608abf9847d920dbc2a975313b81d54d09`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e8e86fc5762fedfcc865b9618a77f7c27214bf2068e2bdb0f7151d8964030`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 221.0 KB (220985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956adc5bd10550d52ee7f60d1d249008d2ca8b414e697b229923777c89fffae`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dac4482b42db1364dec4448343ae95036dd4f7b02440507ae3e40da8dc0d43`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c1f0c63244642a743f32f026370285292f3dae250a308e6364fc3de8ab05effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d526ff26ded3a191cd728d6ee4458ac19061aadfef60a349e786aab31ba72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:56:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 25 Mar 2021 23:56:54 GMT
RUN apk add --no-cache libssl1.1
# Thu, 25 Mar 2021 23:56:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 25 Mar 2021 23:57:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 25 Mar 2021 23:57:06 GMT
VOLUME [/spiped]
# Thu, 25 Mar 2021 23:57:06 GMT
WORKDIR /spiped
# Thu, 25 Mar 2021 23:57:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:57:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d211148772ab04d0ac7d6a254412fe1f42c1e2e7015b60b873a95da6f14a452`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9963e2f655c56703f1a6c0ddfe5ddd34f7f2725e4b4dadfe50a44dccb3fabbef`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd16cb6da0cae4c5ecfe500cf635456f5c13193987be355c858e78a57bf1150`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463e1d0912abda7c19a7c110819c8a1b49e67d57f21ab80715f4a0ee1664927a`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48866150c20dea94d44784f072b65bdf6f2292cc61d11de364bbe2d47f21ecce`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:dc5f5f896cc7441fb4676b3aa5a911dac58aca8762ebbfb936e79ede5e376367
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:280bdf816a8f0ce321d66c5a765695190a9c3edbbd8af313d70b5fd047cf0cce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36268964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:177e254b3165eba26156c945f4dd0bcb1294728c43424187b5216211524d404e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:33:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 09:33:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:33:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 09:33:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 09:33:35 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 09:33:35 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 09:33:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 09:33:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 09:33:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372a623e820848080246423f9522d76632fd56ebd9e7cbcc3e2667c4b0379a88`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791b1741aa3b0fd443ebcc5a2f2a6b735a3ea18414dec574b0c61762a240137`  
		Last Modified: Sat, 27 Mar 2021 09:33:54 GMT  
		Size: 2.1 MB (2128524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44955b5b9fc6dbfc59ba93dc9add40129c020cf760eb35202c7bc09a7975985`  
		Last Modified: Sat, 27 Mar 2021 09:33:57 GMT  
		Size: 7.0 MB (7037245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed155aee7ced703085049efda143c0b629962d415f08d6e885d66fd6b4c4eb61`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8de1bcbffcf9f5c4958ddb3025efacc91c14296edb9b078aa73fcc2f011de14`  
		Last Modified: Sat, 27 Mar 2021 09:33:53 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2e00324da21253f7f0beedc1d2a123fa5efbc0e732f32044159d733abe700a17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1314e5a5cb457b2a8772a9ab8d7b1c83e9190f6c1b920601a114714ef5b080e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:36:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 01:37:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:37:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 01:37:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 01:38:00 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 01:38:02 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 01:38:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 01:38:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28182091d78cadb3063bdd9ce75c263b768f3a24453ab10eeef8d29081a26b52`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa81838cd994f801fc7d925cf1700aa43b15f134a749eac7d4a4da60a15a175e`  
		Last Modified: Wed, 31 Mar 2021 01:38:24 GMT  
		Size: 1.8 MB (1839326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b00960d8e0c9e05dc7343b699974e653177c263af4f99f3f849b4062226ddf`  
		Last Modified: Wed, 31 Mar 2021 01:38:23 GMT  
		Size: 5.5 MB (5479910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0df0d7972be414ec17fc2d27808177f0e968261e2abc699a4ddea72869042`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed60abb976ac8333612b838e368cffd3ccb982d68fed535f5b555d86cb0e6ed`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b32775847daf03e28d6505b2efe6e3f13e6c861418c1d19cb03953193dfd095
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29756781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c71a26ce499550c85d6ff57d5bc1454d0cd7582bf67d215918c27ef2b87fcf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 11:17:38 GMT
ADD file:911acc83e6d3d4b00ecc59effce9e5ab69d62aa3e77a24db76e270db8cedce5f in / 
# Fri, 26 Mar 2021 11:17:39 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:35:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 05:35:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:35:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 05:36:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 05:36:09 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 05:36:10 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 05:36:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 05:36:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:36:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05a8be0db5eb6dbb349e49a01211d3a11adc23881f696760a058c0c8ae8e39b7`  
		Last Modified: Fri, 26 Mar 2021 11:27:34 GMT  
		Size: 22.7 MB (22709509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8740734e875c6119761eaa450ddf86492e161c3ba189bb7a553228675739490a`  
		Last Modified: Sat, 27 Mar 2021 05:36:37 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41322223cb0db7b2f85b4ce782bded120e746ec956a59b711c3a94efefb21201`  
		Last Modified: Sat, 27 Mar 2021 05:36:38 GMT  
		Size: 1.8 MB (1759472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4fc89e05f2e726a42d86b61ece624ed80a3325daa509925e7af84d886284ab`  
		Last Modified: Sat, 27 Mar 2021 05:36:40 GMT  
		Size: 5.3 MB (5285595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3fb1951ae5521b62f63897078966f06bbd4b671a84e23feb40b9ed8ed2a51`  
		Last Modified: Sat, 27 Mar 2021 05:36:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca730b0805353a00e92749eb1dcf1b63bf134359024f20d27a2d5ec0e5a574e`  
		Last Modified: Sat, 27 Mar 2021 05:36:38 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0e3bf42a5f79b5c00bf96b4263f861de2095043a5af73c8973a8d9a12edd7401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117933bd3e53f5572f06d07dc3be9201199feebe0e59f35880fb08d848df320f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 09:05:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 09:05:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 09:05:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 09:06:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 09:06:18 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 09:06:19 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 09:06:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 09:06:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 09:06:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73432000cbf913494b2dd2895431780fb24c5de87b4116dc4120208afeb895d4`  
		Last Modified: Sat, 27 Mar 2021 09:06:48 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca8b7a8ebcb36d0f266af5caa12326b78384982ff7b407c5bbb184588ea191`  
		Last Modified: Sat, 27 Mar 2021 09:06:49 GMT  
		Size: 2.0 MB (2007872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7978c28ef3edd4ebe57f3893e93deb88a5383143db5999487fb12384ce0996a7`  
		Last Modified: Sat, 27 Mar 2021 09:06:50 GMT  
		Size: 5.9 MB (5905343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd38d1ecd49b461de15549f7b257a299e4c9f1a13dbb15adcdf758c44dafd7e`  
		Last Modified: Sat, 27 Mar 2021 09:06:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2530fb66cc23163412987920279774b1da7169ab73501a343e24c3b797fa4c`  
		Last Modified: Sat, 27 Mar 2021 09:06:48 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c7b62ea34691dc2c5a699b708d4a0582923a757ad9b41a6b5c9ed012455e6aba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bd5250a469ba27b4d7a5c6f483a6dec8e967d14cad2362ce98bfbd924ae446`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 00:27:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:27:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 00:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:28:18 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 00:28:18 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 00:28:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:28:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 00:28:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db59fb742889351c8257d71d9af7f8ab754780dfdb80e60bb34a5488afc26249`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2479ba868a69059ce8416072149d301726c919056b2d354373c241954b855dab`  
		Last Modified: Wed, 31 Mar 2021 00:29:13 GMT  
		Size: 2.1 MB (2132647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7d122183831a8ed76e681eeb8ead7cf5f075914d4386bf5fb20dcf081064fa`  
		Last Modified: Wed, 31 Mar 2021 00:29:20 GMT  
		Size: 11.6 MB (11633214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdfcb59f4fbfed086e7dc5075c6db916e00188a042b7612c5f03252f5eda4f6`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645a8c57aa0c862e9773fc2240ce6dcc565e9100a5223a0f67eb77140507ccf`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:7c7c058360198a6cdf1c0c5de4c7536b662d0aadb492a39eb71da1745ec6ead9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2e30091907d1d9785d74152c96711b6ea697670f5b2e51c2fef7e50032815e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:56 GMT
ADD file:74d504a9a34f47729165ef4ceedc9f0eaa2e91bfb6a24ebfc3ceed0248267a27 in / 
# Fri, 26 Mar 2021 08:09:57 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:56:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:56:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:57:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:57:54 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:57:54 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:57:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:57:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f863e006c40853ec8c23aa5b7a0e95918001f96878fb45770410ac4df51cf88`  
		Last Modified: Fri, 26 Mar 2021 08:16:29 GMT  
		Size: 25.8 MB (25772487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920815f459af869c2bafde850a4833f2c0af39a10540924371f7c810a2740698`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecefc467b0208174c90913c171e0635fc983fe0271e56d94814d9365402d9a`  
		Last Modified: Fri, 26 Mar 2021 18:58:21 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946d42bf9e7b59ba6752c87e806b5dfbcaab31bb0b4c62ad64e1106e2806bb5`  
		Last Modified: Fri, 26 Mar 2021 18:58:26 GMT  
		Size: 6.4 MB (6416271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bca10ef1481bbdde6f3709e04eb5245089e289de05b36095d3c0b7cd7d5a32`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbf9a1588f37aee944ed6e518b80a6c1c787fe4b75da67bfd3b3f191544931e`  
		Last Modified: Fri, 26 Mar 2021 18:58:23 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:9f6d20d1daa6cd853c2829541ecbd642ac3de0a47b6ba6d09aec3b064a882007
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccb828b29ef1c5d8e88d454ac3307b2607e7d07a516b3a6028fe00e30aea8116`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 15:14:22 GMT
ADD file:feb26657639018f8f43408e43e8ecec7e84632f33b42d5521241b842b58747d5 in / 
# Fri, 26 Mar 2021 15:14:28 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 16:36:00 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 16:36:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 16:36:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 16:40:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 16:40:38 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 16:40:41 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 16:40:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 16:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 16:40:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:035681ea37d9aab4545aa2211af3bf79addea316f71afde84412406734ef8a85`  
		Last Modified: Fri, 26 Mar 2021 15:22:05 GMT  
		Size: 30.5 MB (30525677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3001f02c630196b6d34866a51640bb423722404e58e6ec0dd89623c69ddc5f`  
		Last Modified: Sat, 27 Mar 2021 16:41:14 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2204248b5fcb9625e734191b9113a495608d92eca33cf00bd9b4d1d7a5ca8e5`  
		Last Modified: Sat, 27 Mar 2021 16:41:15 GMT  
		Size: 2.2 MB (2225167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08edb758e4fd44b9b6c53de4bc3867a35c3611d94678664bb443687ffdc898f3`  
		Last Modified: Sat, 27 Mar 2021 16:41:17 GMT  
		Size: 6.7 MB (6743526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc132087dda4152235c0aac9f32757e35db7c6e3958fee5627a67a81d573e214`  
		Last Modified: Sat, 27 Mar 2021 16:41:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676f92e18e0d0b6e112f621b4f69817f837335a26a2852bc7fddafeed10f56`  
		Last Modified: Sat, 27 Mar 2021 16:41:14 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:97d3bd125ab186461612f5227612b8bed1b7cdf339597a848150b8abb1df9748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11acca930a3acc9f10aec0e92255da2f3d7782c440d9ebe986775b5d784b5f7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 02:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 02:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 02:25:46 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 02:25:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 02:25:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 02:25:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 02:25:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c742a04892cc406ec636d3b61ae8b30ea2be9d8094b04a3e6fa844006600bb`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee293ba212f1e0d102b980847b925882c507858cf70dd83eca37c45fb14d8fb6`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 1.8 MB (1821969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048c0826dbbe30eb38c444743a578a8400ca9bb488e6dd498c2ae0c74a524ba`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 5.9 MB (5943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8fc932e810d22ad352fd6f592c4c76a7e0fc36211bb96549e2044049a0ae6c`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd24c1b830fe7b47376748fdbcf9a99c29e655cc7047927ab24e2aad8d1cf83`  
		Last Modified: Wed, 31 Mar 2021 02:26:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
