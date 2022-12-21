## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:260bce2a24fe8beab3de6fdb9d0b3fa69e4a2904fa67da5e4f1874d592ce1e19
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:7b0798374c08193bdd947e9ac82c0b976857848fe20998e4aea93a585281f7a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55025392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33adbd87f934d4a6c25af3d8f3d713fbb083db88d5f890a76de04671fdbb3a48`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:20:25 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d2cfcd7624bd828b33928d163b914ad3724ffa89a92ff6c333039efbeaf077`  
		Last Modified: Wed, 21 Dec 2022 01:24:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d8719807b093df3ec60363113b4930b84f668cf9ecd87f1b7f56cef5281827d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52545023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9058567953d44f0a695a2c448fb6a23ca360139e687716a86c1c21c7be67b7c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:07 GMT
ADD file:92bc802977fb4abf65d3a11a702509aece192d088d815bf79a0e6bdb5a8b57c8 in / 
# Tue, 06 Dec 2022 01:49:08 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0eeca4d47a0d9a966ac355f8eb8d728ca02c90f2db97fac6164fb9dd7eee639f`  
		Last Modified: Tue, 06 Dec 2022 01:54:02 GMT  
		Size: 52.5 MB (52544799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f61db4b316b9644e5a64ea5198997d338ffe2750468bfa0ee668470aba88c2`  
		Last Modified: Tue, 06 Dec 2022 01:54:22 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:797f3584d9ec626697449ecd80ac1e69a2d3c01a54b5814e2174fbd0db3f8f88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50207313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c04a8b8754e8218b2c637773a13fb06218e0f4668bbb6853ac1a80f19b6b86e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:30 GMT
ADD file:72eaf12ec65c98e9cde1654b6adb2b3d19f7d81c13b12801c198f699252b7503 in / 
# Tue, 06 Dec 2022 00:58:31 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 00:58:40 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:58e27900c24f1f8f5b6b5eacbc073583f2372b58e9f5678dfe171b496b9cd71e`  
		Last Modified: Tue, 06 Dec 2022 01:05:33 GMT  
		Size: 50.2 MB (50207085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7c2b05534a97f44daa31087ab617829c0cdd24887dad490c696fdbaa01474b`  
		Last Modified: Tue, 06 Dec 2022 01:05:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:2ecc623d8ecdcdb8f5713f832fb6426e5df8a632454fa86efc4b86b75f9e0bd3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53699370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b4ed82197fc3738498ed3cc5285402e1d17d636cf13cd6d1ccf83384fa100b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:40:10 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2ba695ee23c89a841ece02d1afbc99cd343ed9f8082d532b2b6f8677da0e53`  
		Last Modified: Tue, 06 Dec 2022 01:43:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:6f3ad8d925313326afcfc880ec469cafb5092f41d94c07f89a91fb30ec1d6a8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56022611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7d896b5a11eb39c3e3f75354f54380cbef66e67e8c6cf0e8ff6dd92cf930ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:34 GMT
ADD file:f84226ae95254e2a6a67086b709477f04fcf4d6c3a6ed05dd9cabcda0156ec04 in / 
# Tue, 06 Dec 2022 01:39:35 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:39:42 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a9be27fc8e6e19a1a3d5f3a8805c7b1a4c21e2db96b34ed6fd26bb06b286b67f`  
		Last Modified: Tue, 06 Dec 2022 01:45:14 GMT  
		Size: 56.0 MB (56022389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2019581186642596ab1660223f78267eb5c87deac607247851bf0132004eb0`  
		Last Modified: Tue, 06 Dec 2022 01:45:31 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:832d55c33288618be1d9a35fd5be95ae84626232c275604296b60fff65cb1799
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53245310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78163a604aed6c83ff0a6333b6f682da34ce3ae809986104e3f81f3520d61653`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:09:53 GMT
ADD file:972bcf9c0f583e92c03e74f66acec816703788fcc96e3a43357262f69e552ce5 in / 
# Wed, 21 Dec 2022 01:09:59 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:10:13 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:977ef99ba351dc6668a8aa09ee6ce134ad6e6d0d9cdf1083465b1effaa1969d2`  
		Last Modified: Wed, 21 Dec 2022 01:18:00 GMT  
		Size: 53.2 MB (53245083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3af57db875a298e4ef4f4dc3d02a02780dc89e9aa8fde7d041b3383e0a4965`  
		Last Modified: Wed, 21 Dec 2022 01:18:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:4d06638bc8f02c1cd9660693367f51115b7238d3b5d5c7e08ae551f32cb74daa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58897268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2512e560538f1a94dad5c4545b2422d1e4764f4996294e73e11c3857839de092`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:17:30 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8449cf94ee7583a0102a721eadfb2052c59b324c09ae60ff8854976b218f1aaa`  
		Last Modified: Wed, 21 Dec 2022 01:23:05 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:ff38718dba116058790b11b6b64cbf1ba340de4b720ee8211ed4717db35cfcf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53273111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea82e477637d626d7d6f9bd243b5d4bab172863d0083ffd3865361cf8b70a75f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:42:37 GMT
ADD file:022ca98bcf37301887c0e5d24eebe36e6c81a037e13434cf887bb848aaabe291 in / 
# Tue, 06 Dec 2022 01:42:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:42:51 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a3a57c761295cdc2f327925c14939b8b76fff91be8573eef2420cd05dcb39c1c`  
		Last Modified: Tue, 06 Dec 2022 01:48:26 GMT  
		Size: 53.3 MB (53272886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9205efa7b7bde8b893738af9297750318e2f2e00a011f9beebecb36b96b299`  
		Last Modified: Tue, 06 Dec 2022 01:48:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
