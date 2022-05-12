## `spiped:latest`

```console
$ docker pull spiped@sha256:f4b43567408be8eb1659d8f62cd6cac70cec4980020e9dc46e64479044d9cda8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
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
$ docker pull spiped@sha256:a66911a787746637e44a865f64e731ea404d2266efa5d987ee58d6d535a3999b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b801341ea8d054b7b965f35306e02a25be57d78de5177ed30cfb7af2b0267b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:31:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 09:31:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:31:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 09:31:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 09:31:32 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 09:31:32 GMT
WORKDIR /spiped
# Wed, 11 May 2022 09:31:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 09:31:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 09:31:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080576f9a12bf8fca30a9653a7d9a0772acec767c26a2330bcdd92e5be0cfe95`  
		Last Modified: Wed, 11 May 2022 09:31:50 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bcb584eb7cb0f5bd593db63ab12b7b34bea2aa958fde7434a9b859ec903c08`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5664b9af48e8dd5dd00adb4691215c987017dbdb64998cdc9c30c22786d136d`  
		Last Modified: Wed, 11 May 2022 09:31:51 GMT  
		Size: 6.0 MB (5967174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6affb70c27746eb9c197393a54cd9b606353628e04424d0b4935ac195b6674a`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd4accaf294c916a8ef636747fa575dbaa0f547f8bd5c7001c0112a9507dc2`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6b56704713f5efb9e393f0c751fe4e3ecfc3762033496269972dbb442a70972d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33952053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b14d990d1127fdf382852ac149cf58dd872a968df8176e8a74a5778ea0738c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Thu, 12 May 2022 01:35:14 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 01:35:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 01:35:23 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 01:36:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 01:36:15 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 01:36:15 GMT
WORKDIR /spiped
# Thu, 12 May 2022 01:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 01:36:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 01:36:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5a9157aa645038e20cfd8d939540308935a2f448009504b4b50f55ebe7fcc8`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d8521d9bd468b1d6a357f9682b3e0efc683bb7ce8c61b98639d89a6e5a9d3`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94258b91da89ba5bcfb0b99e7a7224030f4fbc734a79e19488d7b2e198797278`  
		Last Modified: Thu, 12 May 2022 01:36:55 GMT  
		Size: 5.0 MB (5027685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ecd42d03f9650c45b9f15fb17188211b89f7ea6683a8aa6d8cf3ea08653577`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82055141d6a68a71687d6ce1c4aa739a9d6fa527bf54e1eb9120550413add7ea`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:869f873265d46c19a7ef8e99c75310e34199aaacaef33bdf15f86b96e3f3e031
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31326980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37ce8bbe3ed2ad9cdbe03dad14155e98db66700df5ccfc9f438ffc712f18629`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 20:14:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 21 Apr 2022 20:14:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 20:14:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 21 Apr 2022 20:15:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 21 Apr 2022 20:15:24 GMT
VOLUME [/spiped]
# Thu, 21 Apr 2022 20:15:25 GMT
WORKDIR /spiped
# Thu, 21 Apr 2022 20:15:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 20:15:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6735c69794075d50eaabf15a612f5327e0e06efcf5e9fb3506c0a15a2e44e`  
		Last Modified: Thu, 21 Apr 2022 20:16:26 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3954fbb32742ade4d09f7de5a24b799df2be24e900dcaa893cd8a96a56f9caa`  
		Last Modified: Thu, 21 Apr 2022 20:16:26 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0196e7d372a68d04f4a8db8ee17d963f5309f31bd3e2de3c87f1738a47c1fa19`  
		Last Modified: Thu, 21 Apr 2022 20:16:30 GMT  
		Size: 4.7 MB (4747972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ac7133605a50c53c0d2556551029995cc6cea3075e189e942cb665d6230a4b`  
		Last Modified: Thu, 21 Apr 2022 20:16:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cc36e09684bedc55194c1e3b51965ea507f35d45636e07846ef3a9daa38e7c`  
		Last Modified: Thu, 21 Apr 2022 20:16:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:572906adb8bf287a02331ed2dc6b70d40c1795ce56eb514a7b873ac8b0b07782
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8ebf44dc7acf424cbe762be8778cd542ccc7006e183a616763d3b92f5af2cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:24:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 12:24:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:24:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 12:24:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 12:24:56 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 12:24:57 GMT
WORKDIR /spiped
# Wed, 11 May 2022 12:24:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 12:24:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 12:25:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25366de1af948b0eef7cad0d0d1fbc56648a743854da03fc57dc121c2384213`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 1.6 KB (1621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef033e02dd13ee59e5336850b85b81cbd2ccd353a033415114d010d6a8254df`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac510a96382ea09a86f8f4cadc73653a8177516d4771a4a7e3bccbdeeb326de`  
		Last Modified: Wed, 11 May 2022 12:25:33 GMT  
		Size: 5.3 MB (5270881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1616a14c0096a1c7108f1fe3372296010619c2f7c502e1802e6d3855dfdf0ebd`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaa87e60ef72bc3e5eab8bd8a81a9cee650735736cd7c760f4366260b5461d2`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:d933a3ef2f835e9d32f01babb2f55693ab6f3b2150d76a4e72d6fdec66739208
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40284215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8994e3dd3df7e9fdbd0d51ca1e620fa69f6efd232ff5d5d2b381cd6b22fbc13c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:51:27 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 15:51:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:51:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 15:51:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 15:51:52 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 15:51:53 GMT
WORKDIR /spiped
# Wed, 11 May 2022 15:51:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 15:51:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 15:51:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9bc810ed14e83b2b6c2de848151a8aac3442608851df4e4ba4f35402048a54`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddd23897c0dc65364a8fda9129fe87c608a02ac54bdd3002e70407c7dff7b8a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a55bc0fd5c56c871a37888a72d560d40d0364889e86b54c791bea4bb7c85887`  
		Last Modified: Wed, 11 May 2022 15:52:28 GMT  
		Size: 7.9 MB (7891471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4fc1778cbfb42cc882687278e3d3bb64b10572a3b56cf12d7ba9b128537d21`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc951e82cef08be37b45eba1592c940f1a946d625884f3e80794061addeb20a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:fd460dccb2cca886ab01729919d23408b554000427b1c4e7880fcaeeb33978ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d68b6ce9beb17583f0d8186abb858ead76615104ff02e59558a46b6141c57ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 14:28:35 GMT
ADD file:11939fa9b6e0a3bde2ba32552130208df232ae0dd139b9244b80fa309690d57f in / 
# Wed, 20 Apr 2022 14:28:39 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 01:07:11 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 21 Apr 2022 01:07:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 01:07:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 21 Apr 2022 01:08:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 21 Apr 2022 01:08:58 GMT
VOLUME [/spiped]
# Thu, 21 Apr 2022 01:09:00 GMT
WORKDIR /spiped
# Thu, 21 Apr 2022 01:09:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 21 Apr 2022 01:09:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 01:09:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:211e565c951d5d12adf5ac13e34b5fdba747f88e6b462c2863538110b219144c`  
		Last Modified: Wed, 20 Apr 2022 14:39:17 GMT  
		Size: 29.6 MB (29641236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e19f3363f7cb07ea4b3a0ad412fca5c727d1813ac04bd4940ea1d607c657fec`  
		Last Modified: Thu, 21 Apr 2022 01:09:26 GMT  
		Size: 1.6 KB (1629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69bf594be84039807ebdc9b3c572db47f69e725e98328e8865230b5d0895dab`  
		Last Modified: Thu, 21 Apr 2022 01:09:26 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f3a21e1ee0f4f7c271e9ef40166c5a338c07b3662211a38fde4c6e7d33651d`  
		Last Modified: Thu, 21 Apr 2022 01:09:31 GMT  
		Size: 5.7 MB (5704960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b05c0e75dfebd3f55cc414ed1007be33b5a8eacc394f02c4c40afc3125401`  
		Last Modified: Thu, 21 Apr 2022 01:09:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50594bd507b5e96171fc501cc75333437f3d8028d1f39fab0824f4ab8eb38a50`  
		Last Modified: Thu, 21 Apr 2022 01:09:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:e338e5b4a068b2c06d20548b51e98cf9e6711b5ba3f91a55f33517103107db26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54eb4238d8977094c460b01a31bf18ab2865f97d34da09adaf33454df8e1a99f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:18:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 14:18:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:19:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 14:21:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 14:21:45 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 14:21:59 GMT
WORKDIR /spiped
# Wed, 11 May 2022 14:22:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 14:22:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 14:22:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e371d58c256a557b6f8f7b903d8a39345ccc364236516cb3ec208e9e40e92c5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4caf1ad053d6d5585c461ca9b8d4c6a14a963b94b0d13bb0594b2244f15a8b`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23602e10ec58354d8276b2a6d7549e7f11c523d76e28603f149ca4c0e1e951`  
		Last Modified: Wed, 11 May 2022 14:23:04 GMT  
		Size: 6.0 MB (5999080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa6bf1315149ea1738416c3df58107d0e9c60aae5cb546cfdcbb50aa6855062`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82539badabc1522bce1e3acd0e092aceb9818dd6904d2ab5fe8a10ab39a0f6b5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:a2261239d98aaef54af72737a4aa30c1a01f4089439604c977e606d06e5eb317
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d218c6ec1b1cc03c92a160497f19dc4deed41827aaf7bef061ddc8ca4c8f6fac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 06:26:51 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 06:26:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 06:26:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 06:27:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 06:27:07 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 06:27:07 GMT
WORKDIR /spiped
# Wed, 11 May 2022 06:27:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 06:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 06:27:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873c48057acd3a3e859a48bcca0c21842c182414ce09c34a3cc1c1886f7de52a`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c3eb03701aaff2a58238f35a586fbc044102b129292492a02c7479e57440b3`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22498c1d73103d486b8e69a684b02839606786d6cff45d0dfbdbdc6e26ce68c`  
		Last Modified: Wed, 11 May 2022 06:27:40 GMT  
		Size: 5.2 MB (5186734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6758dfdb3a7588b70d2a3af8806cc9cea3dee7221cfe99f32973d6c0eee71d46`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fcc234dd9c90350b33b0e204d793aec0e7ee86952bb815ce76739eced0d2a7`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
