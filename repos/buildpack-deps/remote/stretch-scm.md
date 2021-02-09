## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:afdf06a8818840ecaba50529f2cb7843412fe386758e75a4e469dccbf65b8663
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:22642db8101254c71f0dd36e67af6f8e095c46197282348a4f98ebbcd612c4c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110776905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86da3fbe603d115b700922d865e7daabad42b87c7bcb259b81fdb38813e4b20b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:39:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:39:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:40:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0edb687a3dadde6ae013f9b8f08340de1f105266abe3081bba8e8939267978a`  
		Last Modified: Tue, 09 Feb 2021 04:48:28 GMT  
		Size: 11.3 MB (11268653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6891892cc2ec4337be73614b6c3eecd8f1a1ac16eae254d1e4b6090358dd6782`  
		Last Modified: Tue, 09 Feb 2021 04:48:27 GMT  
		Size: 4.3 MB (4341906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684eb726ddc51bc28fc2fad831de6492b911f461a18bc7334ca803d74caea0d4`  
		Last Modified: Tue, 09 Feb 2021 04:48:45 GMT  
		Size: 49.8 MB (49786461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0e5173edad4af0889e5f90e3229a5751fece4954b8027046095269397d0f702f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106560622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7aa545cfcdc8e3da81ef5269899fb06f31e66fc796614e24c495030d87cf44a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:54:21 GMT
ADD file:4a3e3822cf3025351ee745e9adfe582c57bf68032749bb1f77594e37892e9976 in / 
# Tue, 09 Feb 2021 02:54:22 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:33:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:34:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:35:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:824fd5bfbc8362cd95df386c15b08b44f2ffd373830fe89693ee02957cc452d1`  
		Last Modified: Tue, 09 Feb 2021 03:02:51 GMT  
		Size: 44.1 MB (44091538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2536a58d0cbd78f6d44640d872806f4ad0629a87290629491121dd76a4140a8`  
		Last Modified: Tue, 09 Feb 2021 03:43:29 GMT  
		Size: 10.3 MB (10319821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc22fbf12ab85b871231e120ff2cb9ab0f28233e84f61380ac54e272febe478`  
		Last Modified: Tue, 09 Feb 2021 03:43:27 GMT  
		Size: 4.2 MB (4161429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320e998559357f3dc4829c2423d6b2cb179bba084a05cf33f7132ac9ab8b1712`  
		Last Modified: Tue, 09 Feb 2021 03:43:51 GMT  
		Size: 48.0 MB (47987834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0f5fea3d33a1894c3976c2ccba0899435841582ba4250628cae8c5115692b372
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102076656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa096a9cbee7f666e18fb455699773872fa4ab4a83343c5bce7778bb845cc586`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 03:04:53 GMT
ADD file:f884b9fc23d1b8ad0bd21aa823afd0ee186bdebb6829ccba72f77caaeffd8d12 in / 
# Tue, 09 Feb 2021 03:04:55 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:32:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:32:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:33:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5275c778c803ce7d82407c77cfad4fb07fd1ec80fc99ba94cef475a92e4d090c`  
		Last Modified: Tue, 09 Feb 2021 03:13:25 GMT  
		Size: 42.1 MB (42119892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae60b5ed65c5d76acc7c0baf6fe0549a03f324c20d1882c25d60b44aaacaeba`  
		Last Modified: Tue, 09 Feb 2021 04:42:37 GMT  
		Size: 9.9 MB (9913736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99de29c3c448a06c87fa2f84824e9e1d0e9a9c7d7aebb93fce0ca22b55b6c9b`  
		Last Modified: Tue, 09 Feb 2021 04:42:35 GMT  
		Size: 3.9 MB (3921069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0218d3a084ad8951d29ac2b647d325959e28ea7dd339a851356a9e6ba934cfb7`  
		Last Modified: Tue, 09 Feb 2021 04:43:00 GMT  
		Size: 46.1 MB (46121959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:01e9978e644636fcc730a5bdaa36ceb48546c6fe01146547a6678efafa9a8146
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105191638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ea9442a914fa646337ccb9d7a11fa9814a8840dbae64fd2f933306f5655441`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:17 GMT
ADD file:fb69ff7b2a28f793efbd16e04b74ffb4557d39e1844b3789075b4d3ff97a0eaa in / 
# Tue, 09 Feb 2021 02:43:20 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:50:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:50:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:51:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:296c9f0bf5f2cf24e87bc5abd674fc486e8df419d4aa2d362453f64d38900504`  
		Last Modified: Tue, 09 Feb 2021 02:49:43 GMT  
		Size: 43.2 MB (43177550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d546321c8e11789c75187b5b592633207519d75f96e8f03e8378d2da4a72a9`  
		Last Modified: Tue, 09 Feb 2021 05:00:16 GMT  
		Size: 10.2 MB (10182589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91c8ffe219846d18819503633eb252121c21cd20dbff74278b85c4029370992`  
		Last Modified: Tue, 09 Feb 2021 05:00:15 GMT  
		Size: 4.1 MB (4096615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8d698654f0ee6c5be4a19593a2d7a793c4bed9cb10de0c87d1d1c2ce6ba368`  
		Last Modified: Tue, 09 Feb 2021 05:00:37 GMT  
		Size: 47.7 MB (47734884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9fe1a162406889a4662cc23b1d824961d9b9185f664a15e3b1998df971e06d69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113244065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ba5cd74379902db5532d374f7e5c28bb5280da18006ba26cedc09defe775133`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:08 GMT
ADD file:4c25bc56152d0955bbdef26f612b172a90484913cbd1ab3332b3444c8c0c012e in / 
# Tue, 09 Feb 2021 02:42:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:15:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:15:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d7d8e56e51b8663a269c93107dcdf848d2f6a4f73ca51bb1ced208a1fa80c32`  
		Last Modified: Tue, 09 Feb 2021 02:49:23 GMT  
		Size: 46.1 MB (46097671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9386feb5ba4ed6a19c0f411d6bbeb6be55522fb55c5949e5b971a40dc2ad8594`  
		Last Modified: Tue, 09 Feb 2021 03:24:49 GMT  
		Size: 11.3 MB (11318391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f022cada5651b5e51027512bea825a799fd040cd53ba801a405d5d6ad0d011`  
		Last Modified: Tue, 09 Feb 2021 03:24:46 GMT  
		Size: 4.6 MB (4564427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba2031a83604ea64e4d0146093dbb549fdf4fd53cf78e7170fd2e072b1164ff`  
		Last Modified: Tue, 09 Feb 2021 03:25:19 GMT  
		Size: 51.3 MB (51263576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
