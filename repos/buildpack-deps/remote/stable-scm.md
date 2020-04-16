## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:18896de4d3b5ced7ea1142f56982fe34e3db00af3b03a46e09414e450027b4dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:stable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fe41ee6c22e87c913da813d51e44cf3faa157cad052dc9cb8fd0588b12beef74
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120018204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e513ce6f01b146831a89ca8c8de67b78ffb9ad480ee6f30beb8c090528d6d76`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:03 GMT
ADD file:a0c8e81c4c7fa85b43d4a9daaed7ba25964a0bf494711b6911cd4b7f5201a17f in / 
# Thu, 16 Apr 2020 03:22:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:00:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e2b2a5af8f65687add6d864d5841067e23bd435eb1a051be6fe1ea2384946b4`  
		Last Modified: Thu, 16 Apr 2020 03:31:27 GMT  
		Size: 50.4 MB (50382957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b6f03ffac4cb4e42f8ab0bfc480bd3a3fa20e1ddee37784db63bc886b0cbb3`  
		Last Modified: Thu, 16 Apr 2020 04:16:01 GMT  
		Size: 7.8 MB (7812113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f0c679f0f4c39597721c1df5cdb4f9685b26bd789a44eeb406835a1800d5f`  
		Last Modified: Thu, 16 Apr 2020 04:16:01 GMT  
		Size: 10.0 MB (9996327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4b47407fc30b8206971ec60f280b107b00df8007da2fb912ebb8656b53695e`  
		Last Modified: Thu, 16 Apr 2020 04:16:23 GMT  
		Size: 51.8 MB (51826807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fd8c3ce9709457e2bd6bde4f742b024ac873c88594a9ccc2b17aed6283b0318a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114675138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0177d13e53c62c42266ae8fa13e549cdd27dd10fa46711efece3dc9dfd91574c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:32 GMT
ADD file:a72a8728037d512b79dddab73bd0df9cd4ac56f51fb9f5f8f92cd0814ab43c5f in / 
# Tue, 31 Mar 2020 01:24:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:24:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:24:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c37639eaa7e0ad121e7d329798e6c27a345dbc864d59dec4f04446a2c40e819e`  
		Last Modified: Tue, 31 Mar 2020 01:32:42 GMT  
		Size: 48.1 MB (48095724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f87c19604cd8bfe32a8092d64433839a11077e2602dfd6e6f5dbd9d1f8f2d8a`  
		Last Modified: Tue, 31 Mar 2020 03:47:12 GMT  
		Size: 7.4 MB (7358987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4e7c27f7acd110a2d7b7ab9f59d4f00ec1be6f6901751dac4ce0f170bc1244`  
		Last Modified: Tue, 31 Mar 2020 03:47:12 GMT  
		Size: 9.7 MB (9687046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d074bdc44f55deaca5b5a75768bbf484abf4a9c2be35396a1a775d8f06901644`  
		Last Modified: Tue, 31 Mar 2020 03:47:37 GMT  
		Size: 49.5 MB (49533381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fe48f3fcc4161f2991c99a4d51918dbdacb0560b638c5cda081f9f368278cadc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109647997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842b565b25ecaf31c70d97680e2a5bad583150401c73aa7c6492d9fe9442da60`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:14 GMT
ADD file:c2369e5669e570f90abaa1fd4fcea4ae1e6654bbd81e8fa070a5b2484c03ee74 in / 
# Thu, 16 Apr 2020 00:59:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:38:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:38:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:39:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:020b29c91094d59c5eb128b7bc2b0b835e2ba4414358664e467428fe8b95bf52`  
		Last Modified: Thu, 16 Apr 2020 01:08:38 GMT  
		Size: 45.9 MB (45864371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878eece65f73163f26e0755d7bf2d0280b635e9354ee5ac677dd0e1c3b9f485`  
		Last Modified: Thu, 16 Apr 2020 01:56:53 GMT  
		Size: 7.1 MB (7096553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070c5585774beab3cf31d2f66df886bd4295763a00c5f013aab32f261a9559fb`  
		Last Modified: Thu, 16 Apr 2020 01:56:53 GMT  
		Size: 9.3 MB (9343267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e454adb17af2402de86f3b7834eb2d85a7ab8d1199be3963a7ddf802e25a5480`  
		Last Modified: Thu, 16 Apr 2020 01:57:17 GMT  
		Size: 47.3 MB (47343806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:35df78d052ae0b0946f924be1366a1236253e3ba38745a08100146e18a4eda0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118990678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e78c0a35174992b27b59bd5b6f38a7a0cd6c50de5432443679bf6dbd52889ec`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:20 GMT
ADD file:02afb66e938cbc67271aaf8cbee75def87458a21d961d02e86383e0ed36b0c71 in / 
# Thu, 16 Apr 2020 02:41:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:13:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:13:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d080dad46627d4103daddf54c89f2ef0a0b72ba8270066c50e95ffbf4a79362e`  
		Last Modified: Thu, 16 Apr 2020 02:48:36 GMT  
		Size: 49.2 MB (49169521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c76f347939ef96b2815e45f9fa43995940a8d4a01525012b2bce1adcbfc3a`  
		Last Modified: Thu, 16 Apr 2020 03:27:53 GMT  
		Size: 7.7 MB (7681332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b6b37aa5fec6dcadc18e45dc6d58e4cf4b967540152c4f44030737e2f5351`  
		Last Modified: Thu, 16 Apr 2020 03:27:53 GMT  
		Size: 10.0 MB (9983908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0caa3b2294305ed3cf1d91d1fe2e2dbf3e294a694a4f636dea6bf733975e237a`  
		Last Modified: Thu, 16 Apr 2020 03:28:16 GMT  
		Size: 52.2 MB (52155917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5a119ea7f354719d4704db92e90b664a9dd7752afbaf0845e5a2d0c3bd13502b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122890572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31480e12b660496371aa78347efaf2d1dac7b5f30b81ae1b3bff67f29903ef77`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:37 GMT
ADD file:9a9b9c1d98dfe76e20b3ed67b866e2bdbc1095e26de13b892d07f2a3ee062c83 in / 
# Thu, 16 Apr 2020 01:39:37 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:18:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:19:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a29df432ebf22a237e5e0940a65a1f908be66a5204c5ef240ead7315c27335f`  
		Last Modified: Thu, 16 Apr 2020 01:46:01 GMT  
		Size: 51.1 MB (51147069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec62877ba52bb13d1e47ca6d0c47e1e0d1c61598a0ff5c3590b28c93b2718c3`  
		Last Modified: Thu, 16 Apr 2020 02:37:17 GMT  
		Size: 8.0 MB (7981604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab3373b511919f98b91c8b654596e531ed2f4612bf5b9d63614e0aa420ee01`  
		Last Modified: Thu, 16 Apr 2020 02:37:18 GMT  
		Size: 10.3 MB (10338497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80102fc76b236a12f5fdd11396159f29e8b9567c8c5a159b09b8dc46fc9c003`  
		Last Modified: Thu, 16 Apr 2020 02:37:39 GMT  
		Size: 53.4 MB (53423402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f65a71835cfc34fdf8d3b5b36e1f2576182410b528f8b93a1be33e73364dbffc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130509348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d05f126990da65de2f1892cb4149738f6c89e6e222835b336b331a44591ba3fc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:00 GMT
ADD file:ccb86d1c4380ce5c6d0f26560ca6d637d15f7a9dd5a3e56977bcf80edcac69ac in / 
# Tue, 31 Mar 2020 01:32:04 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:17:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:18:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:20:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ee2adf89ee904a62d0e8993a1c564c340ff8a0d3ae152066c13e15fbae902ea`  
		Last Modified: Tue, 31 Mar 2020 01:44:47 GMT  
		Size: 54.1 MB (54138582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7915606b477e202ed2b21747b3be7759d7149f3196e41b5fb1cf369c4de0be`  
		Last Modified: Tue, 31 Mar 2020 04:01:16 GMT  
		Size: 8.3 MB (8252489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbb0da6a42dc57d1f7b6790ad807eb7769963d865a7fbc93c11ad41ec9aa16`  
		Last Modified: Tue, 31 Mar 2020 04:01:15 GMT  
		Size: 10.7 MB (10727214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4349e78867844cdb6b83633fcdacb72c4290b5d7124f9e8e94ea8c947dccb`  
		Last Modified: Tue, 31 Mar 2020 04:02:06 GMT  
		Size: 57.4 MB (57391063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e869e0adb64b910253dd6808066b06af738b5242c6a4b255298c386453d63fac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117595274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6e7ac1c744fc6535921a35d804e0962aeab4380fa2cd8a95441b8feb1e4be7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:03 GMT
ADD file:26367817216af13dc3ba9f495303f7bee8fe138fc8fb728289781563308ce0bd in / 
# Thu, 16 Apr 2020 00:42:05 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:58:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:58:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54e2fb160a5d4a95ec7efe70c0045923ee557e87ee68ce03f2150b8366f26729`  
		Last Modified: Thu, 16 Apr 2020 00:46:03 GMT  
		Size: 49.0 MB (48960213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f0f1e0f91312a55967b48addc24054fb2e7fb63926a621dd6e86ea62aff2b4`  
		Last Modified: Thu, 16 Apr 2020 02:06:25 GMT  
		Size: 7.4 MB (7382082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7ce4aae52f7ba529ea00a3a1bfe7656e52dc1d8b0168a3d70b4e0a4392989f`  
		Last Modified: Thu, 16 Apr 2020 02:06:25 GMT  
		Size: 9.9 MB (9882086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5250b872c2e5d6fcb26d734d43c62187b594e1ce80d34f0cf57fd5e3666b8f`  
		Last Modified: Thu, 16 Apr 2020 02:06:39 GMT  
		Size: 51.4 MB (51370893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
