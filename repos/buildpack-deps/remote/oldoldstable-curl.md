## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:9a5a3f39544012d33135dc94d43b9371a6a74fb552a4654ae66555abfc69d2b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2ce1f7e3b705c7ee6c02ee6a27f0623e0669788c757fd68cf66795f700485d6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61025684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df5afae6cd998f4850662ee41db5641365d4de37cf3e23b984919303ea7cf19`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:44 GMT
ADD file:8486e54cd9c7f48cd93b4dc399b71f2053aa61655dcc37e06a9274d4878408a1 in / 
# Wed, 26 Jan 2022 01:42:44 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:16:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:16:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a834d7c95167a3e129adb00a5ddbaf5d3c035ad748ff7ee1273373d150457820`  
		Last Modified: Wed, 26 Jan 2022 01:50:37 GMT  
		Size: 45.4 MB (45381397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b3fa6f1b88b95ac6adeafdb618011e672d4c9f5637b92be373276ee7e066dd`  
		Last Modified: Wed, 26 Jan 2022 02:26:13 GMT  
		Size: 11.3 MB (11301881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778df3ecaa0fbba90d3a7d88947a4376ebdc7e2fcf8a4b5ce43b3c699faadff6`  
		Last Modified: Wed, 26 Jan 2022 02:26:12 GMT  
		Size: 4.3 MB (4342406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:af74b28d5fd3241a8f8d3e9b29ed42f041776a0dfe6e9fc34910d14fa713118c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58605294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f81a4956a429bfc7e73b642e4faa596cd544a19350c9cc8bdc53beb01a22ab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:04 GMT
ADD file:f9ce41b640f98db33431f520d66468b33575b20c5247749d76dc03214f1a92c3 in / 
# Wed, 26 Jan 2022 01:47:05 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:44:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:44:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:81c5e7cc968aed78bd97c17445dd362c3dac0397104fd90548cabfafde2c64c0`  
		Last Modified: Wed, 26 Jan 2022 02:05:19 GMT  
		Size: 44.1 MB (44091791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b75993187fe65689a3ef56f900036b8f43234e10bb71bd0afffc124ea0518c`  
		Last Modified: Wed, 26 Jan 2022 03:04:21 GMT  
		Size: 10.4 MB (10352067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa9fe1cd41c295218d445675d34d1e730babea880e423ef7417804205d3301c`  
		Last Modified: Wed, 26 Jan 2022 03:04:17 GMT  
		Size: 4.2 MB (4161436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:31de7211b000e6a93b664055488924e87877bade0494a68aeed4e08bda39a8e8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55994573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f3f6ca6dcbd83b195d6089c316e2788f4d8bbc6abb9faeb6ad85a8ec28e4713`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:34 GMT
ADD file:2d0ec7b989e0ef6e7c2d7cdfa1710507ce32d2218c0769aa5adc804e485973dd in / 
# Wed, 26 Jan 2022 01:47:35 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:49:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:49:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a4becb4205b812ec841e47cdf4840f3cd4afedb320617c1a611bd7daacd1b1e2`  
		Last Modified: Wed, 26 Jan 2022 02:05:16 GMT  
		Size: 42.1 MB (42116772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19142ccd43f320261157cec769910c598094bd2f6235ca3fb72f11ff969ba877`  
		Last Modified: Wed, 26 Jan 2022 17:12:46 GMT  
		Size: 10.0 MB (9956581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bc45f0a06bfebcf8cb3dd7f3b1577bb99c1c9a19b3dc44bab307cdd59267bb`  
		Last Modified: Wed, 26 Jan 2022 17:12:42 GMT  
		Size: 3.9 MB (3921220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:01291df860179d521e4f044e24d14c190897cb36d2ccbbeeaf9c246d259226d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57264533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef32f42e64fa081f0b445616c1245214388d0efa26eadc29d612f5effc3513f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:34 GMT
ADD file:fc57ceb549dcf9223a7806f1dbd83ede31ad1705eda04387f43795b8949b19c4 in / 
# Wed, 26 Jan 2022 01:44:34 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:17:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11cbe372cf332799e1339b2b8a04723e8224eb56d69212a1308d1df0da55eae2`  
		Last Modified: Wed, 26 Jan 2022 01:52:53 GMT  
		Size: 43.2 MB (43173725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf576a0611a8862b3ac5cc25b79aedd7b2f5a1a457ead352a467fa5b906d0f6`  
		Last Modified: Wed, 26 Jan 2022 02:27:24 GMT  
		Size: 10.2 MB (10216892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc21f7f695aceaf60c5d2590b7acb0d3937aab7af8a9470dd74605632805610`  
		Last Modified: Wed, 26 Jan 2022 02:27:24 GMT  
		Size: 3.9 MB (3873916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8ff2fecbbd29b4a769cef680f241e18cb4f5c23c78a2043d31ce3c50339ba54b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62022360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a71050bc48677b04fabc35a5491a4947f76e686e8c3e7e23f904f391e4656b0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:51 GMT
ADD file:84c4f9ca5f39d4d5afa373f2ef32d0a65a614861bd5e53fe072387283ea5901d in / 
# Wed, 26 Jan 2022 01:42:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:22:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:22:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:58d50d1151db66fec3407a887e75ea0080e2b06c23447d1aa582592c9fbd7eec`  
		Last Modified: Wed, 26 Jan 2022 01:53:54 GMT  
		Size: 46.1 MB (46097933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cc62fa793c6ec57e2be9c7b8ec84514c2c0118cdbc2b4336ee49f720fe729c`  
		Last Modified: Wed, 26 Jan 2022 02:33:31 GMT  
		Size: 11.4 MB (11359514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1167f9e9e1ee3be249d14a5d199dbb303b25457deb6ff54ac1887165400cc0b`  
		Last Modified: Wed, 26 Jan 2022 02:33:31 GMT  
		Size: 4.6 MB (4564913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
