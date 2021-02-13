## `spiped:alpine`

```console
$ docker pull spiped@sha256:d151d981ca0ebab580c3ff2c4360baa2e99aca02d7c13f9a4e9fcd89425eb2f0
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
$ docker pull spiped@sha256:835d7b06f38b14f3497dfa8ef3a3387976759c1d4da641bee7b66ab2614327e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883c5cce06c38a0f7a19e769ba33df23b5104eae4f2f2529c4b6c7d2540dd71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:10:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:10:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:10:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:11:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:11:03 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:11:03 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:11:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:11:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:11:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ada2cbdd62e07ee40d2f05c48cbb06a172e5cde247cb27defa9146e342ee24`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0809851ee6dd7d72995918c73439754a4ff183f0aa0f142407150e9c75130e`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814bb6e0e86dd762b94f3a86fe4ea3dcac961064cb970ae9852a2389eab5bc72`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 212.3 KB (212296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a22052f5d37047c574696d71e90ee4fc969f40189329fc130b69fd39cd39ab`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db107fe5f9add27475633bd978bdbc7404ae29a7f594d3a2e5aaff7ac44b63db`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c27babd1d2aafca8bda58fedee7d3038c7b20fbf7b5e1eb870270268eed209c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2832841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d677780adfebbeebb133e4df636a0d26d64e0813b9fd46fedf2f1d9db0a3783d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 23:07:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 23:07:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 23:07:57 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 23:08:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 23:08:24 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 23:08:25 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 23:08:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 23:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 23:08:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef16c09cad69b4f5ffbad02c5d05e54a8776d0f589b5070292f555188352fc2`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd09edfda78fafd09511434ad81f68f3aaa910006a0cf43dbd8c9aeea23e2fa`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b616073d9c59a7d6763e8532e2e8bd4c592396a4250e30e030e29ef220db07`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 202.3 KB (202293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcdea289e6dfa0b452fe3805b1859196021df0753f5954e2728ee1947cf9828`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa80572babecc8c62f006bbc854c927644a0939f8982217861c889a29c084e7`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ae4d066b309a39b651ddcafcf7e0b5544d6698a4cfc4a7eb1c4e493356befb0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2627898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79097e2ce8ba1eaa302fbfdff3d7cd160ef52f71c4e89a7e4d3c097be5fa9c82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 22:39:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 22:39:48 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 22:39:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:40:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 22:40:17 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:40:17 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:40:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:40:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516139fc4bc5d3abbe484f41d65d96291d928c8313850bcfac5c409d91294e8e`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55705b9c11a25d31d806dae7cc70ba9979dbe2d872e5a1fa9675221a82cea552`  
		Last Modified: Fri, 12 Feb 2021 22:40:50 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19434ef650615c9f560946ec913d75335ea2c4da848dbe31002ba504051fe66`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 195.5 KB (195547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab2b83ef52894e4d6228617de9f67c33d742d2f237ee7fdfc38aeec8bf87f9a`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11720b6738d8b9681acab3a3423ae35fd9b3144467c23cb413deadffcfda6fd6`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:217ad97919e9aff3523891ff4cc50a783dd09a49976ae1f43a2cf615bd3167f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d125f8b9e25718ed14e33e37580e480d52edcf753f1cf917b1c4dd0ea4b9f358`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 01:49:09 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 01:49:12 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 01:49:12 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 01:49:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 01:49:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 01:49:43 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 01:49:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 01:49:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 01:49:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b73d7b095df7558c4913a1b56bc566a203d1705bceaf849063716da396aa3d`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a11963159741a5e3e3effd779670b8e3d7d46c46802b674c8c948528833d118`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984eda174ae2399fbfdebdc2ed85bb966ca11956df853e13be5060029f19f345`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 204.4 KB (204443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d588ba06f796ba5588dbba0b0cacec4a16b2a60183e3cdffacf7f0d27bf18`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e9caaa63d130b7c7a0ea6bcc1b2f984eae242f1ebea0d8bc7b5e487aea9a88`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:4960ec29bb9ef335500e75f0083cd0266fe301739478d22c7eac9fd71a2a0ab3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3049596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4479a0b49914c6027a4470086fafeec21241b4ec58e6a9b2c913d6bca2d22ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:59:25 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:59:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:59:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:59:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:59:50 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:59:50 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:59:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:59:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7723c1203294add77f79b9f3aafc10eda8572905ac503c7f5a0b2d49e488ed`  
		Last Modified: Sat, 13 Feb 2021 01:00:17 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce806478241c0f699afc38824da58e636c67df1e42986b00e0984769077c20`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bd8240d52bc7724188c29d5ef4610ea463be9b970b707886910547d6edbf85`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 223.3 KB (223257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209f92f3e8326cecdb9a9e84435c267898cd9258f7a6ab104632b2653a905c9`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40d0142f6f8ec7c14fc1fbc2ea71a8ccf3e8f67ba870450c9b5601ea7a710ca`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:33c381176119d7660214d2991cb4a2ccfa254db448220f4df615870f3a84fc66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50abb8300ea994b3e481699c0929ed73d9007f8f85432f87cc74afeda4045cf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:55:50 GMT
ADD file:b14fd5f3f7fcd16e2b4ec6932d3e9c07c7400c577cee5fdcb88b0795a70a7bfb in / 
# Thu, 28 Jan 2021 23:55:52 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 02:34:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 02:34:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 02:34:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 02:35:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 02:35:24 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 02:35:28 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 02:35:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 02:35:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 02:35:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b94a1d8d591af02f1b419642bee91066ecbb9c65099d6903deed310fd1c2ff`  
		Last Modified: Thu, 28 Jan 2021 23:56:32 GMT  
		Size: 2.8 MB (2812517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e118e9785a8eefb11035770ba3f016fd6735fff79024dddf90bd04b98150410`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c02326e8246063ab1916219ed81aa1f954ca993bc3590ef06d7b6748d815977`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc9abddce71df5b7d8a16936252ae190e82033deb046797cf5341fff77f026e`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 221.0 KB (220996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d1ec7b1f9be796457a3f27e5d1d7644cac7c122fd210e179931e04dbc0e7ad`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce293f6c247be36cea3048f53a9ad45fe1640112b6b234e232b79e69a9f1efae`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7b710fbed5a510700538e3437d8b3a418f829953d9b8fec0334ba9799219909c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2815889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fb1ee7014b5ab54030e234cfda6659e5d0d99d1c2033497d7f89f88cf5c2ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 03:11:30 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 03:11:31 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 03:11:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 03:11:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 03:11:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 03:11:42 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 03:11:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 03:11:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 03:11:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345d8435943aca39411423265dc836788d9ec232e833f7cbc90ab835db3625c1`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b2484becfe02ade48d7c733db97b58e1ce5dfdafe33927ad4a722949f1d565`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85179c983a9cffadd2d46f7ecf69991dc589c1dfb0379e6b34d372fb81f127e`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3949274cf2ec2bb3ad5931b5b9a119173d5ace06d37332a4d2c7a7d5f2199f91`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290cac537fab95725326ea6e10e2a1333216daaa916d670eac7fbf7005373593`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
