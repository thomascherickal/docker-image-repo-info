## `spiped:latest`

```console
$ docker pull spiped@sha256:7f9959fb832c006c9b7a3f8254ca480038ecaadda485391e1a502bfd640dd83b
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
$ docker pull spiped@sha256:cbcdcae2145e7f1c5b4c4e2ec9926e8f7cf2741c2edd41e74eb1a5ca85431c6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a3a8321db5126e2cfa970d9cabeafcbc493ae611c56ac1b7f3bc9c1877287`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:36:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:36:35 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:37:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:37:06 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:37:06 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7e552308a9a7e56787eb8f2ee2cd0e5ae1bcd3e6e70767a3f1f63d04df1043`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3cfef5f840d90ca6a31c452db1ff437bc80f30c34bfe95e60a73d26faa39a`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 2.1 MB (2128094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b92b058cf5a162f3e9e9c1b57e6ea521b98cfbdfe95c64e96543614c0aa889`  
		Last Modified: Tue, 13 Oct 2020 02:37:26 GMT  
		Size: 7.0 MB (7037515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e07e79b0faf86dec01bde507101fa39b284b027b0a16dcc2e0385b2711b7d7`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774b42f92e50846c6909f7c57a4559f4e39365596961f3cc60c181fd5ff02f7`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:758eeca094a599eb3c40488fdc3660e244d92eb1cc051222499690c2800be3c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32171540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:301a1400dd597f63f9f970d233a48c6368dd4f5daeae24b57ea1e176ab3f2f80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:37 GMT
ADD file:d75cebdc79385debd2d6d1c8c34855d2bd4779b13ee47f76e34c6d8fca037531 in / 
# Tue, 17 Nov 2020 20:20:45 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:42:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 06:42:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:42:44 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 06:42:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 06:42:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 06:43:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 06:43:39 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 06:43:41 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 06:43:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 06:43:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 06:43:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b8dd2ec17ab788b6ea03a9b6cf68afada9a8692681d29e9795db0abf6554404`  
		Last Modified: Tue, 17 Nov 2020 20:30:33 GMT  
		Size: 24.9 MB (24850311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2df983a334d6a2a60ff1f3d42b92a0cded5b175956f23fefeb1c6be1a67b72`  
		Last Modified: Wed, 18 Nov 2020 06:43:53 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018774055c0831c1463c402b1d74727152000afd63b85cc2701712391dca5a1b`  
		Last Modified: Wed, 18 Nov 2020 06:43:54 GMT  
		Size: 1.8 MB (1839116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fad6490cac039fbb603f19a4d225d45753cb19a05c79d98f61428f4e144386`  
		Last Modified: Wed, 18 Nov 2020 06:43:55 GMT  
		Size: 5.5 MB (5479912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89f5dc9c0aa507943aa3c77a5d229600a9498f45edf703e011410de95f859a1`  
		Last Modified: Wed, 18 Nov 2020 06:43:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bc0b5be5df57d6e22ade93d143e703b6a941977e35864a3122f355de0b538c`  
		Last Modified: Wed, 18 Nov 2020 06:43:53 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c92653d99274d40ed92e53b51cd458c1c727bd16db66392e4ece2f0b00be2bba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29761232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2661d3a07d889d24fd48344b6e5491127cb4f992b7c6792f931e16aed75e01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:11:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 07:12:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:12:02 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 07:12:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 07:12:49 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 07:12:50 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 07:12:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 07:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 07:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cf66057f794f2070347e36745e45359107e121bbf72ef76a056d4d4fc427c8`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d27f2deb7663af698a4e93d06d910420b62eff5f2514cf63280715267d5e70`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2c064480e805187730287fd350b20cc30e1d074b9bf0a28d1d2a9a99934bc`  
		Last Modified: Wed, 18 Nov 2020 07:13:11 GMT  
		Size: 5.3 MB (5285408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c3e496f6405bc525c1b47e008b53a0702b5b3bad600d201daaefffd563a900`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070369842a89c55f148641e29030bb3456430e5b407bca9462c0845656ffa901`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:bd8c013e18d70ea795869cd67cc4c91cd12a4a46c99e81a6265b730a8c714ed9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ef4e8f5b127720ba9505de9ed04ecd332a825b084c225f9cc7ff42b6149a2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 21:06:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 21:06:37 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:06:39 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 21:06:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 21:06:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 21:07:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 21:07:41 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 21:07:42 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 21:07:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 21:07:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 21:07:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a84f6f016cb9d510c26fe73828e975a9f6fc50997854f8118cb145c074d5ae`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b87b1c6722e9ec22dc49bb335ce8db2bd481ed351a6ddb5c82f6eb6efd0158`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 2.0 MB (2007865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2397a6f08399786b9b34edfa9dba1ef35efd220a5be1e3bf7f0c703afd2852`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 5.9 MB (5905487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454768d2d9825793660ef493926e3a9571a410a33bd15033af0ad860c1a7decd`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc56fbfab291b081b0371559eab32497a05458b34889aa47c4cbfcad16d058`  
		Last Modified: Tue, 13 Oct 2020 21:08:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:eddfe3c52b1f4b047ef49c6894ac40c53dae8caa677970de4764755a754e2d13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41533953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f2903e64f88c4e2273df5e291e5b21389aab4d0a9650d5208dc6b9554981a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:58:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 02:58:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:58:29 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 02:59:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 02:59:14 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 02:59:14 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 02:59:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 02:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 02:59:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264b3982a6da8264a3a2509542dd8f472e2d82b36d7390aae536e3610041397`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a88c082c81069b5976f79f328a9b78f7cb1c5f3401419d2f93e4bd215f38c6`  
		Last Modified: Wed, 18 Nov 2020 02:59:41 GMT  
		Size: 2.1 MB (2132327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574d0a70d657cc4f156f932200e3fb841eacd020f9786fda644f94670ea16967`  
		Last Modified: Wed, 18 Nov 2020 02:59:46 GMT  
		Size: 11.6 MB (11633270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08225d6c4b1f5a1e4901290593a71354dd7c6c676ad0319b46ca6f412e3b7ddc`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02262d310542335fc2631f9f33cc647034e6d1631581742ac01cc8aead9aac83`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:243dc5166fb19dded5aa7f688c64f8b13bf15e99a113733d155ab74f1f168a20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33907845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b92b94ba5487463c171553956b8c9a332f44c401cb8db357c44f7c19a570229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:59:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:59:27 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 23:00:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 23:00:36 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 23:00:36 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 23:00:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 23:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 23:00:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9c786dc23ade88d3972745848ed18089b024099778eb9bf9d5c735c7c4614`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2f2cc0e46aaf9c5d0d01e3ff5c89071efebe06cb0ea5051f316c674af976b`  
		Last Modified: Tue, 17 Nov 2020 23:01:03 GMT  
		Size: 1.7 MB (1712030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e296927f1a689719138bc125a62b2d185095d494c1a18e511c2892e5f7e6ebc`  
		Last Modified: Tue, 17 Nov 2020 23:01:09 GMT  
		Size: 6.4 MB (6416166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2df2217335c02b14a90f6c1795f3149d71d77ba2611651c6a679b4bcca6d78`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d899f01843caa25aba126202c9fb34048dffe56d82e9d6296c2ec3177157c39`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:11f9c1dbc68d2bcdd7a7f524027219a963ce523b201e71ae83c7052e635b27c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc337b8be5274e46ce4e2892582058be9fe426dc646660aa407e845573321c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:32:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 08:33:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:33:18 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 08:33:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 08:33:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 08:40:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 08:40:16 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 08:40:29 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 08:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1d07b98a86b2674f96635104e41916c1e547434cb7d561cd85492408607281`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c21d3c72f09a47ee5eaa7be57ecda6468c5095c72c0ae090abfab50a53f17`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 2.2 MB (2225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a219f1f2d5be3ad0b26293fc2b817c1bb804bb21197d100b7dd072101f007`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 6.7 MB (6743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cacc68fbff4f9b9f07d0bb78c5b34216d92ff73ee186cbac165f8ee0cc552`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6e602fa91081254fd3482a446e8d14916d389cda086023515709324d584b`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:db61217a4053f03c05b983f7d2722530fd82d6735e721311d7f90b17be40b713
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33488732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b062dbf1be23d35f8fb2e20a863861f260daee06fb4b84c4e4f7a669a6ecdbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:00:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:00:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:00:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 22:01:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:01:22 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 22:01:22 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 22:01:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 22:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 22:01:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43806a3fd3d362292aa4489b61228dc530d6820323d12f115ae0c4736e1b8ea`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80774235907721c9cd1bfff884ac7b597fe103ccb597a2563894bbc9a60bbb7`  
		Last Modified: Tue, 17 Nov 2020 22:02:11 GMT  
		Size: 1.8 MB (1821805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af91886a196e09e46584c37d8e2a8b40ab99d06f7096b4bed331ab4a63609ee`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 5.9 MB (5943582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d47aa91c0fe928301af1785740dd8890de723dff4c762a9c290e2b85178a1b`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a66f51280aa12fc65c7a03ae1bc737a260e3eb12d0c742a80d2757c48ba6cc`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
