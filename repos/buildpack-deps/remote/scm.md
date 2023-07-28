## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:c6e4c95967f67486cdf8b363c4e68bb5a7b7c72b3fa1a8eb50bb765198483b84
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

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:529e163a2641648602b7c30f6628836a07309db7eec36b54bc1f3079fe1a0075
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137700186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:612d62ca1b84af9b3c9ea7d4f8f7451dea5d5280997f2995f5a5476d50e65656`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fa3c22ae74006b877a8e927100f62a8425ed6c059db37367d5a38c434687d59c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131678797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67dd402f7ea7f634b30239e8d28c21bda53cc96ae3fcfae29987eaab76ccb902`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:21 GMT
ADD file:7b6666a92b89bab40a1b4dda36930e1b5a7b9ab40ac8dadd2179767e027de097 in / 
# Thu, 27 Jul 2023 23:48:21 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:882ddccdc867712377829e4abe9ddf1190166c3dbdfc4cee67aafb08e253cc1f`  
		Last Modified: Thu, 27 Jul 2023 23:51:04 GMT  
		Size: 47.4 MB (47414939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f253718c89752af3d3827fa9e08b951a2eeb9e7fb65162096eff9684d21a4b38`  
		Last Modified: Fri, 28 Jul 2023 06:25:10 GMT  
		Size: 22.7 MB (22709706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54a2e1f4e1f80c2371c6fc46dad3133af5078cb0653caed09e33a1b64063c79`  
		Last Modified: Fri, 28 Jul 2023 06:25:32 GMT  
		Size: 61.6 MB (61554152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ad9f6f3059df25e76fcb798e3008e81b1463eb1f88b58eb7ac40eac428262366
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126431790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927d152d21166d702bc67a564e7d95c38acbe78275a23b81f2dcadf8fc1aa619`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:57:34 GMT
ADD file:be1c9c3d1025b24193774f5c0d5f790387924ed669771b461b2c599068512dc5 in / 
# Thu, 27 Jul 2023 23:57:35 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:57:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:58:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f76b23045cf894a3a989a9812af93c6b2eb7169116a938d01b03e6856046fd3a`  
		Last Modified: Fri, 28 Jul 2023 00:02:46 GMT  
		Size: 45.2 MB (45232980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc5ca91792613eb694a9a6a96dea7fa075fa3d9bf6cd91997b3575293631923`  
		Last Modified: Fri, 28 Jul 2023 02:06:30 GMT  
		Size: 21.9 MB (21936835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41630b85b67c30afc21e9a68ad3a0b59c168c1955785b07d9f581d53cf5fa22c`  
		Last Modified: Fri, 28 Jul 2023 02:06:49 GMT  
		Size: 59.3 MB (59261975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:884232595c8920b7cbfed7fc11b6cd00b0511c7139f19a0593f2754ed0b4e6e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137149696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c369265734f2a0f30a94ea509e82f8ae0356b341ab526bd9c79f007b9e6458f6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:42:51 GMT
ADD file:fa545fc37115e874135945921d2cc72df8dc5b16d4354b2052717c7a57043e0d in / 
# Thu, 27 Jul 2023 23:42:51 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:36:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc9ce7290e7e014f69623715ba619a0d3488a7b6ecbf09e55e11160365691192`  
		Last Modified: Thu, 27 Jul 2023 23:45:54 GMT  
		Size: 49.6 MB (49591268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73373011d63f722a4ac6bc23ce7831a17f19e27ef530544642f060aa1d6b028b`  
		Last Modified: Fri, 28 Jul 2023 01:41:58 GMT  
		Size: 23.6 MB (23570127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dafffb02e2671e7e5cc07c996fed89f6ccc8e3276ce2dc1bbfb81502cdd795`  
		Last Modified: Fri, 28 Jul 2023 01:42:15 GMT  
		Size: 64.0 MB (63988301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e93d1e1d0a091272e88d7d8bf0e0e21b3df095765d52c1007b9bbab8d01069f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141404445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d40934ac087de93ceffbf81437543947fc9c9c8b8184568346ac03da80f35bd7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:28:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f685d713d76bdc0731a917b074d79f3de7c84bfe09c53585642801175a72f`  
		Last Modified: Tue, 04 Jul 2023 05:38:34 GMT  
		Size: 66.0 MB (65972310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9e6b325e9f83cee376fbde36a72981f811fae25c545e31c8915da5654dff04b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136105543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b95c96798319d28a7d61e576aca883a6bd72c3ba77b41f8b73169a8976c95c09`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:13:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fab0a49ca1e0cd2eb4b9660e3a70dc1ab671984cc4843ea845a6cf76532eaa`  
		Last Modified: Fri, 28 Jul 2023 01:32:19 GMT  
		Size: 63.0 MB (62950846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5dd7e0c399d7c2e1caffce633e4a61612e952da52ecbea4a157bb64b33c9217d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148794670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e832d07020b4ac561f2b7991e32781a0d9bcadf847e6b3f9dee41ddb482a3e67`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:22:41 GMT
ADD file:b20300808df8e1ce5b5ff534088c39d6b04467476af024e54545f7857f78a508 in / 
# Thu, 27 Jul 2023 23:22:43 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:48:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d31d119ff78cff1435e4eb51d8918916c2d5057cebf12b76d5352660fb90de`  
		Last Modified: Thu, 27 Jul 2023 23:28:46 GMT  
		Size: 53.5 MB (53543346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a33abb1f7b6ee01625f07108e25c720832ec763cb926abf676b8841aeff7a3`  
		Last Modified: Fri, 28 Jul 2023 01:59:03 GMT  
		Size: 25.7 MB (25680980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b3b1ad4b6d7fdd0b5ed658423ee70f16882053f8cd775f5234fe8217ad8a4a`  
		Last Modified: Fri, 28 Jul 2023 01:59:35 GMT  
		Size: 69.6 MB (69570344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fe52fdb7dfc1097fd196129b9cf64eb9d39e4dde91b2ce0f7f7cc1301c482e63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135063525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db3ac5f048464fd046388417ced0450bc6bbdb078b9de300cbfdbb2aa3757d9a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:46:54 GMT
ADD file:7cc985c20b5bf9e4dde7f388e4a49154bad3005c95f50de92b01ecec9212e022 in / 
# Thu, 27 Jul 2023 23:46:56 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:55:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:56:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93e4b40dfe5599c220b1b5acf9563fe87baf3eaa3fd2f0df5e8c0c6640a9d9ff`  
		Last Modified: Thu, 27 Jul 2023 23:51:59 GMT  
		Size: 47.9 MB (47922041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c098e736df62c7c1ec5d7910b09ebaa881acd0aa44d8c82aae2beb615c5fa8`  
		Last Modified: Fri, 28 Jul 2023 02:02:18 GMT  
		Size: 24.0 MB (24028836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a0231d345104262f6b9c9131e53bf2671fb787b9a070f6c1eafb65fa6561a0`  
		Last Modified: Fri, 28 Jul 2023 02:02:35 GMT  
		Size: 63.1 MB (63112648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
