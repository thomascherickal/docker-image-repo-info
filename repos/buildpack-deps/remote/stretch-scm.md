## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:8443fbe296f172b4248e1d8d9b5f734f1234aad5dee9aa6c997b1af5881f337a
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

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e8e625f4969cc834325843bb85a11c0736551d1dd5b2910d02ec9d7981417377
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110596973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797765de7a324f1dd848875af327ef4fbf5c64a332dc159fc5d6e60874ce12dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:23:35 GMT
ADD file:82e0eb87c6ff97b66f86c9fee44884c4cf1b08f5721f36878fc7a15a125b5079 in / 
# Wed, 13 May 2020 21:23:35 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:39:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:39:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:40:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ce7b04634a37b5c20274b3cc1469490cb28f734448d2c84d01454465418e1f`  
		Last Modified: Wed, 13 May 2020 21:29:57 GMT  
		Size: 45.4 MB (45375936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99828f061d94e903ecb427fa486d6f5876932a98b7bbe2dbeaf26d1b7a4d52c`  
		Last Modified: Wed, 13 May 2020 22:48:42 GMT  
		Size: 10.8 MB (10797470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c850eee83158cd6c3f9a0c3a52202356cce4782a6c3e17f69786722711814e11`  
		Last Modified: Wed, 13 May 2020 22:48:41 GMT  
		Size: 4.3 MB (4340177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdf93eb77fd0efd6548185bf7c7f4fa03ea8a9c9dda06ca7a07b20f5eefbfb9`  
		Last Modified: Wed, 13 May 2020 22:49:00 GMT  
		Size: 50.1 MB (50083390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6583603c8b004b9b9b94bc8b61f59a8227b01934496563dbe37600aa2bc0b101
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.4 MB (106399377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76c832ebe030c5bfaad5571ec23d07e9b6d84a68030d18d460b2a805e6074945`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:54:56 GMT
ADD file:85da223f359bde63cb0354ad866044074595630104ae55a1790b83f209585e48 in / 
# Wed, 13 May 2020 21:55:00 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:48:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:48:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:49:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e24629b52a5049ace3da69cc30167057bc65b6c050c9fe405d45685d76f1dd5`  
		Last Modified: Wed, 13 May 2020 22:03:01 GMT  
		Size: 44.1 MB (44067816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d758908a0acec534a104fc28eac5f46f7cff0b2e7d72e3d10a141c322ccc13c`  
		Last Modified: Wed, 13 May 2020 22:59:50 GMT  
		Size: 9.9 MB (9866753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccfd03f2512eb54a2aac699e7339f04dd979d0d314217d9c5522916b9b1095e`  
		Last Modified: Wed, 13 May 2020 22:59:48 GMT  
		Size: 4.2 MB (4159121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f673ada185ba56e8d7f1984fd7d09160290af02c98aad30c66617c23b100bc00`  
		Last Modified: Wed, 13 May 2020 23:00:12 GMT  
		Size: 48.3 MB (48305687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6c07c0d0a16ee2e2b67cbca43e608b5565cc5b187d9eeb759839324387033e4d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101931524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2dfa91aabe1b7a2374e13cc4d40dfea8f85c157bc576583cf19a74863b36c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:18:55 GMT
ADD file:22401e33698b1bb830736dfb4dcfcae97faee4aeb57fbc910c50a0806fb726e3 in / 
# Wed, 13 May 2020 21:18:57 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:11:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:11:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d01aee5144e594ba9bd007624dc3b8437510d15e6c34689c8475bf2d6b5c3e4`  
		Last Modified: Wed, 13 May 2020 21:28:12 GMT  
		Size: 42.1 MB (42101107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe054c42f454952057587a2811701e4d75d2373543ff044e7bb2ac01b58b9ea`  
		Last Modified: Thu, 14 May 2020 00:24:33 GMT  
		Size: 9.5 MB (9498400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c387dfbcc5dd736b7a3ff0e096644f3893be259a4dec30a1309d0374383da2c`  
		Last Modified: Thu, 14 May 2020 00:24:31 GMT  
		Size: 3.9 MB (3918743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141c54e66e7537474c859e5f9b803c8ef3c12cc787c474cbb8e9e4fa5af50492`  
		Last Modified: Thu, 14 May 2020 00:24:54 GMT  
		Size: 46.4 MB (46413274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d2d5efbe95b78462edec381abcd34718665cf8d7617945e28da481e457709f54
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105036255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368aee20debdb765a73bfab3a928e9f8a09a0a4ae0f0da87a88c02a09dbaa0dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:47:38 GMT
ADD file:e7776aac0b87be303e31e5947db89f835a4e17175e339ec23becf5fe4a9548a5 in / 
# Wed, 13 May 2020 21:47:41 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:32:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:32:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:33:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0480c895dd1d5b237cb931426f18706cbe8dac16e19ed583f3010f3655094efa`  
		Last Modified: Wed, 13 May 2020 21:56:03 GMT  
		Size: 43.2 MB (43158976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cf6474b5cce4b1c7c8d54d2c80e8db074f4c5d89471a009859e0c318ac7d76`  
		Last Modified: Wed, 13 May 2020 22:42:35 GMT  
		Size: 9.7 MB (9748540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f97c7d6d20cb6dbf105d3e25bea385e4b74876e9fcd4cbd49ac0e5b30c69c80`  
		Last Modified: Wed, 13 May 2020 22:42:34 GMT  
		Size: 4.1 MB (4094379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3166282442cd611f517b83932715119560eac9ad53b1356b6377568687f87a2a`  
		Last Modified: Wed, 13 May 2020 22:42:58 GMT  
		Size: 48.0 MB (48034360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2eeb05402d54e0d302c8a4f7b186ae792c31c10b1268919ddbea569b4b7eb721
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113091253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d20f0372fc295640b57a2577dc3368bb0a675b18d4c2c4decb8ae13ecd348dce`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:23 GMT
ADD file:0d501ab6846646b4793ce31bd08a81ee75bf7ca50e44fad4f41d38ea73217f94 in / 
# Wed, 13 May 2020 21:42:23 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:56:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:56:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:57:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:738ccd27fcd21d91d1826e5bb5ee29ef3a82a770de7e1407c86b04395fdd1335`  
		Last Modified: Wed, 13 May 2020 21:49:47 GMT  
		Size: 46.1 MB (46095041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82205e09585e2a065853d934b8b472473745ad9b5efb22d99c6058389714f39b`  
		Last Modified: Thu, 14 May 2020 00:06:36 GMT  
		Size: 10.8 MB (10818400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3797adb63c6052aa7506f3676edbac22d3e2c0f54ee7d52a3d9457de30b41e4`  
		Last Modified: Thu, 14 May 2020 00:06:34 GMT  
		Size: 4.6 MB (4561500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0080f1b328cb6563f844483103df9f1ccb13092859d03f61682cdd0a0cbc02`  
		Last Modified: Thu, 14 May 2020 00:07:03 GMT  
		Size: 51.6 MB (51616312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:860601868f5a4b50f829f79682e50ad65c20901371a3a528f1241e2042dd97b6
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.7 MB (108745578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107bd4c13957543f5a5f1ad377616397ea7e97ae0e98b50bcbcaf56ea2b5db76`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:52:06 GMT
ADD file:7bf5ef3df2c7fedfe3177de091f107679e7882507d08882b3203eff7ac42da5b in / 
# Wed, 13 May 2020 22:52:07 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:06:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:07:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:690bb78d0f5d6a469cf42f228761b11696fe51dbcca8ec4392ae892677a415b6`  
		Last Modified: Wed, 13 May 2020 23:02:33 GMT  
		Size: 45.0 MB (45048775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7defc0f982fc7a60239b6792c0bae2cf47b26cdf0863043492bbba235b9f0035`  
		Last Modified: Thu, 14 May 2020 00:23:25 GMT  
		Size: 9.8 MB (9826324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f70cc1cb7d757de66211d78d4b389425f5ae180b0ccea6f03fecbdea3dd5619`  
		Last Modified: Thu, 14 May 2020 00:23:21 GMT  
		Size: 4.4 MB (4394839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d29d67ee359ca0802370c893123f53ab51312ad79581f7da8055d95e364e0`  
		Last Modified: Thu, 14 May 2020 00:24:16 GMT  
		Size: 49.5 MB (49475640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:29da8a63cf35fa0e373e78683ea697d733d91fc6727c9b28b1183dec703c05ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110026709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b93600833a7d838c146a1ad78daf95df52d8d3f9593e8ff62e9848b82c856a8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:39:29 GMT
ADD file:fa4c7e3ca04f092e53cc791a32c929663412df3f68de2733bb867053577bf1d1 in / 
# Wed, 13 May 2020 22:39:34 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:10:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7732483b686efe14a1cf8add89a1568b83892e243798fba30808f1fc6287210b`  
		Last Modified: Wed, 13 May 2020 23:02:10 GMT  
		Size: 45.6 MB (45646193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df33ef5c6dd4781defd528815174987b67a617a4fbddd5e5241a2f67a34098cb`  
		Last Modified: Thu, 14 May 2020 00:37:47 GMT  
		Size: 10.0 MB (10002565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02507bd450f72bbb529f56f9579bb7169fc9be7900bc5b9b0587e4855e51ad8d`  
		Last Modified: Thu, 14 May 2020 00:37:41 GMT  
		Size: 4.3 MB (4296673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a5abe5a03ebb35ed027af57237427bf1650677f1d4c6a907f88cf889b5e403`  
		Last Modified: Thu, 14 May 2020 00:39:16 GMT  
		Size: 50.1 MB (50081278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:10d7ad57461578de472af15cc7e041415b559c4d83f84676d087d5c48394a932
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110442091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cfc571f2635047825ecca94e7131f84d3b95cfd70bbb3a896494c83e608005f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:44:18 GMT
ADD file:80db5381a461bb249455c6e92a06f91a777c0d8db654106cc55f91d6252c3c44 in / 
# Wed, 13 May 2020 21:44:20 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:43:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:44:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:44:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd38adf1f4e3b358b79e0f6559fa135ec376d7abbcc3f8bf0b62a2d19d972cbc`  
		Last Modified: Wed, 13 May 2020 21:48:31 GMT  
		Size: 45.2 MB (45232705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b7499c91144099ccb386aa415835bab026fb0216cd29e9e2b0ef701d9f9edc`  
		Last Modified: Wed, 13 May 2020 22:50:12 GMT  
		Size: 10.3 MB (10325615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89032869e1382e045958dbcc66285bcdc50c4540833a40f19b218759847548a5`  
		Last Modified: Wed, 13 May 2020 22:50:11 GMT  
		Size: 4.4 MB (4372600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40a216015c652fe4455523b0c4b2447eb65f5f5c502d88b116fe834e2041e7c`  
		Last Modified: Wed, 13 May 2020 22:50:26 GMT  
		Size: 50.5 MB (50511171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
