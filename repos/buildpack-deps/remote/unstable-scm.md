## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:344b5f3e55b978fbc29f3991fa3c9a893ba549f7f5476f982d3e92e8fb6b8a6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fcd3b293743077761c86cb0727ecc37367cc990a22a49680aee847893bdaae64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126213428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fafd28ad644ba9be4f74a5cdc1eb067dfc762badc0804578e2ce613f29d667b6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:46:20 GMT
ADD file:cac9ad9d988141c80929e8c31f4cb388618dac0bbc048d4c5e3b8029c85c576d in / 
# Thu, 22 Jul 2021 00:46:21 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:13:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:13:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:14:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:531fc43e70accbfd0e52721b79cfd564769d6f1b7e64a98e9f670327d4c4820e`  
		Last Modified: Thu, 22 Jul 2021 00:51:36 GMT  
		Size: 54.9 MB (54909299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f3334cfec756c2189b8a7cce5cd3ddf363b2acfc7b8a38f1ccf8cdbe4ef115`  
		Last Modified: Thu, 22 Jul 2021 01:21:10 GMT  
		Size: 5.2 MB (5171133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284c0769674315a1486ea9eee2a7dbe2a630850d90b8e445a2b8d7034528be1b`  
		Last Modified: Thu, 22 Jul 2021 01:21:10 GMT  
		Size: 10.9 MB (10872519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5845626ba0291c9852420419c76d5f8620b7801dc4b4420487f0119d42c59b6`  
		Last Modified: Thu, 22 Jul 2021 01:21:30 GMT  
		Size: 55.3 MB (55260477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fddc868bc480d8d9c096cedd279e44d56489226fe39c2a8ebd4b4128d19ffab8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121060861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35367af5334f37ce7b69443897d7ae4354af1708ba2d1483ff7a11ab46e7a8e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:51:25 GMT
ADD file:7b9b18b6a1a6deb81eb9bf8638d60de26198ba106aaa757dfb838b264fc90252 in / 
# Thu, 22 Jul 2021 00:51:26 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 02:07:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 02:08:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de879dbb26d0cc624c499f5907a14117d0f357e4e39699d3208c57d5091b537`  
		Last Modified: Thu, 22 Jul 2021 01:04:16 GMT  
		Size: 52.4 MB (52445986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef97169c47ca52a8e66f6ef70d0a4d9e5cfae0f8b72d1937ac646b3bdf48d8a`  
		Last Modified: Thu, 22 Jul 2021 02:24:13 GMT  
		Size: 5.1 MB (5075544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e445910f582e1f6da040a3bdd8886f00fcc077bf63486317b6de7c17cf3ba01`  
		Last Modified: Thu, 22 Jul 2021 02:24:15 GMT  
		Size: 10.6 MB (10571845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d89631dabbc12408ce2f82d183513c97cde3d9b7ed0f3d4863be9777cbc50ed`  
		Last Modified: Thu, 22 Jul 2021 02:25:07 GMT  
		Size: 53.0 MB (52967486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e5b3206697bb0c0eb1cf9cfc0de827c58df2c947994bde46d403f1ced6336e05
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116192536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40a002dc841a1b3a25165d14c2b6b12e95bdf8beac7616c7a3316e35a527f945`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:05:12 GMT
ADD file:dc3a5129f00ffe49d5f2b5c7472bb0e89235fc02cd3f1cc7d27243e371d4a8e9 in / 
# Thu, 22 Jul 2021 02:05:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:18:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:18:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:19:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d81caeed2081307865201ac11c62494bbd309b5efe940cf9cae7a6739c8ca2a0`  
		Last Modified: Thu, 22 Jul 2021 02:18:16 GMT  
		Size: 50.1 MB (50111961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab786a921ccb7c1afe30eca6993da354114a957337287d819030ab934e693711`  
		Last Modified: Thu, 22 Jul 2021 04:38:30 GMT  
		Size: 4.9 MB (4936974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d08ba7697666bbe33ab34e16c74f6a0e1e670f45c2a33f9f3205862bd88c74`  
		Last Modified: Thu, 22 Jul 2021 04:38:31 GMT  
		Size: 10.2 MB (10217393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d317888fa778790ee95eafb5aed1fdd97c57a5c4c046dca2a88c869fd8f2eb61`  
		Last Modified: Thu, 22 Jul 2021 04:39:19 GMT  
		Size: 50.9 MB (50926208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37bee1487624fd84c180d6b30ee44482d1ae1d363ae4312e0ae72e29742d84e8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125073913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3efdbbeaeb82295134826aa702e6298a62dd1936103e9b1f058056bf4a1721af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:32 GMT
ADD file:2eb550b4dc61105505c60437af91d7300fc5596834bfce84a75b260663bf4f42 in / 
# Tue, 17 Aug 2021 01:47:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:55:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:55:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:55:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c8e1604d5b38112a190afe29ac6b4d1c501651ae9e68b6eaa49788ae64f145d`  
		Last Modified: Tue, 17 Aug 2021 01:56:14 GMT  
		Size: 53.6 MB (53625965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4b3d12f8e0cac2ab78286575b8f56d2cadedcafd68908cc60821856f5e360`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 5.2 MB (5160051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb41ce34a000fbba6dafcb340db9d0b7f64a8efd27ff966f77978ddd2c567439`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 10.9 MB (10873429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7ff3790681e7d2217b96a8b89bdf6b99ab28fa3c7c0da0c88118fa977a7ce9`  
		Last Modified: Tue, 17 Aug 2021 08:03:58 GMT  
		Size: 55.4 MB (55414468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:04e0650bc727dd18f73c095ef5f35e238acfdbc963764c86f55dbd57a2817916
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129204520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3ac461708875960f1d5e7c484c1b60c5867b04bbdbb89494195e2999ae5c74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:42 GMT
ADD file:8d9eb4b2afc4eb0058f4080c5f0eedf0ddef323f1cc5a0403658254d191f117e in / 
# Tue, 17 Aug 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:02:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:79e62a40ce7bfbbe436e33c1da1c5661386b9674fe81402fdbfbb42a5b84998b`  
		Last Modified: Tue, 17 Aug 2021 01:52:55 GMT  
		Size: 56.0 MB (55967475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3391f9add930caab1f7ad8d326db740aab914960a3522b2baea8f34b06d23`  
		Last Modified: Tue, 17 Aug 2021 02:11:30 GMT  
		Size: 5.3 MB (5301763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c1c03bbd7c2f8c23dd8b5a8bae89de98d00fe400f6f7c89140aed7a78c6aa7`  
		Last Modified: Tue, 17 Aug 2021 02:11:31 GMT  
		Size: 11.3 MB (11250490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71047ae47f0ad2d0279c1731200ffbae15c68839f662197eb53927e89f4a346a`  
		Last Modified: Tue, 17 Aug 2021 02:11:56 GMT  
		Size: 56.7 MB (56684792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:01dbe5850925eb9009c48ba896d743425d9eb54e88f88144a71fc452c7c68626
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123227419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107fda626c0b3057d97ce6567e702283ed54496419012afefbb061a4150505ee`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:10:12 GMT
ADD file:21823f99ac9631853baf61992ae48f9aaefd9aa14689bdad76945cbe790d4b23 in / 
# Thu, 22 Jul 2021 00:10:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:46:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 00:47:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 00:48:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7674bbd759fec6741d7d94cfebb5e0cf54c599cb2a824313eb96b1d6622a44b`  
		Last Modified: Thu, 22 Jul 2021 00:16:59 GMT  
		Size: 53.2 MB (53162150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bbf92e62547174ba9022d0c0fe12fa84126289620f8148cf33269681b8273c`  
		Last Modified: Thu, 22 Jul 2021 00:57:29 GMT  
		Size: 5.1 MB (5130754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2614779dff3229eb62dc8a974d88a9bf60cfd085721871ad71d642e0517eb35`  
		Last Modified: Thu, 22 Jul 2021 00:57:31 GMT  
		Size: 10.9 MB (10873093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100254d07ca9795fcf9cb6c9e7d187591a97a9ac79c2b0c7c4351c8e7c1f30a8`  
		Last Modified: Thu, 22 Jul 2021 00:58:21 GMT  
		Size: 54.1 MB (54061422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3f8769eee4695a61ad3940a4c1a1333f1a953ad60dd3dc77428aa8a3e565cc43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135526176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b610da6bb9e2031c67db7105a6676fd68e0690fc594a692cafd6625ad3b44a1e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:33 GMT
ADD file:d5172916465206276bfc66e1d963768fd3cda811ba961e86fdbc4b49f0a72dfc in / 
# Thu, 22 Jul 2021 00:19:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:19:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:20:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bb31d3e4dd3826fb7298bcca3375efce01b08c74be37a5494cb4eaccd247d8e9`  
		Last Modified: Thu, 22 Jul 2021 00:28:17 GMT  
		Size: 58.8 MB (58810717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6ede8e70912b2a939d88a27d547a381f612b6c792d57e726d55e899c3866ec`  
		Last Modified: Thu, 22 Jul 2021 05:18:34 GMT  
		Size: 5.4 MB (5421821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b90280541d7eb6e7e1d27889a4b6e4dc571eb851a0b49f6da40e06522687e`  
		Last Modified: Thu, 22 Jul 2021 05:18:32 GMT  
		Size: 11.6 MB (11626277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96af94f2c600d7f45682dfda0d3faa954448e1b45034e2ccc980c66372c03c36`  
		Last Modified: Thu, 22 Jul 2021 05:19:52 GMT  
		Size: 59.7 MB (59667361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8105fd441cbd36f7bde58e34b24e9329d34e31d2c7e2592edbd60d5ac0d77efd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117103758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27c68b1a73365a21c15885cd64ba01cc9fbb3f9160c6787ce5b37cdaa3cb6a9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:57 GMT
ADD file:17c3a69ac6b2ac905f0d9d5d8d828215848c91b6aca208c63e3c8c6c3c28ac20 in / 
# Tue, 17 Aug 2021 01:45:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:29:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:33:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03abe71e39e08cd630ff168b11929dc5c3c5111cfb3d81f5a8183f7ba7162fab`  
		Last Modified: Tue, 17 Aug 2021 02:01:48 GMT  
		Size: 50.4 MB (50437771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e3ddf2aa723d9dc92fc071b3cc373219cd68de4072a024dc13965f2156705`  
		Last Modified: Tue, 17 Aug 2021 03:07:39 GMT  
		Size: 5.0 MB (4984859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbcb287940d650490755774d53a8edf26fba9558538160b4f649b66979ee4d`  
		Last Modified: Tue, 17 Aug 2021 03:07:43 GMT  
		Size: 10.3 MB (10293904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecda3ed528238bab9bf59ea2bc04887f931df81d6afd6768a21f6cb99a711637`  
		Last Modified: Tue, 17 Aug 2021 03:09:51 GMT  
		Size: 51.4 MB (51387224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:508193ae57b397427a2d0c356c071845bd3d17f174589d82e138df64ec7e90bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123868303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7f4f7bd222e4b52b7b76ccd1407623917c762cf5daa6d1d6646c1c65968e00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:51:06 GMT
ADD file:ab809bd14c40234cf29151f2485ed39a9fa31f67c202abe6bf8546f5899aa52f in / 
# Tue, 17 Aug 2021 01:51:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:37:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6758b3369d7c595105d273788911a60f3cbd8b26d39dea406c75de4d1da4a084`  
		Last Modified: Tue, 17 Aug 2021 01:59:02 GMT  
		Size: 53.2 MB (53226590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee5f5767e372ec2c62434ed4325aa1b14846b20d736bdb81e1861163803d98`  
		Last Modified: Tue, 17 Aug 2021 07:45:09 GMT  
		Size: 5.2 MB (5152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1daed3fa6142f9fe36fd70a1e631c71aa839f077885d60cb4e7fb21210dacc`  
		Last Modified: Tue, 17 Aug 2021 07:45:10 GMT  
		Size: 10.8 MB (10763976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52078ebb293da4fc08dd7b04c3124715e75d72e8d33e91bcdaf326bcad28bdb`  
		Last Modified: Tue, 17 Aug 2021 07:45:26 GMT  
		Size: 54.7 MB (54724881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
