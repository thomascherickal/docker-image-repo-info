## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:662e5c253bbfc5758d8e013c81b93d0eb26ea1759a71a6396658c79e6101c6f9
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
$ docker pull debian@sha256:abf56b870c626876161b21c0ef282925779f2fb59456cb726d6cf7328a5bc16e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55046999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a59f8973e419446d18441c6d9456c5f0dc07e7bc20c7fde4da35d813c0a70cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:20:09 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d64de1b0cf78ac2cefb90979a3f0770583a344e7da1923ed72e3fd3ab612e`  
		Last Modified: Thu, 09 Feb 2023 03:25:02 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:0873908a47bebecb9a9d1f3023724f8e01b3438493f0b02823d4a10961b620e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52550044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3442fbad09389813b5c43f1e520658ffe7afddb3c8fd6bda837410bf6cb3d25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:48:48 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ea59f4fdde97c6dd4edbf112a13e7275063527acb840becf5dc21051e70439`  
		Last Modified: Wed, 01 Mar 2023 01:52:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:7757c3b532c4888237cffb220eed4fa52cb371efaa52f89b21b6e29d95a9c638
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50212272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21db3d8fab7625d55329c29f14853fd941c136b0240f6dc0af4d86eb19b9d7cc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:57:49 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0546b5efd1f515093ac3c65c28960c91b53c63b17611cdd7ddca5a4a10b787f3`  
		Last Modified: Wed, 01 Mar 2023 02:02:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:89f44c45383ce79466de666294dddee54a339a51c6063db652983a742d6665be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53703441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f47f81ffc30ab34ee410f74b9ae3fc7ca913bfdd532d39d0f8a6e6745e5e277`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:20:34 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410c2c002edbd8319b5268b01ce4280e99ea177dd383b96930b012fd67f04868`  
		Last Modified: Wed, 01 Mar 2023 02:24:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:aac31a053c5c65f4f740bfc36354d89607136d8fa95969b3f91ad664ba5877d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56028302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceab832fd86ea848012a582a117cbb654797786ded2a00e4d66b6f020d529cc8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:39:07 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3592856457c8f980ba4bdecebfae4f4ac34c744229d9494553f0b24a312082e2`  
		Last Modified: Wed, 01 Mar 2023 01:44:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:fb35c8858e9893749f7767f8bf1ac2c6f52890b7c5c6df888b826a6745af890e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53265403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9dfcbec6c1c877f34a075a557c1607b5b3a06f8815b1064dbc2d995f9bdef09`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:10:33 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933c99fa7c77f531b37a9edbbfbc39fa314e6c58c1cdead002ac6e81576b6bee`  
		Last Modified: Wed, 01 Mar 2023 02:18:25 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:aa585e1e33a7799482b1270d1d76001741eec64ef58c528384ffc941030cf928
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58923694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0002d058c98437d5081cba499b6a72d01ddd5ffdcc9c88844cd8082eb8eaff73`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:21 GMT
ADD file:0cbfdb018ccae985f6d364f1de7d39fa004cbc966374ba83727c34aa39f946d4 in / 
# Thu, 09 Feb 2023 06:21:24 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:21:33 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:219f4ac08f8026026673d3212473b774749e609a07e734f5812912239893f829`  
		Last Modified: Thu, 09 Feb 2023 06:27:52 GMT  
		Size: 58.9 MB (58923468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e66975b9b371dc88600a464ef4ab402c87b088f3f4fd97c55229d1208c2195`  
		Last Modified: Thu, 09 Feb 2023 06:28:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:e0094bbc4175dbfee531c98acedf7ae1571c687b7ff6e56061131a86c9ce4c20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53277920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:248a7080e717bba67813c48c0d50e63be44f794ca173d47fdf81ce262823c4da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:50:20 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49954ef1ca95589a8b4a331282bf04a1c0e9f926ce6338da6d086a467d5daa4e`  
		Last Modified: Wed, 01 Mar 2023 02:54:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
