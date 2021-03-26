## `spiped:alpine`

```console
$ docker pull spiped@sha256:19684fbf0023be921667a91a92d2cf6e979393817c9e69f7062aa2bb5bd5d5e1
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
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:da8bf89069f02c44e64a52cd3c311da57833ba52c0dfd401bf5b400bcba42fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6928a48d8b494975b09a73ff31d4ec85bbf1a70eb5240a267316a1495d85c91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:26:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 10:26:10 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 10:26:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 10:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 10:26:43 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 10:26:44 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 10:26:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:26:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05731027fa533b4ddfd5253b33af7f2e6329040d608478a1cf595d3594e504fd`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c330cdff7f6294e87be781c7a86aac39a7e7d2431c24def9e8af9476e2c7da`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7422b39d0efd63a811763e22eb91fcaa0ea348b8a13c6a2afd70562f5cb9bb89`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641ca636eaa042a42ed82a4494fe4030af9725300ffdc103faa9e12ce1a3816a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f1740d604bc2886348af7061a47d9a4343057827419e05f23191d5b911a3a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:6d4e4fe6948e5a7992c124e61fa437b6e0413a5bb3401654fb248eb3cb12d114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c19db803961bd8dcd8229779fef2771123c1e74079d8339d813fcec140a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:35:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 11:35:31 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 11:35:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 11:35:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 11:35:53 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 11:35:53 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 11:35:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:35:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:35:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e02a3b4bec768000b32f6cd554e24e6c8494cbd013299b945dfba9976453`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be889af3bc0980bb5b61ae0b456dbd90907f154b74b796a26046e96f70c4f6`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a408cdd7892cb9e528cde840b9bf4c2457e6b9540f7b3eeba4b75bb22d5729`  
		Last Modified: Fri, 26 Mar 2021 11:36:26 GMT  
		Size: 223.3 KB (223278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb962d5a258d79b6a952f2eb3e3c6f8e4497529c9b722d855f051a120a68c0`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c91539d601c2ba091818f38b8b0b17362626aca4e30ca053825d5b4920cbe`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:90360f53f918820e5f6a844dee0754fa75b275607dbe5c71293fd0e7af7797c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f4df11bdbbf450f4e6fbf2b9bd4b57d9432205d415896d1ec7179a79658764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:46:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 05:47:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 05:47:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 05:47:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 05:47:57 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 05:48:02 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 05:48:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 05:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:48:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ade0bad869d6db8a4e76203a6dfe3818480c33c407956be758da40b7da8e87`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6878fc6b1c7c9ff2cb9cd6603daa1608abf9847d920dbc2a975313b81d54d09`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e8e86fc5762fedfcc865b9618a77f7c27214bf2068e2bdb0f7151d8964030`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 221.0 KB (220985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956adc5bd10550d52ee7f60d1d249008d2ca8b414e697b229923777c89fffae`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dac4482b42db1364dec4448343ae95036dd4f7b02440507ae3e40da8dc0d43`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c1f0c63244642a743f32f026370285292f3dae250a308e6364fc3de8ab05effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d526ff26ded3a191cd728d6ee4458ac19061aadfef60a349e786aab31ba72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:56:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 25 Mar 2021 23:56:54 GMT
RUN apk add --no-cache libssl1.1
# Thu, 25 Mar 2021 23:56:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 25 Mar 2021 23:57:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 25 Mar 2021 23:57:06 GMT
VOLUME [/spiped]
# Thu, 25 Mar 2021 23:57:06 GMT
WORKDIR /spiped
# Thu, 25 Mar 2021 23:57:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:57:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d211148772ab04d0ac7d6a254412fe1f42c1e2e7015b60b873a95da6f14a452`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9963e2f655c56703f1a6c0ddfe5ddd34f7f2725e4b4dadfe50a44dccb3fabbef`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd16cb6da0cae4c5ecfe500cf635456f5c13193987be355c858e78a57bf1150`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463e1d0912abda7c19a7c110819c8a1b49e67d57f21ab80715f4a0ee1664927a`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48866150c20dea94d44784f072b65bdf6f2292cc61d11de364bbe2d47f21ecce`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
