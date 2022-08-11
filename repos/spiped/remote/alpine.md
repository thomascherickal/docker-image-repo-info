## `spiped:alpine`

```console
$ docker pull spiped@sha256:acddecb1628480a3371f5c7990076e0d894c6a9a2e7612d844e800178fabe8ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:66b3d848f73df6532c49bb456c441a37691db14797c1288fa9cd5deb9cf9bdb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb8fdfbde39b2b89abb4cdfac48560f245fff78fc822e3daac086fd5b29f78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:25:06 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:25:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:25:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:25:17 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:25:17 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:25:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:25:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210040c27162008830a83da8ed96f452757ffa50050398230f525b2f22a4541a`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b54e70388210c7ffd8a9fbb864ca9f878f8ad3dc1613e4b96b107919baadc`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff19a9777e30476c0a48eab4bc4817e9a96226faf7b42870225d69a37ba8`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 221.2 KB (221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f71a1b577cfb700f72058dad655d1ec9161da01b7fe6e8bb2b2461d1ddbbe`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2f8d0b8416d1c553517142cd373249cbbdc3a03229d96604cd32b318a1195`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9bf39d60020a139fa461ebb060df6df01d5164425285c6bfc1b3113ef2242277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2829328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88197140375c26dcc5aa5dad079e8343608e24c8a03e91eb5d2fb13c9e09deec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:37:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 00:37:39 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 00:37:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 00:37:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 00:37:47 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 00:37:47 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 00:37:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 00:37:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:37:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8a3e1b897eaae3127b4c0c6bf167dc3d7740bbf9596a97a994f1249716538`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa63959f901bfbea0a7da0112a6c04fe32edaaf453bc28bc784d942ef8a1c01`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53413b98987994a206c07b7c3ba39980d1dd0149f4a1be509beab0c15b75da`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 205.9 KB (205888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe12872e965332f5c42d1844aa3dfdbae46eda912838801110e130b89cc181ca`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a33b8651215087c0b9c9d0edc3a3fb9e0d18f0eaf36a0c0bfcddce94e338d57`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:0e746939643dcaba40d0c1f15f4d142129555ff4d3a187e755c3643cb387bca1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2621321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5a28036aaca6f3accc02f7ab66d26c0d7ef2c544316b0df54081730f89391e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Wed, 03 Aug 2022 21:57:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 Aug 2022 21:57:09 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 Aug 2022 21:57:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 21:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 Aug 2022 21:57:17 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 21:57:17 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 21:57:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 21:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 21:57:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a223ea05945b5c5ea98e31d53b7924f548e24abe646453181a3b73f940a52de`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868bbc51d36bab84123a304360d9b4bc7db9f0714c2281b34b7585ff494ab1c8`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18353dabcadb1dc2dc0b669eeff1d9dd8d42a815bd9f860e8ff08c8f2191131f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 199.5 KB (199542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330712fbce762a1e0c7e7bcf9c36a39c454fa780a6901be6761dd588dc043f5f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221966fcc255ad5deb2fa5ce1fc0b504eff307dc6e7aaebe7db90698290052eb`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d9f2978a4900b825028e1c399cd7d0638f75f91f2400f6c6bc1d83d6274fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031699f5a5efac86682c564a2c655c7eab52ce5aa91a856923d2032ea0517c52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:09:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 06:09:42 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 06:09:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 06:09:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 06:09:55 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 06:09:56 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 06:09:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 06:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:09:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf9d3ec407b6270ec79bb3c0552c48d0afd7888773c72f1b25bfc396d4c3eb7`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f1183a0c8143435d389abc100d22d7289e4a81f966ca3b9d8301cfb01947b2`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc3813fe4a6ffebb8bdde4bd9005230c2935072094662e52a3a81cc9a9c3fa`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 214.3 KB (214262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3f496ad70b8f2f8ea93c54500ad75fb9fa4b72d7868ae964cce858765988a4`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46086b9ffd0c9eed5aadecf28229d0ab4532a26add5be2f474ced21cf4f25f7e`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:ee4833bbef16308d250de2dac9ad7a6019a6f2e42880ed8eb3dfd4fcecc4ced4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c145e337e061db2f783bf06d6d6b2f1e63cf3e7dedb8ada91bc1744b707620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:02:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 00:02:18 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 00:02:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 00:02:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 00:02:31 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 00:02:32 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 00:02:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:02:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:02:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072149e09853327c1921fc351fbf7a93e1056edfefc5daa66cbdc6e48843cd13`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34965b4906426a2b44e36dc3fd455d5da36569c3a0c3de199beecfc03c85244c`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddeae6e8a846e3df57fb016e864191c85342272b8c766aea5b9cd0e001b0332`  
		Last Modified: Wed, 10 Aug 2022 00:03:05 GMT  
		Size: 231.3 KB (231325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463f4e96eadc8d28add083b4c188fcdde9cecb3831b8c5427343441c383e1136`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3648573cf3f78bda63b9ea60198dd66926dda5cbd250025fbf6c5c0f08bbbcb4`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d67f02f9e68884fbd145362c4f490cdfb403437bcf89d1135ad1a15c92052a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd901b20c0f04f13ac388776797050b3e6a48903ceeccca414c16f53e1c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:55:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:55:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:55:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:55:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:55:34 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:55:35 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8832ea95a37bc42923d861cfefd27ec973fed3564060fce137b8d54f75e02`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab0760cebdd26f5d818b164fe30701e72c6ec6c6c6b97b100ed16bc24fcf653`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdb874eec093d50ac091467e93cb88955a1ee87db0d0dd84cc6344ad829323`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 220.3 KB (220255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a349e85c23948cd849a1a373c684ee566e0544af2297f9904d664dbb41dc8a6`  
		Last Modified: Wed, 10 Aug 2022 02:56:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd274005021e79dbc526fb1fd7ad0d420d2e5c10abf68e3c7ae46021ae45cbf`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:936312a4e0595fc377ed5e910f12d52cfc4fae63a6190fe388481f204758a480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa6705ab1cc71e7aa223e1b9c9ba81f85eacacdba00737aa34a7014d8d94163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:46:33 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 05:46:34 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 05:46:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 05:46:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 05:46:39 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 05:46:39 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 05:46:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 05:46:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:46:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997054cff6af24fce535516fc4358eabc7dace5f52f427e6a19340c04f6adfe`  
		Last Modified: Wed, 10 Aug 2022 05:47:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78da263b8c9f381935ae64289597db6f2e0d7e77fa388ce819ba7afecd17ef1`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acce323c9898120275bb4b4763b7a8971f71720bf7cafb55201dc313247560c`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 208.4 KB (208429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b550d52792a92d7c50d7e5102763598d59d41f0c34d5bd928fbd55e16de8f8`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130443af95b4efa2ff2d4d039066967531a4e10357d515888d55082f26340a52`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
