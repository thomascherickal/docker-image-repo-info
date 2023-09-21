## `spiped:latest`

```console
$ docker pull spiped@sha256:3e0b302055d6fce03000d591ff49ae4d75d818aef7ab6b1554907327a7903398
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
$ docker pull spiped@sha256:86809c127185cc13c15d1456e139da03ac577f459660c7a4531c71afadb52226
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34305819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b1a40f6ec43487bed3ccebe366888854dcef85fc7031d5c72856997834f477`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:54 GMT
ADD file:a4ac238e8d5bf843acb96f72c03d55e0a7f2fca33ba16d7631d397176acf8c3a in / 
# Wed, 20 Sep 2023 00:49:54 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 16:11:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Sep 2023 16:11:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 16:11:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Sep 2023 16:11:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 16:11:31 GMT
VOLUME [/spiped]
# Wed, 20 Sep 2023 16:11:32 GMT
WORKDIR /spiped
# Wed, 20 Sep 2023 16:11:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Sep 2023 16:11:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 16:11:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9de40a7a125e0755ac5cf1e38c2f8a6b3d3c005cfc82323d13f5dceb50381fd7`  
		Last Modified: Wed, 20 Sep 2023 00:54:44 GMT  
		Size: 27.0 MB (26983563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef3c7a6a349587c40a919213f6918e8c23c8dd47557c50d804fbb5a121acbb1`  
		Last Modified: Wed, 20 Sep 2023 16:11:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef588b895b6c78d1d6c3f8f328d6eb6a5713f823bda5c6175e969a9f51bbc2c`  
		Last Modified: Wed, 20 Sep 2023 16:11:44 GMT  
		Size: 2.2 MB (2184118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75130159a0b64473ad02f239232ae60083edd4a7920ae123e33ba6878e3035`  
		Last Modified: Wed, 20 Sep 2023 16:11:45 GMT  
		Size: 5.1 MB (5136537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb7543f72af5bff46c6c16c388e92dc3c631fb798a6bcd97bc640a3da4cb5d`  
		Last Modified: Wed, 20 Sep 2023 16:11:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3869cd3fa8e6aa3da3e4133a66846dcc44c653007a2b31d117292340d6879a53`  
		Last Modified: Wed, 20 Sep 2023 16:11:44 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:a5cb70fd4b4a936289a12b6d151cdabc0e2cac90fbe275b46d4a15cc86809a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38667188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55712b09ff8abecc36b966650f0899c40416a3cead7efff8fab37c0f7a0120e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:00 GMT
ADD file:0952a54f5474629ed000e89bfd1b8827e49b63270932e45ed8d953a2676ac79c in / 
# Thu, 07 Sep 2023 00:39:00 GMT
CMD ["bash"]
# Fri, 08 Sep 2023 01:22:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 08 Sep 2023 01:22:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 08 Sep 2023 01:22:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 08 Sep 2023 01:23:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 08 Sep 2023 01:23:06 GMT
VOLUME [/spiped]
# Fri, 08 Sep 2023 01:23:06 GMT
WORKDIR /spiped
# Fri, 08 Sep 2023 01:23:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 08 Sep 2023 01:23:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Sep 2023 01:23:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:30ae0f429560d1effd0839849ab7780512b72d9fbc09a6cec67e03092a85a1d1`  
		Last Modified: Thu, 07 Sep 2023 00:43:48 GMT  
		Size: 30.1 MB (30141753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ec572ab01279a092612b8e01d9252a8499967c9c8541b65e8cd69140c02c24`  
		Last Modified: Fri, 08 Sep 2023 01:23:23 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4ffe4efa5e1916eef1126e509649a004207f1b1e987325b45d920ded172798`  
		Last Modified: Fri, 08 Sep 2023 01:23:24 GMT  
		Size: 2.6 MB (2583600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde1ee8b6e1c38f35460e35f265b2034aa196fa2c12c71b2426cf5fa12c67ffc`  
		Last Modified: Fri, 08 Sep 2023 01:23:25 GMT  
		Size: 5.9 MB (5940237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f5a9fe525e96f29957f4ed9470968a01b03335ab2865ca594dee522f605f4d`  
		Last Modified: Fri, 08 Sep 2023 01:23:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6edc4e16b3442ce795cdab93d3ea039cfccd4d61ecbfb29e5ef34aebec95f`  
		Last Modified: Fri, 08 Sep 2023 01:23:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:78a90b24784fa980d784a5948e995a6ce8523ccd1d9b5d66c179e05ff6b055ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36756444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:757e8085aa8fc8338a5f230334c1f05a433c19ffdcf7358b738756ade7ed945c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:11 GMT
ADD file:263719948aa8496c0852aa2ef6c6660c25ce35618af5b1c5bc35c901d853bcf8 in / 
# Thu, 07 Sep 2023 01:09:17 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 14:59:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 07 Sep 2023 14:59:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 14:59:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 07 Sep 2023 15:01:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 15:01:26 GMT
VOLUME [/spiped]
# Thu, 07 Sep 2023 15:01:29 GMT
WORKDIR /spiped
# Thu, 07 Sep 2023 15:01:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 07 Sep 2023 15:01:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 15:01:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6519d39af9071c1099bd2a01d04c824d095fb31f439e10814371707227802ae`  
		Last Modified: Thu, 07 Sep 2023 01:20:14 GMT  
		Size: 29.1 MB (29121387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aefb9a6905bf168eeced8e83a91e7068b7fb4755b8e7857c50c3dcd173b85e5`  
		Last Modified: Thu, 07 Sep 2023 15:01:48 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205c01df5896968bbf6e6317ad4f7d3ea3cad21bce8da9f3d43d160e62304a06`  
		Last Modified: Thu, 07 Sep 2023 15:01:50 GMT  
		Size: 1.8 MB (1831686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6736bbe590ef520568c5c56fd7e96b0513fe8d2efd0e874b5e734cf04939d285`  
		Last Modified: Thu, 07 Sep 2023 15:01:53 GMT  
		Size: 5.8 MB (5801853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71816f5552a92da3f78474b698659b9026050c3b8c048f4d754fffe26169f6a`  
		Last Modified: Thu, 07 Sep 2023 15:01:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d57f9d6402fe11212989b0272189df10b78ed901c1dd2605d1c31c0d18e3c6`  
		Last Modified: Thu, 07 Sep 2023 15:01:48 GMT  
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
