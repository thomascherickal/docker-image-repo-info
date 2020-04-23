## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:c433b95d6a8553f13922f87d56040caf5b1ffd81f5f1ed0c366fbb3f1e1bae8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c6d2cd2830f042eea0a99c94a96616c026156a171e89c69408f76f0dd416f6c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70212108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad4f434eb0f12cf8db178e6147602761dcf57523f25a544a6927fd645e714e2a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:21:58 GMT
ADD file:5d2d72d29ae1c01dc7f5bf337c78d40925a9843052910f79f066f681a2ec43e6 in / 
# Thu, 23 Apr 2020 00:21:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:58:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:58:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2bbc6b8c460d7ed40af9e8f69693608780022541107dbb47c4a717e0a15e84f4`  
		Last Modified: Thu, 23 Apr 2020 00:26:48 GMT  
		Size: 52.0 MB (51979787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af86ee5a9d864ef79346df3bd57faa5631e1b16cc83353b543768d6d306d88f3`  
		Last Modified: Thu, 23 Apr 2020 01:04:33 GMT  
		Size: 7.9 MB (7934538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb4c0ecf8059fde4ddfb61bd7bca435c46f56832aba0b7726caffbe9f0eb90c`  
		Last Modified: Thu, 23 Apr 2020 01:04:33 GMT  
		Size: 10.3 MB (10297783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:5ad82a3585f02060da3f47c1528e28c073a9fe5732e5b976e7a4d18ebcdddb2a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67461650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4d66c8117050e73cf094181b248ee86b4c28b4cbf0e5bcdeefebb73d53c512b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:30 GMT
ADD file:a75ce77565b83a916eece2d56e963b63f9ee7367ef197d8c290ff79a800514a6 in / 
# Thu, 23 Apr 2020 00:54:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:37:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e7313629a61ef455f6387257ffb8f19dafc5546554a81db1483683758531fe25`  
		Last Modified: Thu, 23 Apr 2020 01:02:16 GMT  
		Size: 49.9 MB (49937767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c899094d7c95a1d63461502d6a6462086ecd6082030f55fd59fefae8e1088d`  
		Last Modified: Thu, 23 Apr 2020 01:51:55 GMT  
		Size: 7.5 MB (7515305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19b16385622348c287bab3a3358b580809022125ad4d1aca43b5c38cdfcf2e`  
		Last Modified: Thu, 23 Apr 2020 01:51:55 GMT  
		Size: 10.0 MB (10008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fe2aa7c2d350c24b2810713189ecc2a7dc4cf1446e9b572db4eb158cccb9916b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64584291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e042551de993ce1fa6414237932d14d1e732a2498ac3725cce7a9634eda5cf3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:02:49 GMT
ADD file:5de6dfe62ae35545ab2dc195cdc7ed6211867d4583f721d08acfff371bc7cecd in / 
# Thu, 16 Apr 2020 01:02:51 GMT
CMD ["bash"]
# Fri, 17 Apr 2020 02:09:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 02:09:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9d58ce8574bee4c2429ae80f47b2650443254f3f9a0dd9fc1c8d64277895520c`  
		Last Modified: Thu, 16 Apr 2020 01:11:11 GMT  
		Size: 47.7 MB (47655417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49d113a28808faa8fe3cf110ffbf1d3f61e1734b4bf5bc389129f31b164756c`  
		Last Modified: Fri, 17 Apr 2020 02:13:40 GMT  
		Size: 7.3 MB (7255893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd02f3a35cf68582a2a9020525ec2a2db6792c7abd94d1eed23a0c585b6be`  
		Last Modified: Fri, 17 Apr 2020 02:13:40 GMT  
		Size: 9.7 MB (9672981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5301a8049500a33f64b1af5f6f239f3b8417f18403393f52e8ff74511832fb0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69012440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a14928fbadd7e3cf8282e45396d5d37b41810b98e0e54d2f66bfa0dc151ff25`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:43:10 GMT
ADD file:ff8b5c2517d26b49a4c8114e515f5413a0c64b28ff1e5d3fa1bd70603aaadff6 in / 
# Thu, 16 Apr 2020 02:43:13 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:17:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2f361d4eae096128866baf55f9d19448df20331f319ad8df0f05397bfd2fe7fc`  
		Last Modified: Thu, 16 Apr 2020 02:49:55 GMT  
		Size: 50.9 MB (50910038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c3a136011851aa29f08165cf962f4b5df6865a2236b90a5fc6d0f1c01ded33`  
		Last Modified: Thu, 16 Apr 2020 03:29:25 GMT  
		Size: 7.8 MB (7808061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d0c43c17c0157ca9f4cd6b676d7a8e76ef248c724901495c897b950e8ff1b`  
		Last Modified: Thu, 16 Apr 2020 03:29:25 GMT  
		Size: 10.3 MB (10294341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a87ba4e2f0adbb649bd496aa87acd535ce98f5908aa3fdf6d8f0086a48e5f4ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71893141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf71fda92f308bad4ad835866bcd71e851542bccaf450bb164365b5a1a8664e0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:41:06 GMT
ADD file:5651707cdeb4825b44f6e8cca314dc9b453dbc8c9eb87d4235235b6f6065edd9 in / 
# Thu, 23 Apr 2020 00:41:07 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:53:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:53:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6b90db2302f3b878a7e51a668d323ec00b33326362c4983e10df2b689e081dcc`  
		Last Modified: Thu, 23 Apr 2020 00:46:19 GMT  
		Size: 53.1 MB (53123711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce77e9469d5af64bf3279f4b449bc6a887436148b9e1690295858e67ff72aaa`  
		Last Modified: Thu, 23 Apr 2020 02:02:44 GMT  
		Size: 8.1 MB (8112210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea37667c03d37033a105606940d504f39ee410a6c8103822b0079326b905c448`  
		Last Modified: Thu, 23 Apr 2020 02:02:44 GMT  
		Size: 10.7 MB (10657220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e9fa88f5acc98e2d6c94cf216e5582d2c661e9f1c57c3e94852919db29ef8110
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68481963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fcfde8c0c85be33261564e43540bfc3f3667b763f2aeda69a91bba55661f6e3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:11:00 GMT
ADD file:66d4b8806942796ca49e31a046824a633333dba393126281f5c12e26efea8e7f in / 
# Thu, 23 Apr 2020 00:11:01 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:56:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:56:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e50f308fab9e31aebf27548f07771af5a99a609ac88a60bbf74cd4f85125c24f`  
		Last Modified: Thu, 23 Apr 2020 00:19:59 GMT  
		Size: 50.7 MB (50696153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81374d42ab3f43b1e9a01bc0af60264f1036fe997a6abb2a98e309bef8774229`  
		Last Modified: Thu, 23 Apr 2020 01:13:33 GMT  
		Size: 7.5 MB (7461350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f82f88069fa53135d2819a8aa2d5e279767bf7aaf186c38c0b84e09717b63d7`  
		Last Modified: Thu, 23 Apr 2020 01:13:34 GMT  
		Size: 10.3 MB (10324460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a14d7ed8a8e0f77071e239ffa7a51fa9fe7a9ee93f7264a79a14ea278c5b9928
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75188422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d1f48bd60d679449c7d32d7c82f11d48f4d1d69a3739d09f4094d63766f26ce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:38:45 GMT
ADD file:d55bd2bc22fb060f41d4316af4a741b519580bd2eaf76cbbbf9e3b88355447eb in / 
# Thu, 23 Apr 2020 00:38:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:59:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 02:00:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1757960a31f3d7e8a61f52b30d276d1605aa71eec0c10f82c131db13d7402512`  
		Last Modified: Thu, 23 Apr 2020 00:52:17 GMT  
		Size: 55.9 MB (55855455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6563142de6e877d15e44abd8c25bfd401d3b30ad60789123881110c1b09c3973`  
		Last Modified: Thu, 23 Apr 2020 02:26:04 GMT  
		Size: 8.4 MB (8357037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8308c7f5986dc304d470a4bb73bbf6316be522707269361fee59307548cc763`  
		Last Modified: Thu, 23 Apr 2020 02:26:04 GMT  
		Size: 11.0 MB (10975930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5db4daa50ddcf6520e2975fbda06f770589115dafc5b73ae7149a512818a25ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68366562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c267f3cef03e43df617a65922b94350bca068d62085f85098de51afa7f55a8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:32 GMT
ADD file:8af210766ac887956b2d532d05d6f2685732ae449b64cc451bb1892dd0d39fc8 in / 
# Thu, 23 Apr 2020 00:52:35 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:58:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:59:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cfdfbea2787f2ac0078069f7f5d3094e3b61cefcec7239ac77ce892b23d101ba`  
		Last Modified: Thu, 23 Apr 2020 00:56:39 GMT  
		Size: 50.6 MB (50581330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b13e3ca73b27934f52752169891ab565d3136558697ae5958bb58e05acdcc84`  
		Last Modified: Thu, 23 Apr 2020 02:08:41 GMT  
		Size: 7.6 MB (7601311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf12399d434a43c9b18e6f51ac8d33334d68063a5e80a24b4db1e4a3c589fbe`  
		Last Modified: Thu, 23 Apr 2020 02:08:40 GMT  
		Size: 10.2 MB (10183921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
