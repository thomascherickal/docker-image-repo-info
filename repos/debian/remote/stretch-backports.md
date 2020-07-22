## `debian:stretch-backports`

```console
$ docker pull debian@sha256:3027ad55c28450214ba116f7a36c7fa966be3d8803a57098734ca31c0e9751da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:03ee996b9719ea682a12b5385c3a93c103a9c93d41cdd44ed65fbb19131b8b11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45369896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52a14ebc3ae213213285ef6527255bf8a067758959c810d1fe60b05636f041e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:06:48 GMT
ADD file:f98fe3d719ea765cb59da025d506d0bbd6db7a842b6b63c58c8d4d65b51bdb1f in / 
# Wed, 22 Jul 2020 02:06:48 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:06:54 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7e6d8ed603557d9bf077a9ace4ee506501970a4938b9a704f040ad15f22bd4e8`  
		Last Modified: Wed, 22 Jul 2020 02:12:13 GMT  
		Size: 45.4 MB (45369674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6954bf97a51499d1fb263895c04fec70a7aeab331825e2306b94eeedf7af4e3`  
		Last Modified: Wed, 22 Jul 2020 02:12:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:9e6d757f85e94cc6c0d349bc2950558a06dd8e2fda5c5fc41d25df47415f28e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44078507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:246cbbae44c78b204d86939f9a7921db3c6db5b44c6fd2cff405f6405b550e5a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:54:50 GMT
ADD file:20254f5b25d60e6c982d1c79c039231162bbcd4f257bb6abffd80fcc90989150 in / 
# Wed, 22 Jul 2020 00:54:52 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:54:59 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fd4c1ca2ea2c633172981c07bc3fa277bf52eb9dbb1010857e651754055dd468`  
		Last Modified: Wed, 22 Jul 2020 01:03:05 GMT  
		Size: 44.1 MB (44078283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf3748aa39317034a3486a092122bd0e4181c8a8f7fd4dc4f57ae2e9d7d8e1`  
		Last Modified: Wed, 22 Jul 2020 01:03:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:cc6902738365971880c0d4e514636dd0cb103fc937907ec4a1913fa7dd7f67e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42107703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09124f4a69e37c240c3131c9cffc86072b80f36c3f134bda30ba34923fe0dc01`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:32:02 GMT
ADD file:762e52a5e1d8ff2daa22c3bec2cfdfe4cbcf224deb1e73d7db3af0cbf5658785 in / 
# Wed, 22 Jul 2020 01:32:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:32:48 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:05dc12a0df610a09562914533797508b791bbd115ae17b6a1b75666ec90263da`  
		Last Modified: Wed, 22 Jul 2020 01:44:04 GMT  
		Size: 42.1 MB (42107480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21d2756afcaf6a2c9d48b4cc7f05209dfb4fbd4c3f51ec519ec2a0c4b6e3fdd`  
		Last Modified: Wed, 22 Jul 2020 01:44:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6ec1d3f27e4e583894448c96bcc55cbfe80accf013ea263a88ed97c7619466b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43169630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f501116ecd90063591421ddd06a837e4eb32891e909939a383f1c25e3ffe4993`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:43:42 GMT
ADD file:9c5c9df9952cb51291333837bdb462bbdf9f157e91e616f1e3fb8d2fcb1a1983 in / 
# Wed, 22 Jul 2020 00:43:45 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:43:54 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ad4de4f68e9c2c0f5e5e62d379d936bb88ce467505ed002fb1e10c434fefe90c`  
		Last Modified: Wed, 22 Jul 2020 00:49:52 GMT  
		Size: 43.2 MB (43169407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167ee6e6df70cf9862116173bbe4240fa5fdfaa129a95bb5d758f8ad1e78d06`  
		Last Modified: Wed, 22 Jul 2020 00:50:04 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:3721492c8ffa9017dbbacc4a6352da19b4beef269637a9f2b1f40e505a349aa9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46093221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad9ca71fe495994d749ce90711fa594893521f4a6f9c887c8eb5cb90dc5841b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:12:18 GMT
ADD file:d3f4f838251f30bbb4c033600c18e4c1065e310959dc105d22c6df709decb369 in / 
# Wed, 22 Jul 2020 02:12:19 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:12:24 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:48006630f132977bf4db68efe0ddd39191244134bb38b95a1c28b7cc6ce01157`  
		Last Modified: Wed, 22 Jul 2020 02:19:12 GMT  
		Size: 46.1 MB (46092998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7905611dad7a05f7f291a1c3eb1ec551bc13e0119fc3fc04bd265f5b882da448`  
		Last Modified: Wed, 22 Jul 2020 02:19:18 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
