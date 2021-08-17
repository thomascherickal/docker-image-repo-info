## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:fb466b0b760f39519c6cba7ad7f48980ed46645cf047780ff7b8a02ed070c850
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

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:696bc2e363c02ade646535b3e563297eb9d4f265e694b27270b6ceb672da97d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61016637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d182fe945a36cf74bc01edc6481518601fa080efb8db9c9ce84b4bba1dca7af`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:05 GMT
ADD file:fc9409352ad67880b83ccf1ccd1587eb2666715eae04e4dd98fca919f1bb98d7 in / 
# Thu, 22 Jul 2021 00:47:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:15:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:08224db8ce18b31a78a0a26d1b344d173528e50a7067797c9df4de5d8df353e2`  
		Last Modified: Thu, 22 Jul 2021 00:52:52 GMT  
		Size: 45.4 MB (45379781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd3caf86f5b9d8f8e63437571297df5fa6d454140b9c1985c47d6ad526da824`  
		Last Modified: Thu, 22 Jul 2021 01:22:23 GMT  
		Size: 11.3 MB (11294469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c316554a558d4aa95c0be17c01e4a0366d6026a98eeba53dca5baa6091e815`  
		Last Modified: Thu, 22 Jul 2021 01:22:23 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8354d4c0e56b16004f98f1a34c551c047f8d86e8430b5f1d038448953406a74e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58603715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f206ff6e6428324f3e0f7a0d73ca0a55e3c6092cabecb6a5a586a59e301282e9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:53:04 GMT
ADD file:bfe848278f8374ee4e7de4946371b7176fc2bbcf40afce8ee1f9738af7b06694 in / 
# Thu, 22 Jul 2021 00:53:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:11:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 02:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:984fc5232b7d0db08285a008f512c6a5de7610d4f37c8c97ecd7b1bb98e2dd65`  
		Last Modified: Thu, 22 Jul 2021 01:06:29 GMT  
		Size: 44.1 MB (44091732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9d89827417cfad915b22c846cd8371b341fcf557926f53731aa581557fd3b5`  
		Last Modified: Thu, 22 Jul 2021 02:27:28 GMT  
		Size: 10.4 MB (10350527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21206c9923e5c0ba9febe6fb63521144127d2dc085d2cbd0398dc9a317d2ed30`  
		Last Modified: Thu, 22 Jul 2021 02:27:25 GMT  
		Size: 4.2 MB (4161456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:253d4eb5bd45893900712b4429bd5af52f65b33cc63321036aa8a0eb28f39ad8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55992235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ccd9accc89f56775e9e88bcd3b7436248290478bd825c09d2f7550b31017cb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:06:56 GMT
ADD file:544c40297b94c3ecc6561cf7bfef1cdf9763a18ce5e24b6841a1b70d0516d41d in / 
# Thu, 22 Jul 2021 02:06:57 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:21:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:22:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b3cc5e47308fe8ded537d7ffdcaba46fcdf803cfe9878bd9264754a50eaa128b`  
		Last Modified: Thu, 22 Jul 2021 02:20:37 GMT  
		Size: 42.1 MB (42120108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf69efd3b547fe4dc472fd34a54c466b82ce51b7f04957779206b5ea0ef9160`  
		Last Modified: Thu, 22 Jul 2021 04:41:23 GMT  
		Size: 10.0 MB (9950872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7430ae4c6b93ca669cc72566a38f952b74dece32c5897c46e51a5907bd5a0c`  
		Last Modified: Thu, 22 Jul 2021 04:41:20 GMT  
		Size: 3.9 MB (3921255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:486c3a6b2341e907b4b98d07a5bdb7696fc40fa53278c842ea7eb177b0ee4f68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57489760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5649dbe87bd6213b5227e797ce6214127107e4f7f8913c7e65e690d6f932c6aa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:26 GMT
ADD file:fab290162e6d28cbe115c866c49a1e09d955450dc9e831ccbeefe40e18cfa3a7 in / 
# Thu, 22 Jul 2021 00:41:27 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:18:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:28ed64be8f9ee39d8ded09482441a288852dd40c2e535b64e1f9c0271c10eb44`  
		Last Modified: Thu, 22 Jul 2021 00:48:16 GMT  
		Size: 43.2 MB (43178440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6227db87dba6bebff5c1f1a2bd2d290c25c44c23f3b974a4e99fe72b48777812`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 10.2 MB (10214761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cffb4d8549ecf5dfe60357ee2dc98dd618c73220f26c8cd505b088085229668`  
		Last Modified: Thu, 22 Jul 2021 01:27:40 GMT  
		Size: 4.1 MB (4096559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b810debde3eb574cfdcd27df6d7aa8823d9abe77ebe4f53964bdf041a68a36a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62014603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fabfc6d938961aae9fccd3e6e705d0e4dfbc4e363df6e3b8ead2cf9cff3982b7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:29 GMT
ADD file:c83a7d581497b7df343b529417c3b904cf901379d5124d738ac2539c778912a3 in / 
# Thu, 22 Jul 2021 00:41:29 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:10:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:10:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:27f236654eb1268b8d3986746d9f9fc7ef6d5ea038754025d6953961a088aff0`  
		Last Modified: Thu, 22 Jul 2021 00:49:20 GMT  
		Size: 46.1 MB (46097283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24560580734eb3c4c5331fdde7d8a3d17ba1b35f71b600a58360649f09e6d605`  
		Last Modified: Thu, 22 Jul 2021 04:18:33 GMT  
		Size: 11.4 MB (11352389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b500f684c69eb6ce0ff51c27787bc3252805e441e32a1d1e6b6879f88b8308f`  
		Last Modified: Thu, 22 Jul 2021 04:18:31 GMT  
		Size: 4.6 MB (4564931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

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

### `buildpack-deps:oldstable-curl` - linux; ppc64le

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

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fd934cd37571ae89d232a86713d6299c4aeef09e4da3efe1a3467132462d004d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59885441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4348a1e8c2b52aadbc446941d2408a5db695b837355593875eee8509fe4e37de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:44:05 GMT
ADD file:ce4b8c76522cbe8599502985424901aee9d30d37296761d47dbcb9b0770f7aa2 in / 
# Tue, 09 Jun 2020 01:44:08 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cc8faf537ff83acc994f80bcea99d8e073aa05b5eb0dab5ce495510af0b6d1f6`  
		Last Modified: Tue, 09 Jun 2020 01:47:50 GMT  
		Size: 45.2 MB (45232505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9816eeae17f469b3b58481bdbae04cc1b7b69f8d8a6ef15f6972d91ba2f29ee8`  
		Last Modified: Tue, 09 Jun 2020 02:19:43 GMT  
		Size: 10.3 MB (10280522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a7344ca59dab92a8238f2df0ea3779840ec21afc295e24f39259558c3bfc05`  
		Last Modified: Tue, 09 Jun 2020 02:19:48 GMT  
		Size: 4.4 MB (4372414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
