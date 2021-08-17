## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:59f5f2072cefb831620932277aaa684340a775505eb229cdf4a8ad9f5d03bf72
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

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4dd4d22c21300b3ecd56e72c4c38dd22c6e699b2c8f34aa04a7d6e2e103a0a6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68265792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53846d03afa6818927e5678b2c148ef3dc5307dfe4a3bfa2190781347be8afdd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:116f39525f541f44093df915b4674cafb9b2555f5ec0eace5211ffd9c93e8da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65217356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede6910dc92dec2346ba7f7ffd7827e393c476445713ce0623505d60f066e49d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:49:34 GMT
ADD file:4a4158b5432e31cd686b7b2874c22d86a381ac71c3146fe6746501db3d216b41 in / 
# Thu, 22 Jul 2021 00:49:35 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:03:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 02:03:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cd9bc325fb9e2673d4a4f97499e5ac67f82d24eef19ed2cb8d13af9c9256d20c`  
		Last Modified: Thu, 22 Jul 2021 01:01:22 GMT  
		Size: 48.2 MB (48153246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ac5ad14f3066e98bd031f59bcd25af51c46975f1f67aa9e984aae49997f855`  
		Last Modified: Thu, 22 Jul 2021 02:21:02 GMT  
		Size: 7.4 MB (7376533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538b6814e6bbc64643ef42ffb80c592cecc6833f8c77baa213b7d572de2f060`  
		Last Modified: Thu, 22 Jul 2021 02:21:02 GMT  
		Size: 9.7 MB (9687577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ddfdf5e8380f8ef257e9c89fc47013d7cc22d71e9dde4f7dcd9dfb3f652075ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62385276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:588a1e4f35a98591d5bd72165b43fb04a6de8ca064f41f1a3a6009a0bb4a4ced`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:73fb25f70aff2fe1395437e2f63c45afebf8d13d9fc399df0f72cf04ca265caf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66901350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e784e44a7e53b899b8755b0e62173b9727c5ee15abd70cb4e6c954b7b877fe0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0f44fa0a78c1b024b7b57c7dfdaf67fd1d83e6a47c25ba6951db73d1b87367fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69546124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca2a445c5ff6e65a07e933e73aa21587acb1ac2b1a7d72c2c7f2a19b28473ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:51 GMT
ADD file:98d4857c154cb75c011be69c57275c4a1304d441ddb03fe8388342bc0e2a9689 in / 
# Tue, 17 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:59:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:17ec3e1e9f7b10e3075002c6dd4297be244b5386198d7a417a9d22302080b6f7`  
		Last Modified: Tue, 17 Aug 2021 01:50:25 GMT  
		Size: 51.2 MB (51207344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54b2adab88b38d8137579946b8da20be9bdb174381dc3e02340d5a786c41ac`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 8.0 MB (7998779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea932812b2c3a1292981a835c426875eb75f95cb82d925268ceca609a2f23315`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 10.3 MB (10340001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a8f9d30433eef4ec1a1a845da18190b51a7cab1753580087d9589e553e5128db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66349263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430f47cdc328790aad47f97782df3e71cb1f4248f994e0bc60b6bfb2f2f87ba2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:22 GMT
ADD file:1a6aa3d9fc5224e35958d4109d5bcb3afa5948beb85e45b91f46655fe8fadb2f in / 
# Thu, 22 Jul 2021 00:09:23 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:42:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 00:42:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dfc6cf8967b24f7ad8c4469c3140cf3967000ae27e3b40b7c72fb89755953841`  
		Last Modified: Thu, 22 Jul 2021 00:15:25 GMT  
		Size: 49.1 MB (49080577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f1ec44468b6cf3c95775fd68ad34176e3f3f5b114e01ef45fda232435a0ee`  
		Last Modified: Thu, 22 Jul 2021 00:54:11 GMT  
		Size: 7.3 MB (7252390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5a98fef30417ecbf0d84d2f4e0a5d8c4c745505f4453d9d128eaabe85f0caa`  
		Last Modified: Thu, 22 Jul 2021 00:54:11 GMT  
		Size: 10.0 MB (10016296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3fc82664a4c135837eb0cef01360957a866f9baa21d9028c9dd683fcf179fc4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73182173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456ba3d71899999f2ea8480041211aa6d3353f3958f7dd6f34b7e2c018a3797a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:18:15 GMT
ADD file:e6b00a20c003d499ec3793592cb620a450afe5de34f408e897ae9ea6efde50ea in / 
# Thu, 22 Jul 2021 00:18:25 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:04:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fdbf50ea37550aa240918e3856b527a5dcc59fb570024ad98c902fe59e2ffd85`  
		Last Modified: Thu, 22 Jul 2021 00:27:11 GMT  
		Size: 54.2 MB (54182444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c4eb1cdb7dec331ac914405cf72cda55e246497aa6cdfce759e808d8b0ef32`  
		Last Modified: Thu, 22 Jul 2021 05:13:39 GMT  
		Size: 8.3 MB (8271846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1473db4da98c45802b5d0ee67cc543db64220182999ed71199a61f006246bb4`  
		Last Modified: Thu, 22 Jul 2021 05:13:37 GMT  
		Size: 10.7 MB (10727883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d398b050dd1b4b463d235d080178f508c7fb7d5969fa508643a05685063e0d7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66287689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b51aacbbdaeb0eb0f86c32b9f96b66a4527cf8b1eefcfa93545abf717959829`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:21 GMT
ADD file:0862dc2e420958057c0edfbacc39968850751ffdec84962ab8577b7787c5296f in / 
# Thu, 22 Jul 2021 00:42:26 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:11:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:11:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8776c37054ddd28ba8fe526b8dbc08bf7b521ae9ddb8eacd008d05185571cde0`  
		Last Modified: Thu, 22 Jul 2021 00:47:50 GMT  
		Size: 49.0 MB (49003783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c06f635d71fe906f56e25278d5659aa940f095c1ecf199e41436e197534383a`  
		Last Modified: Thu, 22 Jul 2021 01:27:40 GMT  
		Size: 7.4 MB (7400582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f57129f34059279bed7373d2b35f16c94df2418b85c5ae20dc715f2e1999498`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 9.9 MB (9883324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
