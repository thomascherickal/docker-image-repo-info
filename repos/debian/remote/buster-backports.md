## `debian:buster-backports`

```console
$ docker pull debian@sha256:101614c76f367d53cfa559a6200fe8a35d82f55df29d2e5d377ad8d417a14dc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:874ef968693e757ecd4818149523a5edfdefc2548ca0c9aec058ca30e7926152
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50448862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e587df764e2da31662c5d4f7d6fd7a558e5316a4fd8169dd88db646b73a40ee`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:38 GMT
ADD file:f5e6e6cbfbb36f50f49f06fbac953a130383acb67a1c5e9979441f1915b1077d in / 
# Thu, 23 Mar 2023 01:30:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:30:42 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4e2befb7f5d18aa27b3619ddf1b93607e62ca82d0c627557537c149893346d86`  
		Last Modified: Thu, 23 Mar 2023 01:34:40 GMT  
		Size: 50.4 MB (50448639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a22526bce0ea46423747a75def0ac9d6a201331b082db6bb66a5679f6045de`  
		Last Modified: Thu, 23 Mar 2023 01:34:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:3907bb46643335d0fca202a1487524d20d9fedb650fad17661eb89d968cba4ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52e4e10c0b44df00e6c8abeafdeeffe80cb70a1774298801d53423b04123d4b2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Mar 2023 23:23:23 GMT
ADD file:dabb9dad1d8086faa890c6425e759e27f1052d9677aa640dd310def49d8a5bc5 in / 
# Fri, 24 Mar 2023 23:23:24 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 23:23:38 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:09b82635e0c9396d28359dea2597b070f13d2e7fbdd1b9cb395b7f7a1cd09d59`  
		Last Modified: Fri, 24 Mar 2023 23:28:44 GMT  
		Size: 45.9 MB (45915861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c45c1b6f379a9b05da5f8c2d08f716957e1a645ad48b439b4a7420397f41d83`  
		Last Modified: Fri, 24 Mar 2023 23:28:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d68fd171d73cd5b4c5429812d3903682dece586e91b20107993baf4bb5b4a7b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49239943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce3c1eb6c5aee4696a5abe8f97e9b75c91312bd855ec3f3b19f4dfada5ec582`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:16 GMT
ADD file:35dd833b036748f887e8224e9c5f09846aa5d1d6e1798d12a6355c28e0a087d3 in / 
# Thu, 23 Mar 2023 00:45:16 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:45:18 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6a9fffb8d1cb480140dc56a24c58a5d1a284109cd8a640a3719bcda5963d1298`  
		Last Modified: Thu, 23 Mar 2023 00:48:25 GMT  
		Size: 49.2 MB (49239721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116a819a81004b23d7a9dbd75c5935d1ea5243eb1c41e7cc8c00fb9b62480f0a`  
		Last Modified: Thu, 23 Mar 2023 00:48:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:2af240d313c89f459b54edd124ec5df996458179bcb9ad626ee253e7b2730010
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0c8daaaac0ff28e06fa8437deb9a5d98c2edc9cf5960e22d2a1f2cd797bfb3d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:29 GMT
ADD file:b1ee2e3a45801f9bc3a5b377c91d729589265495607481a83edb501aacee34e7 in / 
# Thu, 23 Mar 2023 00:39:30 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:39:32 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e3f08b81fb272fb973474eec1fcbeccf665d7941774b72a1e9448a5daba9682d`  
		Last Modified: Thu, 23 Mar 2023 00:43:29 GMT  
		Size: 51.2 MB (51207106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85625525d94d6e908cdc57fc6c1ce9f9bfeee0bc464fb248c7fffe7c3367365`  
		Last Modified: Thu, 23 Mar 2023 00:43:45 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
