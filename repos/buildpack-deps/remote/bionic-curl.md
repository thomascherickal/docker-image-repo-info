## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:5b95a97d821fc1a64d13ccbdbfe1cc9614fe0238c540496454a8f04ec6adf0be
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
$ docker pull buildpack-deps@sha256:eb2e182b4921830b6aa5bac0b27dd694f6828bd90ba0b6870b10deba25a9d26e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36371200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e6ec49f5bf6cc6e2e618fe771d1acf0608c7ece10053790e9eed1f70a3ff9d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:52:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:52:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3249722907386ae920ad1220d1ed4fe93044ffb9a804fec2ccafaac96594fda`  
		Last Modified: Tue, 02 Aug 2022 02:22:16 GMT  
		Size: 6.6 MB (6637279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155723c6ff3a636e724c25906d09d75ea6a3c70595fbda2c655ab3ae75c9dccf`  
		Last Modified: Tue, 02 Aug 2022 02:22:15 GMT  
		Size: 3.0 MB (3023651 bytes)  
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
$ docker pull buildpack-deps@sha256:0252ccf587f9487db325574d1a3fe8bb3eb31d91533fe434630d4477512c27c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37130904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad2ddbf64a9d8977cd6af1ef106ddd00047be5f711281f3d1e867d0fa203f6b4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:50:55 GMT
ADD file:6d22c6318075d01068d0a9213f33655abf6c251f8a71d98c17b857b9021b43bd in / 
# Tue, 02 Aug 2022 00:50:55 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:15:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:15:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5496b4c91dece81ce997c62cf2e1ef6f1764e612c6e8f0b385722c6645e4ad30`  
		Last Modified: Tue, 02 Aug 2022 00:51:39 GMT  
		Size: 27.2 MB (27164268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8439504988f2843b5e4ef5dcf3fcec03b31d6e19990975f2aea8b59fac990dd6`  
		Last Modified: Tue, 02 Aug 2022 01:28:03 GMT  
		Size: 6.9 MB (6926590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b6dc1acdd5e447706ea88235a69f6f13e0c84711fc699ba22ed607d3bf8147`  
		Last Modified: Tue, 02 Aug 2022 01:28:02 GMT  
		Size: 3.0 MB (3040046 bytes)  
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
$ docker pull buildpack-deps@sha256:234d3dc6cd2342a69b57b0f60312185e082d0bff6004b71e701f4be7a0ea8784
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34677626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a2df4940e4ad7ca511dabe93e18df5b61cabea6c43542e92a66a618f0aa40f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:57 GMT
ADD file:3d2e9b401524527b395347bc3847be7c9cb465b9a214a1a1d31e74330e293c45 in / 
# Tue, 02 Aug 2022 01:01:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:14:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:14:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be3ed498266c519f84268ff1f02085fa249c0e32fb60a59466e24c862b5f094b`  
		Last Modified: Tue, 02 Aug 2022 01:03:25 GMT  
		Size: 25.4 MB (25369584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fae7a4d4ea1c6cff382e8f74717aeaf4318c898d85ce8bb7454752509fb931`  
		Last Modified: Tue, 02 Aug 2022 01:38:08 GMT  
		Size: 6.3 MB (6330826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97089932290a776584a9006d4825a8ef9a13185d90ec2b9075b7691058ebb307`  
		Last Modified: Tue, 02 Aug 2022 01:38:07 GMT  
		Size: 3.0 MB (2977216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
