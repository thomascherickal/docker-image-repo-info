## `spiped:latest`

```console
$ docker pull spiped@sha256:6761e8727af27409ecc699a28ca2d3586729b1e494e8d6182b748edd897c1327
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
$ docker pull spiped@sha256:e76b1c808c02cff6fc27f5ddf32027a47ebaf903ffb318f0783d07d127d6f434
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38182164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be37888f8982ac9e3d57591df6f03d787777baaaa4bfb9b18d1a12970454d3ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:40 GMT
ADD file:a1398394375faab8dd9e1e8d584eea96c750fb57ae4ffd2b14624f1cf263561b in / 
# Wed, 20 Sep 2023 04:55:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:48:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Sep 2023 09:48:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:48:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Sep 2023 09:48:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:48:40 GMT
VOLUME [/spiped]
# Wed, 20 Sep 2023 09:48:40 GMT
WORKDIR /spiped
# Wed, 20 Sep 2023 09:48:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:48:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 09:48:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a803e7c4b030119420574a882a52b6431e160fceb7620f61b525d49bc2d58886`  
		Last Modified: Wed, 20 Sep 2023 05:00:22 GMT  
		Size: 29.1 MB (29124705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a021990b2c40f8dd26a2f1efe917efd1e62ea910a160c55fc22a2afd808cbeff`  
		Last Modified: Wed, 20 Sep 2023 09:48:56 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3ac9c8c9902623e96dcc5b0c38fd2a5089655f27acd03e26134b3adc1e499b`  
		Last Modified: Wed, 20 Sep 2023 09:48:56 GMT  
		Size: 2.6 MB (2586433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc71963b9ba7d5fa771ca5dd8c96ee53d0b9f228537e51b170656db5d8a3e1f5`  
		Last Modified: Wed, 20 Sep 2023 09:48:57 GMT  
		Size: 6.5 MB (6469428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d628c4263c81106e8ecdaca6b751a38de11667bec53c0310e53fc2eb587e4f`  
		Last Modified: Wed, 20 Sep 2023 09:48:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55121f4f0a670187e2ceddb504fa70ad508c0933c84bc9e7ba4e36ff487d8cd`  
		Last Modified: Wed, 20 Sep 2023 09:48:56 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7799176f5302e51331d55c3e6254fb7e4faa76b6d0ed80142b7bf948369fdbee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34250748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d9a7cd24cc0d83e6861934ba391d4ca6086687b12ed92b305779e9b243d996c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:20:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 Oct 2023 19:20:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:20:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 Oct 2023 19:20:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:20:50 GMT
VOLUME [/spiped]
# Wed, 11 Oct 2023 19:20:50 GMT
WORKDIR /spiped
# Wed, 11 Oct 2023 19:20:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:20:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Oct 2023 19:20:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5af49fa863d037d2f9615ea00e74ea7cd0bdd90b50b911cdbffd64c02d09d00`  
		Last Modified: Wed, 11 Oct 2023 19:20:59 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5737d30da5f2b3b78b6336777b53401c92ffa1c99f2f591d5cbccc00b83bbcb`  
		Last Modified: Wed, 11 Oct 2023 19:21:00 GMT  
		Size: 2.2 MB (2186862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c10e8ebceec402b584fa43bf6607cbfc23d610ea8d49f19dd9d023101c80f8`  
		Last Modified: Wed, 11 Oct 2023 19:21:01 GMT  
		Size: 5.1 MB (5140134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e666d1e1ffaed8f724d30fc9556446662997ff23cbb4c0a4e0c66c3e94e9de32`  
		Last Modified: Wed, 11 Oct 2023 19:20:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d264160502cfd3c86b49bcda648fbd79ef23c63dca4b297b5a557775f1196f25`  
		Last Modified: Wed, 11 Oct 2023 19:20:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:9543a1f98f3d9e65423a9ca2d8467556ef7d8e9493241e4a5258743bfa22039f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31728760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2605d6d1693ce4b0f18a961a9b788f0656b499b85ddd6c6ecbb9a5909e5743b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:17 GMT
ADD file:56b69c762bd03a9b00a1677740f7209aac08bac69a9e73563e326b9b0efbbfcc in / 
# Wed, 20 Sep 2023 04:57:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:38:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Sep 2023 22:38:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:38:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Sep 2023 22:38:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 22:38:44 GMT
VOLUME [/spiped]
# Wed, 20 Sep 2023 22:38:44 GMT
WORKDIR /spiped
# Wed, 20 Sep 2023 22:38:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:38:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 22:38:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e0b5206657a67707f4c57136f811162ce89a951fec109a406df7508d59e644cb`  
		Last Modified: Wed, 20 Sep 2023 05:01:16 GMT  
		Size: 24.8 MB (24805628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1061ccc02c0488c964beea4097bf4eea9d0f8735c7c4d0076062b61be56d5ad7`  
		Last Modified: Wed, 20 Sep 2023 22:38:57 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf95eead4f1a042d2b8e778bc12b7d01752cf55bd95a45b324cea9e47a9157c`  
		Last Modified: Wed, 20 Sep 2023 22:38:58 GMT  
		Size: 2.0 MB (2043288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5fbfcb75378ed3d8a278c240030b268429413471c37a28a3b40af537dd7bd4`  
		Last Modified: Wed, 20 Sep 2023 22:38:58 GMT  
		Size: 4.9 MB (4878245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61807a032d4bef9273d197a1be2c2c6aac007441e915c2072805f08495409d8d`  
		Last Modified: Wed, 20 Sep 2023 22:38:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa9481959689d10eae7364b77c6c082b446a8e2d678e9a0d38a16992411afde`  
		Last Modified: Wed, 20 Sep 2023 22:38:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:3ba43948c46799c4a9964cfe3214d748b4829927f19ff94ecc9e886a86704957
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37067498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfda20cb781c068e97e7724d2214ae2f2985e579c347447ab81231578e9d94a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 16:50:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Sep 2023 16:50:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 16:50:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Sep 2023 16:50:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 16:50:33 GMT
VOLUME [/spiped]
# Wed, 20 Sep 2023 16:50:33 GMT
WORKDIR /spiped
# Wed, 20 Sep 2023 16:50:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:50:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:50:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2ccb7e9907d93a091be63137ee9a2fdcfbfc4609f5c6e6f9afd9877da666e2`  
		Last Modified: Wed, 20 Sep 2023 16:50:45 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84573b91f49d244476babfbfc292ca4439c2fb4259c33d8ae2a71cf8bd7e6165`  
		Last Modified: Wed, 20 Sep 2023 16:50:46 GMT  
		Size: 2.4 MB (2429830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5911f18a674b7f0506c80830cddab54bb0ab95c145eaa2c67d4cb01235eeda`  
		Last Modified: Wed, 20 Sep 2023 16:50:46 GMT  
		Size: 5.5 MB (5478850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9b77b9261b41602d20d51fb43af721d43f5ed06489a271492c232ceb695725`  
		Last Modified: Wed, 20 Sep 2023 16:50:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7039fdaa79369aa5d0624bc701280f3007edcf91dae47a483113a4c454eee5d9`  
		Last Modified: Wed, 20 Sep 2023 16:50:45 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:0673f967e8ebffe52e77a9dfeb0b623dd48f1b3fa8483c0cc1c4e71baf1c7678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38667364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:177b953a52a354eb92388070b228cc7a8231fd78e193e2a47d85195dab9ec1ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Sep 2023 00:41:55 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Wed, 20 Sep 2023 00:41:56 GMT
CMD ["bash"]
# Thu, 21 Sep 2023 02:25:03 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 21 Sep 2023 02:25:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 02:25:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 21 Sep 2023 02:25:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 21 Sep 2023 02:25:39 GMT
VOLUME [/spiped]
# Thu, 21 Sep 2023 02:25:39 GMT
WORKDIR /spiped
# Thu, 21 Sep 2023 02:25:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 21 Sep 2023 02:25:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 02:25:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d840a881438ebcd34ae05552e7189974036cfbcfefeceede5f34c24a03985389`  
		Last Modified: Thu, 21 Sep 2023 02:25:53 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251feb4c4cf3da7f73f90fd16745077dadd4d53d3f49bc29aabc57358504d5d2`  
		Last Modified: Thu, 21 Sep 2023 02:25:54 GMT  
		Size: 2.6 MB (2583625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea863aa480a6cdc7f1d2dced4805da973a859195223122fa8f487875d99a9b88`  
		Last Modified: Thu, 21 Sep 2023 02:25:55 GMT  
		Size: 5.9 MB (5940245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1221f543c6cd80fe32bf96bddcebcc8cde2bccb858dd9bcc38f0ea1b449d56`  
		Last Modified: Thu, 21 Sep 2023 02:25:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29426699791fb37ece37c84447f1221efd9aba5179bfa49263e2e3e862fed366`  
		Last Modified: Thu, 21 Sep 2023 02:25:53 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:9a937201c736a44cc2d3e70f28616c21fcbe1a9ddc9a705ddb4a8164c9359b96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36756704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b87489bca122746f5392d18d5bbab9dc7a1893d344df50195de8cdb8130e7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Sep 2023 03:10:01 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Wed, 20 Sep 2023 03:10:05 GMT
CMD ["bash"]
# Thu, 21 Sep 2023 19:22:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 21 Sep 2023 19:23:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 19:23:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 21 Sep 2023 19:24:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 21 Sep 2023 19:24:52 GMT
VOLUME [/spiped]
# Thu, 21 Sep 2023 19:24:55 GMT
WORKDIR /spiped
# Thu, 21 Sep 2023 19:24:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 21 Sep 2023 19:25:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 19:25:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cfabb822a698e16c826960e14d72b5e0bbe0e92be64b218eaaae53df71fe8b`  
		Last Modified: Thu, 21 Sep 2023 19:25:27 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61630fa66bee395c6728a113104eed6df50ffc2be8c09d7e0246e6d06f2e9d8d`  
		Last Modified: Thu, 21 Sep 2023 19:25:28 GMT  
		Size: 1.8 MB (1831693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f00bb48b8051607f91c32a906fc88a072d0241b4edf1ffcec7860217a38a0`  
		Last Modified: Thu, 21 Sep 2023 19:25:32 GMT  
		Size: 5.8 MB (5801816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b833401f31be351f843dbbe798c9d7c672a05f2d20321753d36029da0d2c61`  
		Last Modified: Thu, 21 Sep 2023 19:25:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3062602aedfb7c2b8b257212c74d3ed4e57eed14c30ac093155696b2d7ab5ed`  
		Last Modified: Thu, 21 Sep 2023 19:25:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:1c25a95d81409d2dd16594c1c08a90a93e49127b2bd70dbc2da959ba3e5ed426
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42306398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d03ec379e2a600a0f1703248082647e6bd20f1eb5e2e2ac4528d61d7595c057`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Thu, 21 Sep 2023 01:20:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 21 Sep 2023 01:20:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 01:20:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 21 Sep 2023 01:21:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 21 Sep 2023 01:21:11 GMT
VOLUME [/spiped]
# Thu, 21 Sep 2023 01:21:11 GMT
WORKDIR /spiped
# Thu, 21 Sep 2023 01:21:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:21:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 01:21:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8f2dcf99ebd16339edbdefa182d83183bbc17045621cca92a0a4267c3b7ebe`  
		Last Modified: Thu, 21 Sep 2023 01:21:28 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bfe965651d9bc0930efe08265464e3c0408b3fb69387cf4223611672773448`  
		Last Modified: Thu, 21 Sep 2023 01:21:29 GMT  
		Size: 2.8 MB (2765007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14b1a1dc829b3a36a3fdd455cb385584ccc3955a4534b64341f8c5401d7eb78`  
		Last Modified: Thu, 21 Sep 2023 01:21:30 GMT  
		Size: 6.4 MB (6420329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75057e005daf515aeafe4dad12671391700076c79effc82949569a5834ee1bb3`  
		Last Modified: Thu, 21 Sep 2023 01:21:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d31a376314f61feef092c71b857a6a2e7fc0f2f2869a21dc0572aac2ab42d`  
		Last Modified: Thu, 21 Sep 2023 01:21:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:d2abf4aac174af3395664f371c97ce9566b230c5685406ec7fdaa68d70d2c586
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35132864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcb4c8663102c4b20859257d43b3ab1c939604c068016e7ef86cd3e96e9e40a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:50:48 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Sep 2023 10:50:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:50:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Sep 2023 10:51:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:51:08 GMT
VOLUME [/spiped]
# Wed, 20 Sep 2023 10:51:08 GMT
WORKDIR /spiped
# Wed, 20 Sep 2023 10:51:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 10:51:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7603b3b8042e246d9fdc380feee257d5650bc18bf28d2e088db07bcffa15f284`  
		Last Modified: Wed, 20 Sep 2023 10:51:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21d5433ec5639c64479b614c827bf91f2c1b5a6e3c3422312b6de7191a26cc`  
		Last Modified: Wed, 20 Sep 2023 10:51:30 GMT  
		Size: 2.3 MB (2257966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5098180deb0ab1562e894eaec56103f48c7cd66e93bb33e69a34c34eb9b302b`  
		Last Modified: Wed, 20 Sep 2023 10:51:31 GMT  
		Size: 5.4 MB (5383335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717f53b138af46de4b3f6cbeb4d43e7aa6c563a59dbf1594f8938a5fe8659201`  
		Last Modified: Wed, 20 Sep 2023 10:51:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d840c75eef35fb2d831c42563d4c545ea314f13223f4b95dfda482126a4bc79f`  
		Last Modified: Wed, 20 Sep 2023 10:51:30 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
