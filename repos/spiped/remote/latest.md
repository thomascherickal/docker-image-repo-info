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
