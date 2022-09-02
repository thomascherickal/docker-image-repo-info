## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:85d56063c429dfe7fa5b832f6f32e6a5633ebef50cb3a929960bc4ab297290d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:82e4aea0f5fd9ebc5fcacbc62339e09d6dbee6793c5c31fbcc2969046a184571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36364835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933ad5fd695e489d7ca313c946e5bcbb7815f2f6a35306da34ff3ade0a68da63`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:19:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:19:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fb6a221e5e93168fd6c2e8fc1f6ac2ffb76528d9054917643eac23ecd551de`  
		Last Modified: Fri, 02 Sep 2022 02:36:30 GMT  
		Size: 6.6 MB (6631015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622831c8e90067ca6fdaa29a2de932500fe9d780882f88bf84f70ea805f1e07a`  
		Last Modified: Fri, 02 Sep 2022 02:36:29 GMT  
		Size: 3.0 MB (3023735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:002deefcca3309afbba23fe105d4098b9ee5fc8e18698d0e00f7d9d6b55cc2e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30597825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011268dd21b5ebbbaba3632553bdb62c05260efc2add18e6b6e031ee96855341`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:53:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e447528136f6bae661b10431db78cb9ef7c19ab2955f91547ad42ab927ab0a0`  
		Last Modified: Tue, 02 Aug 2022 02:13:58 GMT  
		Size: 5.7 MB (5706380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e8366b770a1c9813eeefe7e724b6b8a31f9c0f568cbe9111d2175d9615ae5`  
		Last Modified: Tue, 02 Aug 2022 02:13:57 GMT  
		Size: 2.6 MB (2585832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:235d779b5ba96fcf962b04a65dbcd022592e60f60949906d82ad861d3c655563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32385431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6d7d8e1e57ac5bb13a52926ea521cf7176db645c4d2e6c7948de5d27cf18ea3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:29:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a8ce0030c4c3bf1c638b4471e5162eef4a430b61c537057f0f8ce51fc18444`  
		Last Modified: Tue, 02 Aug 2022 01:48:44 GMT  
		Size: 6.1 MB (6079418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63b2c6b27d8a588f648165c46146db98c94f4640019d6d8caf00868911d4133`  
		Last Modified: Tue, 02 Aug 2022 01:48:43 GMT  
		Size: 2.6 MB (2571299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a39a4b2da542008a0f3b616160d10895be112bc3e3a42e0dd987492997cc3698
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37123975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df3122d5e2603c6434e87227a776ca5d0b36cd618f47b7c49d7f1c6ba9e7b90`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:53:52 GMT
ADD file:93fdf10efcfc26ed4b10659ddc78284113a38c500811d27ffc41de25e2c9b4ab in / 
# Thu, 01 Sep 2022 23:53:53 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:49:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:49:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e09c10b62acdd55abc0548e8b24a3f314d657a49d5b9e4714ae753238c982a61`  
		Last Modified: Thu, 01 Sep 2022 23:54:38 GMT  
		Size: 27.2 MB (27164218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d41b26fc7fe91e2ecf5ff70769343de752ef61a55319ca667f268a98cc810f6`  
		Last Modified: Fri, 02 Sep 2022 02:55:19 GMT  
		Size: 6.9 MB (6919767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7fab530814537d9359e7280fa86174abd2e93c698749527eaaee9d9ddf4b77`  
		Last Modified: Fri, 02 Sep 2022 02:55:18 GMT  
		Size: 3.0 MB (3039990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f2864f6de33ac403d25267d00444500ebaa0a0dba6a0fd39043f71b28fca93e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41217761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877d163eb212fd3c36a9b028b547c8f0897158c6a5fabefa1683afa7d33a181e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:50 GMT
ADD file:32fc7b9b5853c93c45b1a96054c30104fd200ac7d40d0388aff736c478f917cb in / 
# Tue, 02 Aug 2022 01:30:52 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:39:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:40:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1a9ff13e38cae7994b55e6db5c3d190d2b7a03043ae238a6f71a285376de46bb`  
		Last Modified: Tue, 02 Aug 2022 01:33:07 GMT  
		Size: 30.4 MB (30441470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64118351c6d44eaafb1d0d7269124dc78b3b33e148c24e6e74c4ceec8f193a5c`  
		Last Modified: Tue, 02 Aug 2022 03:19:51 GMT  
		Size: 7.1 MB (7056186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef1999418600ed0a0609447fc56e75b3b7fa9da4cf9c794143e6e7bf5e4397a`  
		Last Modified: Tue, 02 Aug 2022 03:19:50 GMT  
		Size: 3.7 MB (3720105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1e8c03c38ce1bf92cdf02ea4b2defad095f6f4136bcac020548e8a6ae7b8da26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34671110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b075c50abcd9e48e0fcd7303d1708a44d75797fac41c55cd3696a96eaa013c51`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:02 GMT
ADD file:ee88f505cbf59825aed59486848971d1be33d8cc49f3a1df647a1486f310405f in / 
# Fri, 02 Sep 2022 01:03:04 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:00:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:00:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f98934bea0e17bc3e47aa5c2cb45f3bbcf512fd6211b763c88da22fffe217709`  
		Last Modified: Fri, 02 Sep 2022 01:04:37 GMT  
		Size: 25.4 MB (25369467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c380fb10cb841412807796ed4eb2a04c1db2dfb865319b304c5fe5fb3c1b9c`  
		Last Modified: Fri, 02 Sep 2022 02:14:48 GMT  
		Size: 6.3 MB (6324340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2f7f4ce09236ffef21b9c319d300db314d1a530955a50f2097828643dee8b3`  
		Last Modified: Fri, 02 Sep 2022 02:14:48 GMT  
		Size: 3.0 MB (2977303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
