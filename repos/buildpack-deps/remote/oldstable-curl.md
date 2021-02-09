## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:ae65aed6f9169ec0373ef4d3a807b2762578fb77933c1a03aa6e1d91af1c7c8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:504d2bcba27b8d0000fd0bda2b4c4a5dddab5d81426f4c51a5ce6d57d7a67b4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60990444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648e90cd03631bdb705ea6e7d5c84d80e067bc4e5c6d78abc48cf857d7de6a16`
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

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a634bd26a599a05e5ebe80e3ea60564948228d4bb84ea82540725ba5d37af342
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58572788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3769c53ecb48e82a78c3bbbb0dd50cee4ddcd253d5cf3226f95b23fc8a65627d`
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

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f4038391e75b6f1d9182892ec5ccb86797ac2312cba9e7f1ce2f0efa8102fcbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55954697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b74cd4f92469299cb0d1e2c2c54e7d96cecd9fad4835d81b5fb1ffbbe0aef09`
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

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:381e9b05d311942ea02631365eeb2c3cb1d1d3a501f279314b06824c2e18dd19
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57456754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59a32216466dee089c5ea06f2c38e62940bd04e8acba2b08d4ffcfe079574717`
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

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:857830e5d2f8b4fcc5ac342e5b8672eb1cc6afc65697d5e99f257b0b49a15ada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61980489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ace57d773b2442bba09b6dbc7409ef9a3813a5cdc95a21a20a68a5b212236a8`
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
