## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:8b9d9ce8050c9b913a1437c988932ffeedc646d642c8a04889268ad1e560f003
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:eee0ff84af2314f8c0e10b03aedbe55530ef370f28887bd2ead845a97535d3d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131302877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3efd04ee9eba61ddea4392a056efad62aab3c7f0dca4ff31813810e0dfe3a1fd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:06 GMT
ADD file:cbb7762965e1100a173296573d49c70a5e56d5318572ae1b037854e45a3c81df in / 
# Wed, 11 Jan 2023 02:34:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:02:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 03:02:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:248f02a8d7fb9e98e764c3ef93b9922d99e6b305be444aa17bace4ac12a55508`  
		Last Modified: Wed, 11 Jan 2023 02:38:08 GMT  
		Size: 50.1 MB (50106530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f922aacf80e8d4f20a47bafd73d9b7865d169f43635eaabc15b5e25eeb6057`  
		Last Modified: Wed, 11 Jan 2023 03:11:00 GMT  
		Size: 9.0 MB (9032940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b287e34dfb83462bf58f6751173d64481c601980dc53909c7d198527f44e88`  
		Last Modified: Wed, 11 Jan 2023 03:11:00 GMT  
		Size: 11.4 MB (11352159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8760a729a20f23e47ce926dd7b082265854f8834280377051a238bfaf725e51e`  
		Last Modified: Wed, 11 Jan 2023 03:11:17 GMT  
		Size: 60.8 MB (60811248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a5c524e775e51d05902c4679ef86390dd0988ed44c29d9790007aab293dc9e06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (126957199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e74fd125525846baafa9d29e9273c8483a208bc20c8deb028249c1facf2d6b6b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 01:54:53 GMT
ADD file:5d45a8dd4f8495c2419fecb2fbe1375bee8fdd9c4ecd8482c9d93073ceaf0eb1 in / 
# Wed, 11 Jan 2023 01:54:53 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:22:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 02:22:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 02:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c18e65c95b83dd67fa3b288d25c836639aed042685d4b545ff41efbf3046505d`  
		Last Modified: Wed, 11 Jan 2023 01:59:27 GMT  
		Size: 49.1 MB (49082333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2627725f148bd514b2afb35f5ee907f5f061ac39a52d6f89b1cf91b8a80f46e8`  
		Last Modified: Wed, 11 Jan 2023 02:31:26 GMT  
		Size: 8.5 MB (8484837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81a8997d0bb710a3d95fc77245088619618e15dc87431056622547133566c3`  
		Last Modified: Wed, 11 Jan 2023 02:31:27 GMT  
		Size: 11.0 MB (11000015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5949aacd5a13ab1919fbce97d65475583ac45fdc71c7ecee03b091614645ce8e`  
		Last Modified: Wed, 11 Jan 2023 02:31:49 GMT  
		Size: 58.4 MB (58390014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3d03fc7843397ab18ad38dd7d946b7e08cb7abea0da9fd8e157b826a3d5316c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118792618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55fd5d55fbff40c5913710d8da06c7c471a71483a12ed1e9e6c76b039218a37e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:57:40 GMT
ADD file:3a39343b0809f063616f72499663466e4a509b48e03fab9262c152a211f015f7 in / 
# Wed, 21 Dec 2022 01:57:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:25:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:26:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d2b0b92caaf35a430a2b891b3ae1c59a6cf60477263bd8e7a30cda427435d63`  
		Last Modified: Wed, 21 Dec 2022 02:03:55 GMT  
		Size: 47.1 MB (47101260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a36589bec34c9187227f581132ae596646abfc864ef9c4f049dcc7cb80d9e3`  
		Last Modified: Wed, 21 Dec 2022 02:36:46 GMT  
		Size: 8.1 MB (8119430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa4da363e919b9e1ffa0593e59ab1b23caa6d60c84b20ebfea4db0863532e5c`  
		Last Modified: Wed, 21 Dec 2022 02:36:47 GMT  
		Size: 10.6 MB (10646191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca23736de3322232278a50330b166e2dc3a96e13bc603c0a868f7c6ed03aed8`  
		Last Modified: Wed, 21 Dec 2022 02:37:07 GMT  
		Size: 52.9 MB (52925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:48d2f90b64d1658caf2a66ba9e1fc9de751cc5cc5e4f2a15b27a65bad43d0fc1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127642164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a6c47f77cc8fd587023c5ca50627c75e6860b80f21e4c39ea861ac64527471d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:25 GMT
ADD file:b83d427ad5bc07aecb363a59c19809d66f1425c1d8df7a4d66eb56624cf5fcf3 in / 
# Wed, 21 Dec 2022 01:39:26 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:03:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:03:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:04:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be520eae96ff7c486efeba591ba872089e3b618ce226d23bf2b72f07277fb6fc`  
		Last Modified: Wed, 21 Dec 2022 01:42:15 GMT  
		Size: 50.4 MB (50372842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fd22e8d17dba55cc72a876a3a9244c7b617edbf94a17fdaad2f9d803c02d5f`  
		Last Modified: Wed, 21 Dec 2022 02:11:45 GMT  
		Size: 8.8 MB (8849270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7950c3893d7d3fd9cc5fb052ba3abdcdc532147811125fdba6efec5d9b4efee5`  
		Last Modified: Wed, 21 Dec 2022 02:11:45 GMT  
		Size: 11.3 MB (11325894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d0bb157e7432bcc4ced269bd85ce3c558f9fcefaac7844b601556fd5cffe72`  
		Last Modified: Wed, 21 Dec 2022 02:12:00 GMT  
		Size: 57.1 MB (57094158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d91b395a265a5751195a262b60e5f714a69638cb2c6167c8f11f77450db73c89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130759663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c1dd53344fffaf3655d01bc02cbabe2222312cd73fe5872f96b83af7aa6b2be`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:38:43 GMT
ADD file:f11f9a6e73a1ba42c97eb037cc53f119df6d6b050eaeb10df2ae716f4eabd8bf in / 
# Wed, 21 Dec 2022 01:38:44 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 09:50:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 09:51:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bce8ae6c08a69b30b85b1e939b782fc4dee31791e21ed3abbf56d1ec1dde0381`  
		Last Modified: Wed, 21 Dec 2022 01:43:40 GMT  
		Size: 51.4 MB (51363529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d633e3250ed10016905229f6d67f3386ceb15eb9d1bc3deb88c518444ced27`  
		Last Modified: Wed, 21 Dec 2022 09:59:17 GMT  
		Size: 9.2 MB (9194506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65f66728bfc6f4d6de6d54692bc94e1c8972c2fb1d47052d38b89b8d33481a2`  
		Last Modified: Wed, 21 Dec 2022 09:59:17 GMT  
		Size: 11.6 MB (11561149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883b0fff1e223e986f26eda6c09aecaf9bf292dbb243e2d42df8aa52d520818a`  
		Last Modified: Wed, 21 Dec 2022 09:59:35 GMT  
		Size: 58.6 MB (58640479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:f9d67cfec18b52e7d645b1494f051e0a25f8c53713d887241842c73a8ec53625
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125860374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0946248af56fc47f86c94919336a85c6f5eb1a71e4622a17526d0da4fba2408`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:08:43 GMT
ADD file:b2458569ae73892acee2eab6d63bd5fac233b8f2939355fc7605c8906c1bbd30 in / 
# Wed, 21 Dec 2022 01:08:49 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 23:43:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 23:43:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 23:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63a99937a40bd4c10c6b0d4be0826a18d963fdd5ca9c794853e98ca819d68691`  
		Last Modified: Wed, 21 Dec 2022 01:16:43 GMT  
		Size: 50.3 MB (50336746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b476ebedac13b0ac645f8735e4d8a8321d9d6dab455dfb083f909d760d43de10`  
		Last Modified: Thu, 22 Dec 2022 00:12:05 GMT  
		Size: 8.4 MB (8382953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d4410a7d6810d0cf4de163bed3aa485a268050cff9cdd1b1d2690d3843d528`  
		Last Modified: Thu, 22 Dec 2022 00:12:05 GMT  
		Size: 11.1 MB (11118852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f052e411ea81eab6516c87a7e7d7d322c9ad6bac847ad1805b31941908d5f2`  
		Last Modified: Thu, 22 Dec 2022 00:12:53 GMT  
		Size: 56.0 MB (56021823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e4cd5249326fe2a87856df8e62965817a2b3fb7175180e4bbfef8ddf42832960
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138101239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0321b17f02c225b1e5ea25a41ea04144a4c1f5e9e851aff96c8bd0c516d34a00`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:16:40 GMT
ADD file:ddf53eeecd4e99f9ac6dd446b84eed33212dae1b2a9476907b99dc988c316e5e in / 
# Wed, 21 Dec 2022 01:16:44 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:49:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 04:50:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a50dadcc8beda7926088df1652aba274c8cf1817cd6956a9342f3b25db470e6`  
		Last Modified: Wed, 21 Dec 2022 01:21:57 GMT  
		Size: 54.4 MB (54373822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9716abced382581cab26adfab0007029a5bb1dda4112dbb4ba74c5cfc7f06ad`  
		Last Modified: Wed, 21 Dec 2022 05:04:22 GMT  
		Size: 9.6 MB (9596165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbde01939e5586504281eded1dd73c49a0b03f58c2cd890cc840b8267967f3`  
		Last Modified: Wed, 21 Dec 2022 05:04:22 GMT  
		Size: 12.1 MB (12128890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eadf6b46d5863b425edea1179a79cfa53aa4e33b4f2e8df8cfb2127727d75f3`  
		Last Modified: Wed, 21 Dec 2022 05:04:50 GMT  
		Size: 62.0 MB (62002362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:22fd62c29c4a6328f91319b7e1531e71be8898c12567e2129a4e3e349d0f6b7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128118870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6a1eae851615ed9b456aa06e8f8a7be4e4eb5e7bbef1a1cefca1adb54d4036`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:21:33 GMT
ADD file:1ba7db44596ea26688f29eb4d23da5507a0d71de49facb85ffddbea04928e97b in / 
# Wed, 11 Jan 2023 02:21:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:46:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 02:46:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 02:47:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc45c63d26bf6e7676d21861c5543952964197c106b2cd255789a8aa3734c0de`  
		Last Modified: Wed, 11 Jan 2023 02:26:06 GMT  
		Size: 48.5 MB (48490381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b941bcdefcde17ded465ffd68a2ebb6d2c7db9642b4c6e5df1e8f72eb96d886`  
		Last Modified: Wed, 11 Jan 2023 02:55:46 GMT  
		Size: 8.7 MB (8665948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccacc30d10abfa911c54fe2ac56c3afb46ad1b934aed0943fb3ef1ff2b4fe619`  
		Last Modified: Wed, 11 Jan 2023 02:55:46 GMT  
		Size: 11.2 MB (11215678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6339bd7d1b55d1a706abd8cfd85402705ea34b3ae5b1d868a704008e244fc`  
		Last Modified: Wed, 11 Jan 2023 02:56:01 GMT  
		Size: 59.7 MB (59746863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
