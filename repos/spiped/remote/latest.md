## `spiped:latest`

```console
$ docker pull spiped@sha256:de60f1e86120845dfc5fc566e992ac2528bab5092551860ff597aaa498ba6d12
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
$ docker pull spiped@sha256:cf4b9920b3942ecc606b6251cd4eb1bd48f98354d8e022b3f6307e507a32a3eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36268832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57285b121dc86ae46a0c0ce8c6f60015ae52e9e52103a25f3f7e0bee876c9013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:34:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 13:34:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:34:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 13:35:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 13:35:13 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 13:35:14 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 13:35:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f47a7b37f3c4e528ff97e5decf3ec7f0f82137d90195c99d3fe65b624ca58fd`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4ec8344be05d9a5973c107aaf4e4cf134ba0065ba7d21299b2a6e1bb25c514`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 2.1 MB (2128360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b9fc3b146c01478f36950913fdf41df19eea49b156804c28887e9f174b295c`  
		Last Modified: Fri, 12 Mar 2021 13:35:56 GMT  
		Size: 7.0 MB (7037267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb08069f68a0c759772577589709386d06dea228eaec0950fe149dd7650cc0d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172a7d7369794ee94aa0835f18b712095f912fa4d72e79d8194dbc44ec7eb9d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a1859deb50255891bcc3c7a0d51355f4f70c6edfe53681e7ef9b5f7c5176e954
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32167605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0a64bf564abffe8a63869d6aa971922106895f4b214fc7169fa59e36c3ee08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:25:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:25:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:26:35 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:26:36 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:26:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:26:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d845bf35fa4e16c567b254de98a71d1e4e1f5abfecc37f18041fc0ad9ac367d0`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99392226a8fd34bae433f750e9ddade149245f97aed7ab145c5a2d5027ca7b04`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.8 MB (1839291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1365ecba2ae17a6ae4b2804ea9b0487564b2a3ca585c2dc067d772334005706c`  
		Last Modified: Fri, 26 Mar 2021 18:26:59 GMT  
		Size: 5.5 MB (5479955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e98946787ec7084b445443fa69efa539d294f50a40e4451f6f309e8654b6de`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323331d38da7c134c92cc01ac4d70bd80866d063ce6c830123cd5642c48a5c1`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:44b3d70bc67d9e79a0419fc5a58d5f75c2346b6b91c850eb8022d695c86d6dc0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29756566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c089b8e65d7c3f6294c9228488e4f6a557c3953b0c0bf77c853af5a8bbe4c8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 18:06:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 18:07:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 18:07:08 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 18:07:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 18:07:56 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 18:07:57 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 18:07:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 18:08:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 18:08:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a72435c8477703e20922f5027fd6568243135941b80e77d47c7dbd306deb7db`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a18dda64e40f4f3e5a9f9ca31fb7c16865b51ae45cfe5ac2e617eae69cc491`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.8 MB (1759316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4ee5438547836415ee455059b8e85b95417a1756c8b483e918d759f168738`  
		Last Modified: Fri, 12 Mar 2021 18:08:32 GMT  
		Size: 5.3 MB (5285580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3c8111fcdf41439b1a236c436224ce598dded7c6865d854ec18b4f9a55066a`  
		Last Modified: Fri, 12 Mar 2021 18:08:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42912a86aee0cc95765faede7cbe55af4057798a132a2122904ff3032149f477`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:996a11488350dceb8604e33f1f98f228dfcb4695ca0d70bf95143b1f96dca774
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877033d2e28e782f80c0ce3818b074e662a0b919a33677f21291883e5623c318`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:40:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:40:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:41:00 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:41:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:41:51 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:41:52 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:41:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca354c521ef166c95eb0651133c5463b60c4eac376b689c5bcb60986e9646614`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae9f3f5cb127a6f21b277922c584457d48075bfab82aa39f465f1eab493e83`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 2.0 MB (2007619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e463abc2137a48bc46b91b4d802e93372aac904b001fb2afc6f8499bde098`  
		Last Modified: Fri, 12 Mar 2021 17:42:25 GMT  
		Size: 5.9 MB (5905317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911bcabad5c4b743e2880b1bef893d4af3f85656bd20931a8067b35b3f7242ec`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2994d1820f2d23b01afa44ab9c272d84d2c302cf2b48a6486c4123af5b63403`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:4dc923ad898759bc3d6fab0372921a04485aeaabdc63decde7af4063d743e298
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41529023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c50ce465ce8c1a90ec0ce4d52c4e9da147bfaa6b030d3b167bfd7978a376bdf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 13:53:11 GMT
ADD file:6c7524352aadfb597840d7c62001b10cf663f17dc2752a1bc5ad40b538138432 in / 
# Fri, 26 Mar 2021 13:53:12 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 02:37:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 02:37:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 02:37:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 02:37:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 02:37:39 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 02:37:39 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 02:37:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 02:37:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 02:37:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cd20c3ac698e839ccd9bbdb86bc90efa00779d975e4064809852f86f56d8f3e`  
		Last Modified: Fri, 26 Mar 2021 14:01:40 GMT  
		Size: 27.8 MB (27760999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a64bde3f02634d1619c75e254b9961b99e6a7efc85fc274622e191406d2fc9`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b2ee4d4d2d7adcf310cc6e555b8e238213756205c7063ff7edaae68dcf3aa`  
		Last Modified: Sat, 27 Mar 2021 02:38:15 GMT  
		Size: 2.1 MB (2132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8871f8a1e0b60f5223ffb9eed20ea1b49d52cd3c8e946accfb3c40ddf83dbbc`  
		Last Modified: Sat, 27 Mar 2021 02:38:17 GMT  
		Size: 11.6 MB (11633213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe7c2c6f83bc692c92f33ea153c717a6b73fb3b20e06a52a92c94008f72572a`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bf3b4efa0c3e5627678a36308847efdaec6f832d4d3b410e85288f491da1a2`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:e122036d98543d87b9208165ec52dbb80182b3995a8fe6f959e114bfceedab05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d2afbae5f13389e96b5a75c34b3f3d8779d7bdfdb5b632016a0a7dc8a6bba4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:29:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:29:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:29:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:33:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:33:05 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:33:15 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:33:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:33:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82731719cf164c1334090880e51dcdc657bcf76a28356d37ab5d3b29dddb03c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078b30e1777b326949f45e26c2edccb9206038fc736257bd267b5de2b0bd2e4c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 2.2 MB (2224920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b723c17a647249606d310a15aed3e35bf407aa07bc6a804c155f9ccb16dd32a`  
		Last Modified: Fri, 12 Mar 2021 17:33:49 GMT  
		Size: 6.7 MB (6743532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d16a0a03be990173113dcd300a3a1d3a78851790b9ad337a52548d0b831471`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13c1f1fd23a837927b6a7954e91788f660a1abbbcfad8c58a0ad6829a0efcc7`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:12f759b16118c1f0d7e9e94a6b9fb43b6f2eef818e37aa4a77f30b5f3d42d1e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33483871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9093d4f6f1989a735c83e462a300ec7787a5fc1bfd5733a853b8e7a6c6178f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 10:53:48 GMT
ADD file:3a3cf2e796c665cae881fb0b8a23a071206531af98c03548ab5a8721b3c67353 in / 
# Fri, 26 Mar 2021 10:53:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 16:47:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 16:47:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:47:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 16:48:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 16:48:22 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 16:48:23 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 16:48:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:48:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:48:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a37ca8d63090f0f22441ceecc0af7881a2668336202cf586e841e3d9e06f2f4b`  
		Last Modified: Fri, 26 Mar 2021 10:57:46 GMT  
		Size: 25.7 MB (25716264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9218249b019c346421bbd61020211795c99650c27d1d482109567f5c54d83852`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960815f9e510f19f5c7d87ed71ad7ee4a2a617b01fa3126deaf13d93c68e6abc`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.8 MB (1821963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38910ce19f0387b2df268b10b4691bdc33d47d3b4148957276b91ed47e9c6143`  
		Last Modified: Fri, 26 Mar 2021 16:48:44 GMT  
		Size: 5.9 MB (5943433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc6af6e6cc8e3705de996630edc8234b408062e105fc7913be86eccec68e28e`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279df31dc6bb719879202509a10292d1046cf406b6032ec3bcd331c1782ec52`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
