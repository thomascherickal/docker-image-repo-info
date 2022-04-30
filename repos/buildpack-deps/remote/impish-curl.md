## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:301bed108c2c70cbe611f410343ca5fe2bdcf6ee64b86a2f6f3632cb62f0da51
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
$ docker pull buildpack-deps@sha256:024ac25c0bc92777e9804c2a82e233c4954d3c7b37109d678b04074a393a62ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37630130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe369d0b4edb90ea746276c55ee35f59e16d8c439782e06809cce2037250283e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:07 GMT
ADD file:e36038a1f6ee02f3f9a7db183e116f58d277e97cb7e71032634097d802654d02 in / 
# Fri, 29 Apr 2022 23:21:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:50:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:51:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:940122ec7d0c039d048e3bf953a33cd8ef814fd587266a5e732d24d2314af8f1`  
		Last Modified: Fri, 29 Apr 2022 23:22:38 GMT  
		Size: 30.4 MB (30383364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc136e8e3c47f61408398c98287fa53af20236ad2006f834594cc5863aa38b67`  
		Last Modified: Sat, 30 Apr 2022 00:02:21 GMT  
		Size: 3.7 MB (3694309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afad01b9cdd53ebce85092828446a6cd6f8cfb65ca1a433101b71577c8919a7`  
		Last Modified: Sat, 30 Apr 2022 00:02:20 GMT  
		Size: 3.6 MB (3552457 bytes)  
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
$ docker pull buildpack-deps@sha256:90224933b1f4fce13a17be37b5d015a9760affc7d552910d80ead924df8f10c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36035035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3bded070b488c30c2084f3b1ce3b937eff3acff037f792433556aa745489a5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:43 GMT
ADD file:d800d571fc22b337baaf45095bd1a303ca66065106c8b943a7a869e145896077 in / 
# Fri, 29 Apr 2022 22:49:44 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:17:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:18:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:924f038c577f5fb37fec4317d1c44a40bae2f6ee798dc0e31394270b30d69e8d`  
		Last Modified: Fri, 29 Apr 2022 22:51:50 GMT  
		Size: 29.0 MB (29029534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e757d57f9b92f1d537667767d80d964200253f44e0fd0450d481d49710944c4d`  
		Last Modified: Fri, 29 Apr 2022 23:25:46 GMT  
		Size: 3.7 MB (3677922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053745174b0f3dbc495ff442a2793d0657bdd261a9d160f87c6d47424f4d33d`  
		Last Modified: Fri, 29 Apr 2022 23:25:45 GMT  
		Size: 3.3 MB (3327579 bytes)  
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
$ docker pull buildpack-deps@sha256:3f2b72a797603e99ce96fff87e849e666d80037e85a0fe1ff7b53a08dd8225e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34506551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7020ae834412acd59934284cc26c1773e879260b50e1699074cae12a71f679ae`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:16:52 GMT
ADD file:9b1d81091b302d999994d0aff49d52975044c0786e8d7aa0df0ce41ec3c5902b in / 
# Fri, 29 Apr 2022 23:16:54 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:42:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:42:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3105f98235ad0afa0e8e8fb758ef0e3a7fa3bc505fc19f49da0968611aa32271`  
		Last Modified: Fri, 29 Apr 2022 23:39:06 GMT  
		Size: 27.2 MB (27210922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95edae64347238ed7479c721c429c7d141a6c1b3ea02127ba646cdf7d9443357`  
		Last Modified: Sat, 30 Apr 2022 02:35:21 GMT  
		Size: 3.5 MB (3491073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71357fe3de61b03bab1dcc8d5c48cfe0a5b87d712f28c6c79da9237cc7e2b4e5`  
		Last Modified: Sat, 30 Apr 2022 02:35:20 GMT  
		Size: 3.8 MB (3804556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:67158f87cdbbb819382473f02ee9f28f4f16a7b7817aba98abab8ee4b817b048
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38230108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f02cab92bcb0c990fe612ebcbffd829d956abfc1ca6a87de0d3d93f4f1f3b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:17 GMT
ADD file:1041ef5c07ca82ee2d7f626a60380e731aa09d0d2b9b6877b03abffa280e452b in / 
# Fri, 29 Apr 2022 22:50:19 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:12:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:13:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fe0d74cf06c14c44f5210e7c3b5af279f02a1d45707ee11e6afae132344bf765`  
		Last Modified: Fri, 29 Apr 2022 22:52:13 GMT  
		Size: 30.5 MB (30502867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98e5deeb0d7fe30f6c49a20d056ebc1bf7817655a9468ead107eb77a50d8911`  
		Last Modified: Fri, 29 Apr 2022 23:20:08 GMT  
		Size: 3.8 MB (3763492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5616be16d6fad891f5d8a2aa1456063444902583f787bdffee6956e7edc2bca`  
		Last Modified: Fri, 29 Apr 2022 23:20:08 GMT  
		Size: 4.0 MB (3963749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
