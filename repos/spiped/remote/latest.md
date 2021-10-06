## `spiped:latest`

```console
$ docker pull spiped@sha256:3b91c14c0efb94dbdc7b973bf694116ceeec7aeeb54d8c41c7e671239b70c7b3
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
$ docker pull spiped@sha256:1494dd15abab70ff861f11b7aadcfb1913d7ad7e0c95fd9fa866fd8a997faae6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37332544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe7196e9627619f9949f053a86afbc40496ceea34000b3b4ebaf24419e51df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 22:24:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 22:24:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 22:24:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 22:25:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 22:25:00 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 22:25:01 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 22:25:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 22:25:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:25:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c16f44407339913efe8feb7893634dfbd49fdb363f86acc003a5264fd624a`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c6c38eeca4ff05d1e9ec76ba7d4487d0301289ccb5e1887cc097cb52812f0`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d3ddbaa314fafbcacbfc77277508c88563cf86d10c7ef081d1c2192c94fe62`  
		Last Modified: Tue, 28 Sep 2021 22:25:23 GMT  
		Size: 6.0 MB (5960379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70bf92a5d2ba79534d0d2f8bddde011587181eddf3b8f0d4a195d014da730fb`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef36802cb5494594cbe25bf22ec477072dfe41486e99081666044bdd6d25fd3`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8436dc3d0b9307c6728fddf500bbfc53e22883abd81495bef1dbd786b56533a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6464f913e7d0a0d02b9c987ff12c419ca24b2f6a2b1c36ca7a5ec61982e60e32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:38 GMT
ADD file:da0067258fc1c6a50273e6b3b2673e88fad974a5a1fe4d5eecfeca2df1ff54b3 in / 
# Tue, 28 Sep 2021 01:50:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 19:39:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 19:39:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 19:39:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 19:40:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 19:40:18 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 19:40:18 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 19:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 19:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 19:40:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86f2b8be18fc44e8eb430e2c472979a79cda6eb6fa3add10cc8c5d8764eb90ac`  
		Last Modified: Tue, 28 Sep 2021 02:06:35 GMT  
		Size: 28.9 MB (28910670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3d70c7ae48d1f12dbe64e009353b0f4ae5906751228150eea7d8fa1071740f`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e560d9a265326647c6bf0ec61bd636c1fc32bb12a184dd1754edbf4b4ac050`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25dd92193301a114db15601dbcf4a5954c8d0de076495781fd6c9adaca0080f`  
		Last Modified: Tue, 28 Sep 2021 19:41:01 GMT  
		Size: 5.0 MB (5025194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f46212d749999bf7419078fc626db777dc61f530dc11ea65f671f6b0dfbbe9f`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fb1ae610eeb08a59770348cf7cf160343c05595fbf209e65f24f2b989ec1ea`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:45b303cbcd7118f178d37737f9f30191148f7ad78d93179a98a89776bd3e803a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31320662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f559c7bf328e87df04da1c8abbfc697650d7e87e733b9daf930625aa5e444b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:01 GMT
ADD file:129e2106788d883a456b145d9aff00c3003ee3480901a30318933b46961d31f3 in / 
# Thu, 30 Sep 2021 18:03:02 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 00:29:59 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 02 Oct 2021 00:30:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 00:30:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 02 Oct 2021 00:31:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 02 Oct 2021 00:31:04 GMT
VOLUME [/spiped]
# Sat, 02 Oct 2021 00:31:04 GMT
WORKDIR /spiped
# Sat, 02 Oct 2021 00:31:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 02 Oct 2021 00:31:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 Oct 2021 00:31:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aad43ac6bd46b2cab91485c8f1dac6a985df690af3e431e9e0b9fd57ad5ed423`  
		Last Modified: Thu, 30 Sep 2021 18:19:26 GMT  
		Size: 26.6 MB (26571924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9025f5203531aac8ffaef492d2ee0449ed32fed21089e855e4526e870a3051`  
		Last Modified: Sat, 02 Oct 2021 00:32:04 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd8234502cc14e79bc85bca5bd62b3a5bfe484f6f436fb1fab2f43cc3216076`  
		Last Modified: Sat, 02 Oct 2021 00:32:05 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271eba3c3594c73a3d96805306128d3b7c35aedfbdb04e9328a34626ae698932`  
		Last Modified: Sat, 02 Oct 2021 00:32:09 GMT  
		Size: 4.7 MB (4745481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8470c59880c9802734058e61ba7d95c956fa06d122d900711e16d8cc93e7698a`  
		Last Modified: Sat, 02 Oct 2021 00:32:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b19175f16b5b9e3387cd344389b01fdfbad041e6a4a0dbb53adb5d0e639cddf`  
		Last Modified: Sat, 02 Oct 2021 00:32:04 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b84b5dfa3a45a4a3247d03ea8e53134778a370366d4967ca1648de394559ff0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35323470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fbc4195f2bf091db9b87db926b163df95846c96bc02823cf4035017216ea876`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:43 GMT
ADD file:6472ab63529e688735f77634402740e08fdbd5bfa788c150915027993df7e8ec in / 
# Tue, 28 Sep 2021 01:40:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:51:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 15:51:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:51:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 15:52:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 15:52:08 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 15:52:08 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 15:52:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:52:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 15:52:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2f8871a8654eb1158cb626f8dc69992dba7e4bd8796fae6aa7cf967f951f5fe9`  
		Last Modified: Tue, 28 Sep 2021 01:48:25 GMT  
		Size: 30.1 MB (30055408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0bac6bf3efd88e9704f2f7b6a2c409b1df5ed4d12bf39715b3a2e61907fb1`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4facf47a49fb1694033154000aac13d2c30aafbf19e2c674bb4b27df60af7e2a`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8071a27573edf8bf22065560ce728d2de0654433685de5e18c1d26c7e8d1b66`  
		Last Modified: Tue, 28 Sep 2021 15:52:42 GMT  
		Size: 5.3 MB (5264803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeea85f6d4b4c5f24b4c9a75aface87afc9ef6b3c57fc95bc4c614dd809768`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309d496f924a836fede76deb85d262cb73b2ad70167020cab673d985568e24a9`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:af2b655879555e25f940b5bc902cb8ab828971b47b2238d6321f8df278c9137a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40267457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b96d038ad9160f431be6656aade8a3d2894947eadca6167bf2e19a3053fb6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:08 GMT
ADD file:8466bd8df052ea7fa26e49575ac95fd4934ddafdad54a9736ac2bd8e7fc6e735 in / 
# Tue, 28 Sep 2021 01:40:08 GMT
CMD ["bash"]
# Wed, 29 Sep 2021 01:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 29 Sep 2021 01:05:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 01:05:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 29 Sep 2021 01:06:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 29 Sep 2021 01:06:24 GMT
VOLUME [/spiped]
# Wed, 29 Sep 2021 01:06:24 GMT
WORKDIR /spiped
# Wed, 29 Sep 2021 01:06:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 29 Sep 2021 01:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 01:06:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e79fce1f6442094a82dc5f6b4d1aa352e04aae39bba821c9021f6da08b1cacaf`  
		Last Modified: Tue, 28 Sep 2021 01:49:07 GMT  
		Size: 32.4 MB (32380160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ea16e10fc5a5a0c4d62cf75b45ed7ad926cec71dc07cd1e46bfcec64a34e09`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7e9cd8372b882a460f62793c1c0d821b3a2d51e3777788be1dfef41055e4d3`  
		Last Modified: Wed, 29 Sep 2021 01:07:17 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200cd2275f388ecc2501c7ab0be9e5795e5aca50325dd9fcf253f1069890417a`  
		Last Modified: Wed, 29 Sep 2021 01:07:20 GMT  
		Size: 7.9 MB (7884038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a169c2e014ded4f64624fb6773ef8fb0c5f3e524fbe12a7f545b861f2bcf54ec`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c16912aa5431d3f809850fa2f91c9d56ea38463628134f5b3b55935f54f5dc`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:028091d21c83e82c61f42923008ed53b9b6e9b130901b2b130429ae0ff355b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3374098957b2318d62eead2991c25245a9a698f601f8546440c6c6e83fa9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 02:10:40 GMT
ADD file:43593ef3d79c9b74a92e318d44aacb578f6f8d835dd72665e057bbfe73df1a93 in / 
# Tue, 28 Sep 2021 02:10:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 02:48:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 02:50:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 02:50:03 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 02:50:03 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 02:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f46ea49e27fccc580c8910db39ba7f51ae208a8d24d46a33140afa92ea3d955`  
		Last Modified: Tue, 28 Sep 2021 02:20:45 GMT  
		Size: 29.6 MB (29627871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa45c48be690dce117b2c0dce958f833f4ce085161cd4c6c5b633016534a89ea`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf26a9aa3a964a21c42b56fd150ed69b7acd005c6629fb4623f95398a88425`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa171fdf362c6c554abf987cede2b8b25abb86afcde7578fea5c091f2cc1197d`  
		Last Modified: Tue, 28 Sep 2021 02:50:31 GMT  
		Size: 5.7 MB (5706116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e04cfec760a4c1a4925c2e96350ddc653e81d2bf92b7ffb7b9239f64aaae387`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b355a5bc54137c27f6b9f4b8e9e3caef346c4d0c43bf9d7496bfa69f266085e`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:b854abceecf263ecd3af9062c9bddf00c657ddc847f0a7beffa3d324806c6bfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41277029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9de0b22b9d88c7e7b941d2522f2954d1ff0b9cdfde5162978baa1f74ddd6d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Oct 2021 17:55:01 GMT
ADD file:f4b696a766a0d9a808c171a1d5db4f0877b0a784649d63bf461dfcf54b532239 in / 
# Mon, 04 Oct 2021 17:55:06 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 04:33:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 06 Oct 2021 04:33:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 04:33:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 06 Oct 2021 04:35:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 06 Oct 2021 04:35:21 GMT
VOLUME [/spiped]
# Wed, 06 Oct 2021 04:35:23 GMT
WORKDIR /spiped
# Wed, 06 Oct 2021 04:35:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 06 Oct 2021 04:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Oct 2021 04:35:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c3b7af0ed242d09d9fee2dfc48d4553d58ad90c5fb862ab58fb89e2d04c5b922`  
		Last Modified: Mon, 04 Oct 2021 18:07:32 GMT  
		Size: 35.3 MB (35272408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61743fc20904f8539cf80302250d866a1c6417663826735c20362034cef7501a`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da94c352893f839938e7606a77c9b6a0c747558c66e01483dd5ef4a69a07383`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534d0224ab6f6639dbd9d41948087e426816f7e37e5940c041d0b712088c87b3`  
		Last Modified: Wed, 06 Oct 2021 04:36:08 GMT  
		Size: 6.0 MB (6001359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb63df061584de7f6a9d4c754a21f5a3426f46c6704a41d99439d92f398a56`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8bfc7f69743b3fb3ffefa3ccfdcbc84807fe7c346480cc8313ee1af72d33c`  
		Last Modified: Wed, 06 Oct 2021 04:36:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:a81d059af60f158dfb49e3e03962db08aa2b6e40cbd80347d509d2026369a479
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5d72188d3d25ba7347f1a8ea21b01cf4a27445b632afe2b83bdd2f0f06c798`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:57 GMT
ADD file:2daa8824c30440336bc6ea1448af03234d491ad7c0d0cac917cae5eb54c315fc in / 
# Tue, 28 Sep 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:55:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 09:55:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:55:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 09:55:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 09:55:36 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 09:55:36 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 09:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 09:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 09:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e2938f4df931c46d7575f0b7bad5bc357277fc3e132b720e704ac7a4d1c9ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:01 GMT  
		Size: 29.7 MB (29650795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f460f8990cce2d9f2e25c13b42c5513a2129ef1a318b1097f6ff1186a5fbef71`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e214e0743e5982442db728a32fd9951aa1a7e6d14317d4cec1824fa8eeca957a`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4f812c2b3b5fbebd9e26191ed62c7eac5f1012927dfb8571c9f99a57d3db8`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 5.2 MB (5183853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972d8d742129ea070e9be63d7a5e8bc2840090dfe9ed23aa907c2508a1e9c3c9`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216f4500775537761e72820f3bb08e33e37ebf36fb33e73f0dca40bb88e2bf48`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
