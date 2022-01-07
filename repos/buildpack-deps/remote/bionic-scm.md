## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:4a593603bbcf423bdd017afee789aa07fc7f137b9d72e456cca923e986c64085
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5e43b1ebcfe2b76e7912db780b8aac130c8578f962609f04f88de0e5abbb150c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81848404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2ce214211225c549bf9107a4c081cc04753411e5f7dc05e2fe18e780cb6807`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:02:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1404df7fbdef68bea55f7c051dbdb1aac1e564886ca277d1f8b1d0bf3fbe8e4`  
		Last Modified: Fri, 01 Oct 2021 03:17:56 GMT  
		Size: 6.6 MB (6643379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964552afca366bca79302ab79366a0528db0710e3db41a0a5c40e90d1b936c20`  
		Last Modified: Fri, 01 Oct 2021 03:17:55 GMT  
		Size: 3.0 MB (3022502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f547fe5b8db9e7e53004a6ebd2656feef7a91d529f9cb21c95b3bc8b108e19`  
		Last Modified: Fri, 01 Oct 2021 03:18:13 GMT  
		Size: 45.5 MB (45477448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:58947866db3f48fa361f7056b87a69b67ef6f4b3348e65f297ab297295dca8ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71273095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa26238d728f2e54ac4d6d4703e94f9750fa80cebe834eccf807a708e56ddd4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:17:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:17:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0514bc47630e4346d13917c20c9a52eb361c5077c2b17f804d305bb3aeeae1ec`  
		Last Modified: Sat, 02 Oct 2021 22:36:02 GMT  
		Size: 5.7 MB (5713518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43197d564770c4e86c4ec1c0d141238ad2a175e92bebfa12b212b729f581ae62`  
		Last Modified: Sat, 02 Oct 2021 22:36:00 GMT  
		Size: 2.6 MB (2584549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd05568a3d4d96e48d84348793a6345f8359538aed1403669bef0db7a6f026c`  
		Last Modified: Sat, 02 Oct 2021 22:36:42 GMT  
		Size: 40.7 MB (40670724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4cd7d49c2897395988195e6981f71613db7fe5968de61afdf95af231ada24c78
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75658920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5408604964ea4bbf7712a3f19081f5d0aeb3813f010484bb8d592e9dd6603469`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:04:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:04:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:05:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a555366df07c0f7aae069a38b120e5b8e6e95f359b898d0032574413b8b2c1`  
		Last Modified: Sat, 16 Oct 2021 03:19:21 GMT  
		Size: 6.1 MB (6084243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233462b381c92a25d3bf01a6a656557732c43fb811b0b5173d611ac8fd767a94`  
		Last Modified: Sat, 16 Oct 2021 03:19:20 GMT  
		Size: 2.6 MB (2570190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b11e5d0bf83fb3fb6bdb6b3cfd1967ea6e80fd7bf3b2f3f6167b48ba59cbd`  
		Last Modified: Sat, 16 Oct 2021 03:19:39 GMT  
		Size: 43.3 MB (43277011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7d140bf24dcf65ff58b19cc89ccff2d79214a2f617ce419fce461f3dea619307
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84406394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbd783bb288326f7a14713c56a0e4533639722b14dcc2aeda4418723dc6cc95c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:39:03 GMT
ADD file:4992040d291a9a6b53435279ff532c15e004fd7c7b35aa4783850a06ccff0694 in / 
# Fri, 07 Jan 2022 01:39:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:01:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:01:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Jan 2022 02:02:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd8c855b84a6297384d4a364fec672137f3aef84749b319ee5158b568545eb0f`  
		Last Modified: Fri, 07 Jan 2022 01:39:50 GMT  
		Size: 27.2 MB (27156435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e486905508589dc62500a1d530f1012b6b203e72ca2e07d9c8b267282daa2e`  
		Last Modified: Fri, 07 Jan 2022 02:08:02 GMT  
		Size: 6.9 MB (6930197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908bb3b2708daae4e8c3f613f3461f07d608b18560a647b4cce654f4ef141c18`  
		Last Modified: Fri, 07 Jan 2022 02:08:01 GMT  
		Size: 3.3 MB (3252123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4636f821a057f53ae57b174c8df872246b464f22b359540cc5a77d74ed2bb082`  
		Last Modified: Fri, 07 Jan 2022 02:08:23 GMT  
		Size: 47.1 MB (47067639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d4a4d531a63f36ca9d9b778f021e88bedc03615312d12bc138ae8829798e9d40
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94933984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b74a920f641c6acbe8e3557e6b0420efaa1a94b372cdffb52a99991e04d210`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 14:41:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 14:42:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 14:46:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1c3498d7cd3adcb6d716b98adcea053880272423eb1a9939a7426d428cfd8`  
		Last Modified: Tue, 05 Oct 2021 15:46:03 GMT  
		Size: 7.1 MB (7058539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494fb7e48f3a6cbd76b9eaab065228a859bdd7e6f41a24d6aa2cf74d77d31e73`  
		Last Modified: Tue, 05 Oct 2021 15:45:58 GMT  
		Size: 3.7 MB (3719778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961571b34653877509a0b15ed874ac56391305c5a20707a48fdf723b3becd986`  
		Last Modified: Tue, 05 Oct 2021 15:46:51 GMT  
		Size: 53.7 MB (53722746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c92ddca8859cefb56a0d70a1b950c78d526fa86cb474577065c230d05202d244
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79684368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21defe54672535cf0cb870511573b424fa7fb21561cac557edee34e832747842`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:01:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:01:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Jan 2022 02:02:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d51aa6028c0bcbca283acef11857a9719bfcf7c326e520202a60fbac277eb02`  
		Last Modified: Fri, 07 Jan 2022 02:11:43 GMT  
		Size: 6.3 MB (6332575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372e9a53b61e00c123206d32eb8d2114f344704896c85db85ac39b155313e3f2`  
		Last Modified: Fri, 07 Jan 2022 02:11:43 GMT  
		Size: 3.0 MB (2974983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040dba1a0049ecda923f0c6a592b103199dc490e91215e1d1ea1c78efd84212d`  
		Last Modified: Fri, 07 Jan 2022 02:11:57 GMT  
		Size: 45.0 MB (45014674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
