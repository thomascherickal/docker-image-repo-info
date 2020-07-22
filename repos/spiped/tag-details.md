<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6.1`](#spiped161)
-	[`spiped:1.6.1-alpine`](#spiped161-alpine)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:6129140a0dd48f9711b9367a7efeeca66e2202fd00d2f75e140c1ef37fac7e9a
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
$ docker pull spiped@sha256:1b3703b88c0276c49f6418cee6564711b22776ffac26ec226cd6ed3e5d597923
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e40d718c053f12a2f6145e68d9d8628a8316d4d443be41670b50186bb4d865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:00:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 22:00:49 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 22:00:50 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 22:01:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 22:01:21 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 22:01:22 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 22:01:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 22:01:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 22:01:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e455e1b26a4f40221478d7ce62207280d0d13dedbfc7ca0aaf58c4340e0ddee8`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccce412a71b5cfa4e30d597dd3a99cfe0db930c43a313bf55a4f714a1e3e46`  
		Last Modified: Wed, 22 Jul 2020 22:01:39 GMT  
		Size: 2.1 MB (2128096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf999adeab53fe5283762e7b188189794e3ab64b206b60b0cbaadbb2b4ebfb5`  
		Last Modified: Wed, 22 Jul 2020 22:01:40 GMT  
		Size: 7.0 MB (7037497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cb2457cdb40f945efdbe8b28f3b34265e1c058d0157ed4d9229949c448fede`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a140f8355f046a042ebbc60094d8df9aebef5deec4ed96b1f68d9cd26ff79bc0`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d579ff53e9f098ca5302da04688adf241acc6a6fc5c312568ad7026dac593f99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32158635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068f8aa8788dd30b663d90eabc6f45ce51c7d7b44af43c1d1a4c788fd829f1d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 11:55:00 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 11:55:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 11:55:28 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 11:55:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 11:55:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 11:56:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 11:56:46 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 11:56:51 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 11:57:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 11:57:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2247b2168e35dbb6dfd4b1589a58bbf99add0a73af4096368bda396424781b8`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fa12e0310a5b57ebc77665d5d0c845d88a29e87f388db311bf39431a2649a5`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 1.8 MB (1839141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4453e159e5f958783f7db893c759f8bdd910010d892eaf0583399934fc223993`  
		Last Modified: Wed, 22 Jul 2020 11:57:20 GMT  
		Size: 5.5 MB (5479836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a514030c90100f9b79199a1f73ec5385edcb84112216f8895f4508bd0dc175`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821be186d03255369b8f4e19ab7fc104245f1589083536c2e96c2b49b6565574`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bc1311bdb1275c4708af8e2cd81cb1dd11f150778a1a9e13ec6d53ee97510cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df99957146f952e25c16b1313937c5316adf6e8007df66cc58ec7de40faddc89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:01:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:02:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:02:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:02:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:02:26 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:03:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:03:56 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:04:09 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:04:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:04:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22172af0169afa0272ff72035f6096febc5d3ede60ac04dc881d1f5800d26c5`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7f1fd14038efa078ebf94b7a162c116dccf414d7b1808cacccce99b0901b06`  
		Last Modified: Wed, 22 Jul 2020 20:05:19 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1cf7eb0ad13a880b9671f96239921ce5ef54c2f5d80739d3767cc6e9f4192d`  
		Last Modified: Wed, 22 Jul 2020 20:05:20 GMT  
		Size: 5.3 MB (5285371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a87f0dff307fe9f323cfd1b1b1cd03c3f80c7cf20ad189e632d3c404ec98b12`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffa36fa5c9d9b8b60adccf7841ed87be33586cfbc5df3f60268deccfc6e47c9`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:90ca459f2716fe31678308da1cd62d0af7b79d87b0401a7d3d0a776e1acc4ac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd226f254c3be89ceb9c4bb6c20aefdc133df54afeb798bcdd4098fcb0a2892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:07:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:52 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:07:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:07:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:08:58 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:08:59 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:08:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:09:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:09:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090da1add6f1974e46f26d2d7f7f722c2b387919c849185bb10a219206f22062`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a8617f0abd2a6ab983a2f2837188637dfb2b47534998d9b7434d28953a4ffc`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 2.0 MB (2007866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f1e6d3329bb93eadc02dee0f5a04eff651b1486c3c23b92fa66712d006b6e`  
		Last Modified: Wed, 22 Jul 2020 20:09:20 GMT  
		Size: 5.9 MB (5905349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31b1358e9f5e7cdb9a68fcac0ed93383f258525c9c26077aeb1861ffb6f52c`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a275c88ee92c00f538ac7771d7a052faf8a375fa59f2b9a2df2935bb34b44`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:8dda3d4d3c2288997850bbe0fcf1dfa852e844ae550118af7990c42833f5ff0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41522530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880155f5e1a96b4e9ca7c51aabc7ccdfeb18dbca3db4a9cd5ca3fba90dba0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:05:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 08:06:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 08:06:04 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 08:06:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 08:06:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 08:06:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 08:06:49 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 08:06:49 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 08:06:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 08:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 08:06:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44566e5b0780af71b3474b5db816d692a1751f17d977e01ee00f59979fead1a`  
		Last Modified: Wed, 22 Jul 2020 08:07:09 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137761b5a755ecd827e03731a861a0fd27f94cf4fc665321f5ffaa89267832e1`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 2.1 MB (2132370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e792a9fde75856fb89ac455423c5f4d5f7ef5b4cf697c63068bbb4f1d57592c6`  
		Last Modified: Wed, 22 Jul 2020 08:07:15 GMT  
		Size: 11.6 MB (11633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc09974b140a07903597f5f2f52e6802438721de8035cf2028d4dba93d72114`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90da1a4bd68ddb52933ffa95caee07d7ace6dbce70422ca720484990d8deeb74`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:93ae2066bfdc02531da3da8cae5f93eba32e347f85ce3f561c255d43881c05e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33894712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4fcc6c7833acebd858160da2ad7c38681d33d3d7423d04d82a8330264d85df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:09:52 GMT
ADD file:67401cc8bdd27435a027e4051d2eb03c5012a09274aaae230008279234586dfb in / 
# Wed, 22 Jul 2020 01:09:53 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 09:31:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 09:31:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 09:31:50 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 09:31:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 09:31:51 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 09:33:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 09:33:00 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 09:33:01 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 09:33:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 09:33:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 09:33:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2cab09a0ed78d8465b06bc43bf504e7c4ed41f36db2ee9cb181c154d562fc9ff`  
		Last Modified: Wed, 22 Jul 2020 01:16:46 GMT  
		Size: 25.8 MB (25764196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6512f4c9c1e27a90f732157f10c587c8363c1da8080af86f85f5564f766fe4`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a0faad5c0d7789e26ba3a662da954e520026f141c1a953a689c533ee1de2e4`  
		Last Modified: Wed, 22 Jul 2020 09:33:26 GMT  
		Size: 1.7 MB (1712068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f30682f51a7d5b7e9956a83541ba90056ce83717835b03f0e9304d721c0b1e0`  
		Last Modified: Wed, 22 Jul 2020 09:33:32 GMT  
		Size: 6.4 MB (6416275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfd3e81b7a925705552310c3a374c4c2155424f80196aa74e8219b099d523a8`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b26bbb062efbcc8c7b44ba0630b2ed24d653b6c55936308a60e22472e9593cc`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:03995222204f42731f98501b4c8c18a9db227d90803b22f30298cc9bfa2241e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39495107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7e2cc3865ddde7c94f2590b83a5b98fa4ca1edf4a7492e052779511b077b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 07:06:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 07:06:54 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 07:07:00 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 07:07:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 07:07:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 07:10:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 07:10:43 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 07:10:50 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 07:10:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 07:10:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 07:10:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e44820d7bbc26a2b3c415a83a4b412124792c2a83acab9a81e7ec244c2c8666`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6e4b1dfc938633e7aae1d4c18c403695eeedb53442abf163bcb83ac6ed8668`  
		Last Modified: Wed, 22 Jul 2020 07:11:29 GMT  
		Size: 2.2 MB (2224929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b74dd8da59a63b4991768759a3e508854f1426b515e80f8c8fcd372ca7ebdff`  
		Last Modified: Wed, 22 Jul 2020 07:11:30 GMT  
		Size: 6.7 MB (6743404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedc9bb952e4419de60a68e2016a1270e9d7e1f08a63719ceaffad505adb216`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713cfc1b4e05eabe0b530ad9fe50a531c48c0fff7525925a733aaca8c9543ab`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:988ca0d41da781226f1f8b397db321e58672ad6497f5582c2ab77121ebbffebc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33480102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5914e06481e56c8eba30dab827747d776a44c8e5766134d225ad478a1f28e0db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:41 GMT
ADD file:2864b647009a85c176c3aeb2d75843b9336b02a18412124b8a03710df61dc971 in / 
# Wed, 22 Jul 2020 00:42:43 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:57:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 05:57:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 05:58:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 05:58:08 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 05:58:08 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 05:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 05:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 05:58:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:71104c8b0e24cdcb6152cf3a5afb2944f578c741e6defa1905768c590598a79a`  
		Last Modified: Wed, 22 Jul 2020 00:45:48 GMT  
		Size: 25.7 MB (25712820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32049947a686f99b19a2dccd83dd1d6e34e07c87916e6b7b317a97636bf39599`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de075e42314ed529d0506784c96bc9064de45ce3f55a604eb181c0a2677cb4ee`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 1.8 MB (1821744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3187de5d650d2a9a9cdf4512e41f3075175a871809da4966ee1b561fcd9cff1d`  
		Last Modified: Wed, 22 Jul 2020 05:58:32 GMT  
		Size: 5.9 MB (5943332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33958405af750e7967cd969177a479077fec1ebc451ca33d1a651eb8ec545912`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e26d1992c44f1e55fb700104063494dfa86a9990e61e9b61b8686e96a6106`  
		Last Modified: Wed, 22 Jul 2020 05:58:31 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:6129140a0dd48f9711b9367a7efeeca66e2202fd00d2f75e140c1ef37fac7e9a
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
$ docker pull spiped@sha256:1b3703b88c0276c49f6418cee6564711b22776ffac26ec226cd6ed3e5d597923
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e40d718c053f12a2f6145e68d9d8628a8316d4d443be41670b50186bb4d865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:00:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 22:00:49 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 22:00:50 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 22:01:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 22:01:21 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 22:01:22 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 22:01:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 22:01:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 22:01:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e455e1b26a4f40221478d7ce62207280d0d13dedbfc7ca0aaf58c4340e0ddee8`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccce412a71b5cfa4e30d597dd3a99cfe0db930c43a313bf55a4f714a1e3e46`  
		Last Modified: Wed, 22 Jul 2020 22:01:39 GMT  
		Size: 2.1 MB (2128096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf999adeab53fe5283762e7b188189794e3ab64b206b60b0cbaadbb2b4ebfb5`  
		Last Modified: Wed, 22 Jul 2020 22:01:40 GMT  
		Size: 7.0 MB (7037497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cb2457cdb40f945efdbe8b28f3b34265e1c058d0157ed4d9229949c448fede`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a140f8355f046a042ebbc60094d8df9aebef5deec4ed96b1f68d9cd26ff79bc0`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d579ff53e9f098ca5302da04688adf241acc6a6fc5c312568ad7026dac593f99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32158635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068f8aa8788dd30b663d90eabc6f45ce51c7d7b44af43c1d1a4c788fd829f1d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 11:55:00 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 11:55:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 11:55:28 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 11:55:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 11:55:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 11:56:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 11:56:46 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 11:56:51 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 11:57:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 11:57:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2247b2168e35dbb6dfd4b1589a58bbf99add0a73af4096368bda396424781b8`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fa12e0310a5b57ebc77665d5d0c845d88a29e87f388db311bf39431a2649a5`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 1.8 MB (1839141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4453e159e5f958783f7db893c759f8bdd910010d892eaf0583399934fc223993`  
		Last Modified: Wed, 22 Jul 2020 11:57:20 GMT  
		Size: 5.5 MB (5479836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a514030c90100f9b79199a1f73ec5385edcb84112216f8895f4508bd0dc175`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821be186d03255369b8f4e19ab7fc104245f1589083536c2e96c2b49b6565574`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bc1311bdb1275c4708af8e2cd81cb1dd11f150778a1a9e13ec6d53ee97510cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df99957146f952e25c16b1313937c5316adf6e8007df66cc58ec7de40faddc89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:01:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:02:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:02:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:02:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:02:26 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:03:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:03:56 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:04:09 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:04:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:04:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22172af0169afa0272ff72035f6096febc5d3ede60ac04dc881d1f5800d26c5`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7f1fd14038efa078ebf94b7a162c116dccf414d7b1808cacccce99b0901b06`  
		Last Modified: Wed, 22 Jul 2020 20:05:19 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1cf7eb0ad13a880b9671f96239921ce5ef54c2f5d80739d3767cc6e9f4192d`  
		Last Modified: Wed, 22 Jul 2020 20:05:20 GMT  
		Size: 5.3 MB (5285371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a87f0dff307fe9f323cfd1b1b1cd03c3f80c7cf20ad189e632d3c404ec98b12`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffa36fa5c9d9b8b60adccf7841ed87be33586cfbc5df3f60268deccfc6e47c9`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:90ca459f2716fe31678308da1cd62d0af7b79d87b0401a7d3d0a776e1acc4ac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd226f254c3be89ceb9c4bb6c20aefdc133df54afeb798bcdd4098fcb0a2892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:07:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:52 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:07:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:07:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:08:58 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:08:59 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:08:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:09:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:09:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090da1add6f1974e46f26d2d7f7f722c2b387919c849185bb10a219206f22062`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a8617f0abd2a6ab983a2f2837188637dfb2b47534998d9b7434d28953a4ffc`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 2.0 MB (2007866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f1e6d3329bb93eadc02dee0f5a04eff651b1486c3c23b92fa66712d006b6e`  
		Last Modified: Wed, 22 Jul 2020 20:09:20 GMT  
		Size: 5.9 MB (5905349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31b1358e9f5e7cdb9a68fcac0ed93383f258525c9c26077aeb1861ffb6f52c`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a275c88ee92c00f538ac7771d7a052faf8a375fa59f2b9a2df2935bb34b44`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:8dda3d4d3c2288997850bbe0fcf1dfa852e844ae550118af7990c42833f5ff0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41522530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880155f5e1a96b4e9ca7c51aabc7ccdfeb18dbca3db4a9cd5ca3fba90dba0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:05:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 08:06:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 08:06:04 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 08:06:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 08:06:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 08:06:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 08:06:49 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 08:06:49 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 08:06:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 08:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 08:06:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44566e5b0780af71b3474b5db816d692a1751f17d977e01ee00f59979fead1a`  
		Last Modified: Wed, 22 Jul 2020 08:07:09 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137761b5a755ecd827e03731a861a0fd27f94cf4fc665321f5ffaa89267832e1`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 2.1 MB (2132370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e792a9fde75856fb89ac455423c5f4d5f7ef5b4cf697c63068bbb4f1d57592c6`  
		Last Modified: Wed, 22 Jul 2020 08:07:15 GMT  
		Size: 11.6 MB (11633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc09974b140a07903597f5f2f52e6802438721de8035cf2028d4dba93d72114`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90da1a4bd68ddb52933ffa95caee07d7ace6dbce70422ca720484990d8deeb74`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:93ae2066bfdc02531da3da8cae5f93eba32e347f85ce3f561c255d43881c05e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33894712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4fcc6c7833acebd858160da2ad7c38681d33d3d7423d04d82a8330264d85df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:09:52 GMT
ADD file:67401cc8bdd27435a027e4051d2eb03c5012a09274aaae230008279234586dfb in / 
# Wed, 22 Jul 2020 01:09:53 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 09:31:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 09:31:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 09:31:50 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 09:31:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 09:31:51 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 09:33:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 09:33:00 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 09:33:01 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 09:33:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 09:33:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 09:33:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2cab09a0ed78d8465b06bc43bf504e7c4ed41f36db2ee9cb181c154d562fc9ff`  
		Last Modified: Wed, 22 Jul 2020 01:16:46 GMT  
		Size: 25.8 MB (25764196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6512f4c9c1e27a90f732157f10c587c8363c1da8080af86f85f5564f766fe4`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a0faad5c0d7789e26ba3a662da954e520026f141c1a953a689c533ee1de2e4`  
		Last Modified: Wed, 22 Jul 2020 09:33:26 GMT  
		Size: 1.7 MB (1712068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f30682f51a7d5b7e9956a83541ba90056ce83717835b03f0e9304d721c0b1e0`  
		Last Modified: Wed, 22 Jul 2020 09:33:32 GMT  
		Size: 6.4 MB (6416275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfd3e81b7a925705552310c3a374c4c2155424f80196aa74e8219b099d523a8`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b26bbb062efbcc8c7b44ba0630b2ed24d653b6c55936308a60e22472e9593cc`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:03995222204f42731f98501b4c8c18a9db227d90803b22f30298cc9bfa2241e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39495107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7e2cc3865ddde7c94f2590b83a5b98fa4ca1edf4a7492e052779511b077b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 07:06:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 07:06:54 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 07:07:00 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 07:07:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 07:07:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 07:10:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 07:10:43 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 07:10:50 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 07:10:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 07:10:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 07:10:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e44820d7bbc26a2b3c415a83a4b412124792c2a83acab9a81e7ec244c2c8666`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6e4b1dfc938633e7aae1d4c18c403695eeedb53442abf163bcb83ac6ed8668`  
		Last Modified: Wed, 22 Jul 2020 07:11:29 GMT  
		Size: 2.2 MB (2224929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b74dd8da59a63b4991768759a3e508854f1426b515e80f8c8fcd372ca7ebdff`  
		Last Modified: Wed, 22 Jul 2020 07:11:30 GMT  
		Size: 6.7 MB (6743404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedc9bb952e4419de60a68e2016a1270e9d7e1f08a63719ceaffad505adb216`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713cfc1b4e05eabe0b530ad9fe50a531c48c0fff7525925a733aaca8c9543ab`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:988ca0d41da781226f1f8b397db321e58672ad6497f5582c2ab77121ebbffebc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33480102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5914e06481e56c8eba30dab827747d776a44c8e5766134d225ad478a1f28e0db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:41 GMT
ADD file:2864b647009a85c176c3aeb2d75843b9336b02a18412124b8a03710df61dc971 in / 
# Wed, 22 Jul 2020 00:42:43 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:57:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 05:57:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 05:58:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 05:58:08 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 05:58:08 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 05:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 05:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 05:58:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:71104c8b0e24cdcb6152cf3a5afb2944f578c741e6defa1905768c590598a79a`  
		Last Modified: Wed, 22 Jul 2020 00:45:48 GMT  
		Size: 25.7 MB (25712820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32049947a686f99b19a2dccd83dd1d6e34e07c87916e6b7b317a97636bf39599`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de075e42314ed529d0506784c96bc9064de45ce3f55a604eb181c0a2677cb4ee`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 1.8 MB (1821744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3187de5d650d2a9a9cdf4512e41f3075175a871809da4966ee1b561fcd9cff1d`  
		Last Modified: Wed, 22 Jul 2020 05:58:32 GMT  
		Size: 5.9 MB (5943332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33958405af750e7967cd969177a479077fec1ebc451ca33d1a651eb8ec545912`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e26d1992c44f1e55fb700104063494dfa86a9990e61e9b61b8686e96a6106`  
		Last Modified: Wed, 22 Jul 2020 05:58:31 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:6129140a0dd48f9711b9367a7efeeca66e2202fd00d2f75e140c1ef37fac7e9a
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
$ docker pull spiped@sha256:1b3703b88c0276c49f6418cee6564711b22776ffac26ec226cd6ed3e5d597923
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e40d718c053f12a2f6145e68d9d8628a8316d4d443be41670b50186bb4d865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:00:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 22:00:49 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 22:00:50 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 22:01:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 22:01:21 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 22:01:22 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 22:01:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 22:01:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 22:01:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e455e1b26a4f40221478d7ce62207280d0d13dedbfc7ca0aaf58c4340e0ddee8`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccce412a71b5cfa4e30d597dd3a99cfe0db930c43a313bf55a4f714a1e3e46`  
		Last Modified: Wed, 22 Jul 2020 22:01:39 GMT  
		Size: 2.1 MB (2128096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf999adeab53fe5283762e7b188189794e3ab64b206b60b0cbaadbb2b4ebfb5`  
		Last Modified: Wed, 22 Jul 2020 22:01:40 GMT  
		Size: 7.0 MB (7037497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cb2457cdb40f945efdbe8b28f3b34265e1c058d0157ed4d9229949c448fede`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a140f8355f046a042ebbc60094d8df9aebef5deec4ed96b1f68d9cd26ff79bc0`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d579ff53e9f098ca5302da04688adf241acc6a6fc5c312568ad7026dac593f99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32158635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068f8aa8788dd30b663d90eabc6f45ce51c7d7b44af43c1d1a4c788fd829f1d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 11:55:00 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 11:55:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 11:55:28 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 11:55:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 11:55:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 11:56:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 11:56:46 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 11:56:51 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 11:57:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 11:57:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2247b2168e35dbb6dfd4b1589a58bbf99add0a73af4096368bda396424781b8`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fa12e0310a5b57ebc77665d5d0c845d88a29e87f388db311bf39431a2649a5`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 1.8 MB (1839141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4453e159e5f958783f7db893c759f8bdd910010d892eaf0583399934fc223993`  
		Last Modified: Wed, 22 Jul 2020 11:57:20 GMT  
		Size: 5.5 MB (5479836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a514030c90100f9b79199a1f73ec5385edcb84112216f8895f4508bd0dc175`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821be186d03255369b8f4e19ab7fc104245f1589083536c2e96c2b49b6565574`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bc1311bdb1275c4708af8e2cd81cb1dd11f150778a1a9e13ec6d53ee97510cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df99957146f952e25c16b1313937c5316adf6e8007df66cc58ec7de40faddc89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:01:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:02:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:02:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:02:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:02:26 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:03:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:03:56 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:04:09 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:04:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:04:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22172af0169afa0272ff72035f6096febc5d3ede60ac04dc881d1f5800d26c5`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7f1fd14038efa078ebf94b7a162c116dccf414d7b1808cacccce99b0901b06`  
		Last Modified: Wed, 22 Jul 2020 20:05:19 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1cf7eb0ad13a880b9671f96239921ce5ef54c2f5d80739d3767cc6e9f4192d`  
		Last Modified: Wed, 22 Jul 2020 20:05:20 GMT  
		Size: 5.3 MB (5285371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a87f0dff307fe9f323cfd1b1b1cd03c3f80c7cf20ad189e632d3c404ec98b12`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffa36fa5c9d9b8b60adccf7841ed87be33586cfbc5df3f60268deccfc6e47c9`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:90ca459f2716fe31678308da1cd62d0af7b79d87b0401a7d3d0a776e1acc4ac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd226f254c3be89ceb9c4bb6c20aefdc133df54afeb798bcdd4098fcb0a2892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:07:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:52 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:07:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:07:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:08:58 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:08:59 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:08:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:09:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:09:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090da1add6f1974e46f26d2d7f7f722c2b387919c849185bb10a219206f22062`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a8617f0abd2a6ab983a2f2837188637dfb2b47534998d9b7434d28953a4ffc`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 2.0 MB (2007866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f1e6d3329bb93eadc02dee0f5a04eff651b1486c3c23b92fa66712d006b6e`  
		Last Modified: Wed, 22 Jul 2020 20:09:20 GMT  
		Size: 5.9 MB (5905349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31b1358e9f5e7cdb9a68fcac0ed93383f258525c9c26077aeb1861ffb6f52c`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a275c88ee92c00f538ac7771d7a052faf8a375fa59f2b9a2df2935bb34b44`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:8dda3d4d3c2288997850bbe0fcf1dfa852e844ae550118af7990c42833f5ff0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41522530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880155f5e1a96b4e9ca7c51aabc7ccdfeb18dbca3db4a9cd5ca3fba90dba0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:05:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 08:06:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 08:06:04 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 08:06:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 08:06:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 08:06:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 08:06:49 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 08:06:49 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 08:06:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 08:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 08:06:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44566e5b0780af71b3474b5db816d692a1751f17d977e01ee00f59979fead1a`  
		Last Modified: Wed, 22 Jul 2020 08:07:09 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137761b5a755ecd827e03731a861a0fd27f94cf4fc665321f5ffaa89267832e1`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 2.1 MB (2132370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e792a9fde75856fb89ac455423c5f4d5f7ef5b4cf697c63068bbb4f1d57592c6`  
		Last Modified: Wed, 22 Jul 2020 08:07:15 GMT  
		Size: 11.6 MB (11633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc09974b140a07903597f5f2f52e6802438721de8035cf2028d4dba93d72114`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90da1a4bd68ddb52933ffa95caee07d7ace6dbce70422ca720484990d8deeb74`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:93ae2066bfdc02531da3da8cae5f93eba32e347f85ce3f561c255d43881c05e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33894712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4fcc6c7833acebd858160da2ad7c38681d33d3d7423d04d82a8330264d85df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:09:52 GMT
ADD file:67401cc8bdd27435a027e4051d2eb03c5012a09274aaae230008279234586dfb in / 
# Wed, 22 Jul 2020 01:09:53 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 09:31:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 09:31:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 09:31:50 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 09:31:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 09:31:51 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 09:33:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 09:33:00 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 09:33:01 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 09:33:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 09:33:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 09:33:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2cab09a0ed78d8465b06bc43bf504e7c4ed41f36db2ee9cb181c154d562fc9ff`  
		Last Modified: Wed, 22 Jul 2020 01:16:46 GMT  
		Size: 25.8 MB (25764196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6512f4c9c1e27a90f732157f10c587c8363c1da8080af86f85f5564f766fe4`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a0faad5c0d7789e26ba3a662da954e520026f141c1a953a689c533ee1de2e4`  
		Last Modified: Wed, 22 Jul 2020 09:33:26 GMT  
		Size: 1.7 MB (1712068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f30682f51a7d5b7e9956a83541ba90056ce83717835b03f0e9304d721c0b1e0`  
		Last Modified: Wed, 22 Jul 2020 09:33:32 GMT  
		Size: 6.4 MB (6416275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfd3e81b7a925705552310c3a374c4c2155424f80196aa74e8219b099d523a8`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b26bbb062efbcc8c7b44ba0630b2ed24d653b6c55936308a60e22472e9593cc`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:03995222204f42731f98501b4c8c18a9db227d90803b22f30298cc9bfa2241e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39495107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7e2cc3865ddde7c94f2590b83a5b98fa4ca1edf4a7492e052779511b077b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 07:06:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 07:06:54 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 07:07:00 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 07:07:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 07:07:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 07:10:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 07:10:43 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 07:10:50 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 07:10:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 07:10:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 07:10:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e44820d7bbc26a2b3c415a83a4b412124792c2a83acab9a81e7ec244c2c8666`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6e4b1dfc938633e7aae1d4c18c403695eeedb53442abf163bcb83ac6ed8668`  
		Last Modified: Wed, 22 Jul 2020 07:11:29 GMT  
		Size: 2.2 MB (2224929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b74dd8da59a63b4991768759a3e508854f1426b515e80f8c8fcd372ca7ebdff`  
		Last Modified: Wed, 22 Jul 2020 07:11:30 GMT  
		Size: 6.7 MB (6743404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedc9bb952e4419de60a68e2016a1270e9d7e1f08a63719ceaffad505adb216`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713cfc1b4e05eabe0b530ad9fe50a531c48c0fff7525925a733aaca8c9543ab`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:988ca0d41da781226f1f8b397db321e58672ad6497f5582c2ab77121ebbffebc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33480102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5914e06481e56c8eba30dab827747d776a44c8e5766134d225ad478a1f28e0db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:41 GMT
ADD file:2864b647009a85c176c3aeb2d75843b9336b02a18412124b8a03710df61dc971 in / 
# Wed, 22 Jul 2020 00:42:43 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:57:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 05:57:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 05:58:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 05:58:08 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 05:58:08 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 05:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 05:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 05:58:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:71104c8b0e24cdcb6152cf3a5afb2944f578c741e6defa1905768c590598a79a`  
		Last Modified: Wed, 22 Jul 2020 00:45:48 GMT  
		Size: 25.7 MB (25712820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32049947a686f99b19a2dccd83dd1d6e34e07c87916e6b7b317a97636bf39599`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de075e42314ed529d0506784c96bc9064de45ce3f55a604eb181c0a2677cb4ee`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 1.8 MB (1821744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3187de5d650d2a9a9cdf4512e41f3075175a871809da4966ee1b561fcd9cff1d`  
		Last Modified: Wed, 22 Jul 2020 05:58:32 GMT  
		Size: 5.9 MB (5943332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33958405af750e7967cd969177a479077fec1ebc451ca33d1a651eb8ec545912`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e26d1992c44f1e55fb700104063494dfa86a9990e61e9b61b8686e96a6106`  
		Last Modified: Wed, 22 Jul 2020 05:58:31 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:6129140a0dd48f9711b9367a7efeeca66e2202fd00d2f75e140c1ef37fac7e9a
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
$ docker pull spiped@sha256:1b3703b88c0276c49f6418cee6564711b22776ffac26ec226cd6ed3e5d597923
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e40d718c053f12a2f6145e68d9d8628a8316d4d443be41670b50186bb4d865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:00:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 22:00:49 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 22:00:50 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 22:01:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 22:01:21 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 22:01:22 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 22:01:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 22:01:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 22:01:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e455e1b26a4f40221478d7ce62207280d0d13dedbfc7ca0aaf58c4340e0ddee8`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccce412a71b5cfa4e30d597dd3a99cfe0db930c43a313bf55a4f714a1e3e46`  
		Last Modified: Wed, 22 Jul 2020 22:01:39 GMT  
		Size: 2.1 MB (2128096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf999adeab53fe5283762e7b188189794e3ab64b206b60b0cbaadbb2b4ebfb5`  
		Last Modified: Wed, 22 Jul 2020 22:01:40 GMT  
		Size: 7.0 MB (7037497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cb2457cdb40f945efdbe8b28f3b34265e1c058d0157ed4d9229949c448fede`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a140f8355f046a042ebbc60094d8df9aebef5deec4ed96b1f68d9cd26ff79bc0`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d579ff53e9f098ca5302da04688adf241acc6a6fc5c312568ad7026dac593f99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32158635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068f8aa8788dd30b663d90eabc6f45ce51c7d7b44af43c1d1a4c788fd829f1d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 11:55:00 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 11:55:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 11:55:28 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 11:55:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 11:55:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 11:56:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 11:56:46 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 11:56:51 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 11:57:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 11:57:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2247b2168e35dbb6dfd4b1589a58bbf99add0a73af4096368bda396424781b8`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fa12e0310a5b57ebc77665d5d0c845d88a29e87f388db311bf39431a2649a5`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 1.8 MB (1839141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4453e159e5f958783f7db893c759f8bdd910010d892eaf0583399934fc223993`  
		Last Modified: Wed, 22 Jul 2020 11:57:20 GMT  
		Size: 5.5 MB (5479836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a514030c90100f9b79199a1f73ec5385edcb84112216f8895f4508bd0dc175`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821be186d03255369b8f4e19ab7fc104245f1589083536c2e96c2b49b6565574`  
		Last Modified: Wed, 22 Jul 2020 11:57:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bc1311bdb1275c4708af8e2cd81cb1dd11f150778a1a9e13ec6d53ee97510cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df99957146f952e25c16b1313937c5316adf6e8007df66cc58ec7de40faddc89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:01:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:02:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:02:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:02:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:02:26 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:03:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:03:56 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:04:09 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:04:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:04:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22172af0169afa0272ff72035f6096febc5d3ede60ac04dc881d1f5800d26c5`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7f1fd14038efa078ebf94b7a162c116dccf414d7b1808cacccce99b0901b06`  
		Last Modified: Wed, 22 Jul 2020 20:05:19 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1cf7eb0ad13a880b9671f96239921ce5ef54c2f5d80739d3767cc6e9f4192d`  
		Last Modified: Wed, 22 Jul 2020 20:05:20 GMT  
		Size: 5.3 MB (5285371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a87f0dff307fe9f323cfd1b1b1cd03c3f80c7cf20ad189e632d3c404ec98b12`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffa36fa5c9d9b8b60adccf7841ed87be33586cfbc5df3f60268deccfc6e47c9`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:90ca459f2716fe31678308da1cd62d0af7b79d87b0401a7d3d0a776e1acc4ac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd226f254c3be89ceb9c4bb6c20aefdc133df54afeb798bcdd4098fcb0a2892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:07:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:52 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:07:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:07:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:08:58 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:08:59 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:08:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:09:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:09:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090da1add6f1974e46f26d2d7f7f722c2b387919c849185bb10a219206f22062`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a8617f0abd2a6ab983a2f2837188637dfb2b47534998d9b7434d28953a4ffc`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 2.0 MB (2007866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f1e6d3329bb93eadc02dee0f5a04eff651b1486c3c23b92fa66712d006b6e`  
		Last Modified: Wed, 22 Jul 2020 20:09:20 GMT  
		Size: 5.9 MB (5905349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31b1358e9f5e7cdb9a68fcac0ed93383f258525c9c26077aeb1861ffb6f52c`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a275c88ee92c00f538ac7771d7a052faf8a375fa59f2b9a2df2935bb34b44`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:8dda3d4d3c2288997850bbe0fcf1dfa852e844ae550118af7990c42833f5ff0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41522530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880155f5e1a96b4e9ca7c51aabc7ccdfeb18dbca3db4a9cd5ca3fba90dba0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:05:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 08:06:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 08:06:04 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 08:06:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 08:06:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 08:06:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 08:06:49 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 08:06:49 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 08:06:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 08:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 08:06:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44566e5b0780af71b3474b5db816d692a1751f17d977e01ee00f59979fead1a`  
		Last Modified: Wed, 22 Jul 2020 08:07:09 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137761b5a755ecd827e03731a861a0fd27f94cf4fc665321f5ffaa89267832e1`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 2.1 MB (2132370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e792a9fde75856fb89ac455423c5f4d5f7ef5b4cf697c63068bbb4f1d57592c6`  
		Last Modified: Wed, 22 Jul 2020 08:07:15 GMT  
		Size: 11.6 MB (11633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc09974b140a07903597f5f2f52e6802438721de8035cf2028d4dba93d72114`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90da1a4bd68ddb52933ffa95caee07d7ace6dbce70422ca720484990d8deeb74`  
		Last Modified: Wed, 22 Jul 2020 08:07:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:93ae2066bfdc02531da3da8cae5f93eba32e347f85ce3f561c255d43881c05e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33894712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4fcc6c7833acebd858160da2ad7c38681d33d3d7423d04d82a8330264d85df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:09:52 GMT
ADD file:67401cc8bdd27435a027e4051d2eb03c5012a09274aaae230008279234586dfb in / 
# Wed, 22 Jul 2020 01:09:53 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 09:31:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 09:31:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 09:31:50 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 09:31:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 09:31:51 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 09:33:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 09:33:00 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 09:33:01 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 09:33:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 09:33:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 09:33:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2cab09a0ed78d8465b06bc43bf504e7c4ed41f36db2ee9cb181c154d562fc9ff`  
		Last Modified: Wed, 22 Jul 2020 01:16:46 GMT  
		Size: 25.8 MB (25764196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6512f4c9c1e27a90f732157f10c587c8363c1da8080af86f85f5564f766fe4`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a0faad5c0d7789e26ba3a662da954e520026f141c1a953a689c533ee1de2e4`  
		Last Modified: Wed, 22 Jul 2020 09:33:26 GMT  
		Size: 1.7 MB (1712068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f30682f51a7d5b7e9956a83541ba90056ce83717835b03f0e9304d721c0b1e0`  
		Last Modified: Wed, 22 Jul 2020 09:33:32 GMT  
		Size: 6.4 MB (6416275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfd3e81b7a925705552310c3a374c4c2155424f80196aa74e8219b099d523a8`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b26bbb062efbcc8c7b44ba0630b2ed24d653b6c55936308a60e22472e9593cc`  
		Last Modified: Wed, 22 Jul 2020 09:33:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:03995222204f42731f98501b4c8c18a9db227d90803b22f30298cc9bfa2241e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39495107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7e2cc3865ddde7c94f2590b83a5b98fa4ca1edf4a7492e052779511b077b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 07:06:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 07:06:54 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 07:07:00 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 07:07:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 07:07:06 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 07:10:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 07:10:43 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 07:10:50 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 07:10:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 07:10:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 07:10:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e44820d7bbc26a2b3c415a83a4b412124792c2a83acab9a81e7ec244c2c8666`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6e4b1dfc938633e7aae1d4c18c403695eeedb53442abf163bcb83ac6ed8668`  
		Last Modified: Wed, 22 Jul 2020 07:11:29 GMT  
		Size: 2.2 MB (2224929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b74dd8da59a63b4991768759a3e508854f1426b515e80f8c8fcd372ca7ebdff`  
		Last Modified: Wed, 22 Jul 2020 07:11:30 GMT  
		Size: 6.7 MB (6743404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedc9bb952e4419de60a68e2016a1270e9d7e1f08a63719ceaffad505adb216`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713cfc1b4e05eabe0b530ad9fe50a531c48c0fff7525925a733aaca8c9543ab`  
		Last Modified: Wed, 22 Jul 2020 07:11:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:988ca0d41da781226f1f8b397db321e58672ad6497f5582c2ab77121ebbffebc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33480102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5914e06481e56c8eba30dab827747d776a44c8e5766134d225ad478a1f28e0db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:41 GMT
ADD file:2864b647009a85c176c3aeb2d75843b9336b02a18412124b8a03710df61dc971 in / 
# Wed, 22 Jul 2020 00:42:43 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:57:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 05:57:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 05:57:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 05:58:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 05:58:08 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 05:58:08 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 05:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 05:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 05:58:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:71104c8b0e24cdcb6152cf3a5afb2944f578c741e6defa1905768c590598a79a`  
		Last Modified: Wed, 22 Jul 2020 00:45:48 GMT  
		Size: 25.7 MB (25712820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32049947a686f99b19a2dccd83dd1d6e34e07c87916e6b7b317a97636bf39599`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de075e42314ed529d0506784c96bc9064de45ce3f55a604eb181c0a2677cb4ee`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 1.8 MB (1821744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3187de5d650d2a9a9cdf4512e41f3075175a871809da4966ee1b561fcd9cff1d`  
		Last Modified: Wed, 22 Jul 2020 05:58:32 GMT  
		Size: 5.9 MB (5943332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33958405af750e7967cd969177a479077fec1ebc451ca33d1a651eb8ec545912`  
		Last Modified: Wed, 22 Jul 2020 05:58:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e26d1992c44f1e55fb700104063494dfa86a9990e61e9b61b8686e96a6106`  
		Last Modified: Wed, 22 Jul 2020 05:58:31 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
