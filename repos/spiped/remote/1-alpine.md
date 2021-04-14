## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:aefae8d25636a458e185a9bdf732f777ad466c60cedc0d9660e80d008d507bae
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
$ docker pull spiped@sha256:11ac8213b02d297409d7b7fcdd8b0a48a5be943ccb0afd600aca0acba5baf06f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c25b1de2b0d5ff0e8efabf3d3cc3abcc606adf1766270b1b437a961cc0b775`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:28:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:28:12 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:28:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:28:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:28:29 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:28:29 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:28:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:28:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:28:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86881cb39d8440a13e92432f2eebf9be90157813318580e5dfcfd3470cae225`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d85f5395d4deda0716a51b14ea11cabff7f6a33b0c4a4ff807e9d3e6e9b0a`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f474ecd48230c6ff5ddc935a076e4f4fe4dc842cd8bc8113839f2b35227a75b5`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 212.3 KB (212303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1525e8140e52c856b6afb278a1a36428f04cd948fd81c1361fc5575a8bcd998`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db43661c359dd89741c1ddd2a67f9902ceb333ea378289323d319e3df1b370b`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a8f094524aa54d65da82ac3129b78c13a1ff5cff473d26e7953a81a96c202ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6d756d9322008040c5902e261b8428a4eeadbaf973e8d48fa6a7d393a33176`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:50:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 03:51:01 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 03:51:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 03:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 03:51:35 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 03:51:36 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 03:51:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08375284756efffda8b0f8680579238d367b99e6e9774c5bc2948a223609b9`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9fba38f067baa6197b369a281149dd510a1a81b8a3271a50be709bca735db`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c433c405968ee69b45b2f652261c102453e750588274755fc5de0131b9918`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 202.3 KB (202276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6fc7889befc7a0ff491331bbd30d5efd63004b5ea0da1e12bb1b849fc697b8`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1e0e8f7257294af246022ecb31dac77d4340b0787771e6d6b552b99d97616`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:076dc896656b1b4cf2ded048821367d8960a5bdb96ddb4134bbdd3187442c04b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:782d764e7be26a956af06a4286ae1b384c9c368084344c3e2900945d2f76f4d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:09:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 13:09:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 13:09:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 13:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 13:10:24 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 13:10:25 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 13:10:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 13:10:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:10:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbca5e1d36141c0703b9cfbdde21f7aceb9796887027dcd1d7a2e934b1fc721`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fc7f276e5dab20703a18829c9730a7077537acc4f6b5216feb60a48d1cb7af`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83608b5141dc6e57fd5e8a524faa93d2bdd7816d6370cdb30f2b3e66fd48312`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 195.5 KB (195543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aea0254b4506405454f45907a949681726a965e3c091150209d6b37536036`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6556f29ebddbc9769ac742e20aa5fb223a3573b7f648aa3e248a4a71f3d7f251`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:a18a91f86b35437e8de014ede30b49f8afe472d01a834ef109b1d83125b17f10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b51f1caddfbebc660deb95c3ba908c2d59ea1915fe919d84af4688775bced6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:02:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:02:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:02:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:03:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:03:33 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:03:34 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:03:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:03:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:03:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdada7d83e7e80aaec853072a1598b0c0fc5272fc127acd150cc8dd6adadbdae`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88e6d0a2872d085185993ef77cc2e06a04ba200b3661ab389ce0108a0e5da41`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f834d24bb46d96feb30e4bf9137b76b2bec1a1678b72705fe99d890bd366c042`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 204.4 KB (204435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4d996ecb3b43082fd444b4ce2ff7632038162bb56e65886c1c16bf7cafd554`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3552f514ab3c2e5888b630036603538eef1cd5a75728c8e35af64dcd84115`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:654e6d7a720dfa4eb8a1d72df30b8f1e3122cba0850349dbcf246f63b93d4606
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405b48065d7865937665d693ec98c89b327b2a5a2922eda935887d7f7d7dd0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:51:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 07:51:35 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 07:51:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 07:51:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 07:51:55 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 07:51:56 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 07:51:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:51:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d549e288a1942f308e98bd63e9a88e4b46c1fd3bf5b46f2af22e3dfde82b0bc`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa5f33d7d1cc9f41cce3689eb319aaecec97ed85da04c9220d700f146c9e81`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e0f606528c3ab5b91505c21f3557ad732bc6d02d418edf4f63403cbe99a82`  
		Last Modified: Thu, 01 Apr 2021 07:52:32 GMT  
		Size: 223.3 KB (223283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c744159f7958c465d7ed11c8ffb2650a8a91e820729271b6c36beba8d56afae`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef80b8c05f87168506c2964fb0229d9fc6efd4fc2cc912e4b5abff7ee0a01f`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:94267d6b497d02f0f85f471c82b5b6bd0d149e12aaf359edacbbf01c941ea032
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436f12a351ea0c0ebd29c513beeb1e7e954fd1bffb8fc9aaeec88ab529a2bbca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:46:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 31 Mar 2021 19:47:04 GMT
RUN apk add --no-cache libssl1.1
# Wed, 31 Mar 2021 19:47:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:47:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 31 Mar 2021 19:47:41 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:47:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:47:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:47:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d452bef84dc63670e365215d08665984515db53171a73aac95e8fcb2e11ea8`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059bdf7279d42a1fcb055d84641ebef32bc778bca1c1d14239c4e8bd30476bd2`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96156d3c4691010d3da5a61f5368d99699eb901120314ef42751999506efe688`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 221.0 KB (220983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff346b44ef1d664ee7482a759efd0565ed8a4a05b594e069d232eee428364260`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84860a0e3e2e15db90c68d04ba424f8adfdeef75fc2e25b9719ecdd3fd36147d`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
