## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:3a56b02855ea32ed50860a39738470403c9782ee1eb175b6e986ac4f46e27937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:98acd7bd5bf8de17ac0e85dd773f23884e9941ac6b5198decea43299f045fce2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37627713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f76a056d18857c8e521869ef29d268171c560d5195e8985b2b6847dd0e9500`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:11:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:12:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41583b66ca848f858206ad13d445c445a42b861cb9680ee051e0044d4009451a`  
		Last Modified: Tue, 07 Jun 2022 02:25:52 GMT  
		Size: 3.7 MB (3694680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb932530756d3b13de14424901f964ff45c1fa6c30ee51a67696e49cce8fd03`  
		Last Modified: Tue, 07 Jun 2022 02:25:52 GMT  
		Size: 3.6 MB (3552743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e91c66eaa9a9c8566baf7d517458b3e2a78274a4dcfb96da63d311c6f5cdce01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34108232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d867f61c95918e9dea55c8d00f9125df5dc4316ac6b5e9f52be689d36698f96`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:09 GMT
ADD file:98b792cccd674eb149eee0fddc60ebe9484757384fe35630fc361ecfc28f9e42 in / 
# Fri, 29 Apr 2022 22:59:09 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:31:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:31:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2a09877f6132d465ce4f615f0c5f4bb1dc0e311ce406712beced416d3257e69c`  
		Last Modified: Fri, 29 Apr 2022 23:03:29 GMT  
		Size: 26.9 MB (26920477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4af27a84ac863174a3e2c6171bf9613a188ce8b1b037ddbc4f0fedd477c695`  
		Last Modified: Fri, 29 Apr 2022 23:49:02 GMT  
		Size: 3.4 MB (3444024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a5bb5b4bcc573ab723569d88c431ee0657394bc927acb599d0f698782c366c`  
		Last Modified: Fri, 29 Apr 2022 23:49:01 GMT  
		Size: 3.7 MB (3743731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c9eb8183ec09ff77a30dbec0c80ba89eae5d12e36ed14ddb5cbeee0e45844325
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36021466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dc3395b96a16fbe246bbdc99d97930378cb2abbaebea114b4732ed023380198`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:24 GMT
ADD file:d1932d13ea73e26ad39647db09c23895cf0644ba34851cb87e777778d59b6730 in / 
# Tue, 07 Jun 2022 01:25:24 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:46:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:46:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:166e0294b8df947d819744f38e21281ed5f29a2a3b19d191deee511cbfb0e473`  
		Last Modified: Tue, 07 Jun 2022 01:27:26 GMT  
		Size: 29.0 MB (29018061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957087bdfdb81f8de1aa677dbf22ddffc44a0634b3562eed0aadaf264402b3a8`  
		Last Modified: Tue, 07 Jun 2022 04:56:01 GMT  
		Size: 3.7 MB (3678996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f19f7c7d5073b3daec192d10dd5c1097243609ac12726bd5f01620361aec36`  
		Last Modified: Tue, 07 Jun 2022 04:56:01 GMT  
		Size: 3.3 MB (3324409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3a2fae63759982b2e57ded564d702d7b2796cb6596fa2bfdb10deced765aee1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44561684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:489dc6112e243eee374c3db22d3fd5ce8b19d9ec58da3be3ddeee337314e8ba2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:47 GMT
ADD file:6fee77e76b27182351bc3f1670478775d45b940b676a9c68b3057638166e1f3e in / 
# Fri, 29 Apr 2022 23:22:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:14:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:14:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8b9131999f6427d8e2f8c2e6af3dc4889e32c5ea861065b2f8c24539e9c7d81a`  
		Last Modified: Fri, 29 Apr 2022 23:25:51 GMT  
		Size: 36.2 MB (36172344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e32408ebe4867c2297c1f79093340488b3a376d8635067d1db6b9a03f7ae14e`  
		Last Modified: Sat, 30 Apr 2022 00:27:38 GMT  
		Size: 4.1 MB (4147019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739ead4bfe37181451861b7314ee488b7b8e5b129ccc84ce944bd824e2ac556b`  
		Last Modified: Sat, 30 Apr 2022 00:27:38 GMT  
		Size: 4.2 MB (4242321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:47553a058afbf5e2741f2ba361b7fb539596b221d12e2e8016c07a8fc4a16076
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34501322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a238c8978d4cf9767d84a4bc08213f45e23cebc2c4596c2684f72a50f59fd428`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 18:16:47 GMT
ADD file:4e3bc2c80a7472615f8c75ce5306a21584b9e79bbf9d38909f6931d844d9bdbb in / 
# Mon, 06 Jun 2022 18:16:49 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 19:18:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 19:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3dfa8236861920dda2ce67cef8af1fa06ae6cb669612efbbf4a2c177a1c1e451`  
		Last Modified: Mon, 06 Jun 2022 18:39:09 GMT  
		Size: 27.2 MB (27205258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9da3832471cab1699fe42149beb8fd20cfc97fd0502136045f739495c7ec559`  
		Last Modified: Mon, 06 Jun 2022 20:18:40 GMT  
		Size: 3.5 MB (3492079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9964b882c71197b2b0ccbbd484d2f7db67a95789eb4863714c6825ce59d7c`  
		Last Modified: Mon, 06 Jun 2022 20:18:39 GMT  
		Size: 3.8 MB (3803985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:850eb1541190e05c60a7fdb2abe84142d349deba8f35d64cd01e14e092dc4351
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38009104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:534048628b2134b31c35418ef0a72976c050586df83ce082459550a7f824acdb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:22 GMT
ADD file:cc4245955f965ca283118b525a5660643b47b60228e1c1ca6350d786a2f54a69 in / 
# Tue, 07 Jun 2022 04:05:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ef8f08deb2ebee9069392096f64a14c620b5694921860dc066d66f8418e72b44`  
		Last Modified: Tue, 07 Jun 2022 04:07:58 GMT  
		Size: 30.4 MB (30425743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2497e758347dfbb792ae78569954af6fc4388e3f627db376173aa91653450b`  
		Last Modified: Tue, 07 Jun 2022 06:08:04 GMT  
		Size: 3.8 MB (3763634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd01edb65da54b7b17c9bf0d0f3ef8d36e9d24a14afb5c3fed60ea1694f6dc0`  
		Last Modified: Tue, 07 Jun 2022 06:08:04 GMT  
		Size: 3.8 MB (3819727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
