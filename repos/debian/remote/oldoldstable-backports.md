## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:f3044ff79015e592ff2c01a77c7d2ed594f606c5a71c9b3f806c05e961da050d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:e99c785c67deec8faf233f804f7b18d787f9f2851fc39297d0dce7e0ca5ff435
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45427687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:096abacdf3e787598a4806f906f8e321342157d38343d4fd281f10e655f8968e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:57 GMT
ADD file:91c1b90dda98c0f3328e5c763b36b29831467c0a0cf52df5359551154d2e6355 in / 
# Wed, 20 Apr 2022 04:43:58 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:44:00 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d195d42244aab04cff1a0e88441cc5fd6954f65abf0514e85b72d7c4a631445d`  
		Last Modified: Wed, 20 Apr 2022 04:49:36 GMT  
		Size: 45.4 MB (45427461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872d25904c5d3caad43216df724674640e8d212683e520aa153dcc575450739e`  
		Last Modified: Wed, 20 Apr 2022 04:49:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:22a23b548de996a944d14de8f21c6ed272bbbdd00a07bdd7a655ef22608e1f7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44122930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66336408614f60d2352905373c02e766809b5c841c75a3c11a001955f1c247ed`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:18:16 GMT
ADD file:e9d593b94101c656c0e16180bbfd484731d77bff96a72ddb0c9434a4c47d574a in / 
# Wed, 20 Apr 2022 07:18:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:18:29 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:011248ff897363bbfbb6391be232b1fe34d171c43e4402a37d13bb16665622b4`  
		Last Modified: Wed, 20 Apr 2022 07:34:41 GMT  
		Size: 44.1 MB (44122702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3562a03d0a7e26b75f2bb976b97802db99261413529365b6568934c8c2991089`  
		Last Modified: Wed, 20 Apr 2022 07:34:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b9bef32dd514404f2a8e56313e36b20d3c83ca4f76e9626661c7dd5148afa65c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42151358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba884bdd9ec69ba1af654f45cc5ae00b7b4dd7bdc974ab76bed21aaef3dece36`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:20:08 GMT
ADD file:82cf2a47571e24e1fe3a28674406c1f33e8601d4d4a324875469e66a84891f49 in / 
# Tue, 29 Mar 2022 02:20:09 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:20:22 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:824a32552e1b3d7fc60d23dfc4c18c7490430bb3bf5a3b2d8351f0b68e43cb40`  
		Last Modified: Tue, 29 Mar 2022 02:36:08 GMT  
		Size: 42.2 MB (42151132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79db98e1060c96479b9dbebae9db8ee6a588e618fceb77e3b65c0e362fcae6cf`  
		Last Modified: Tue, 29 Mar 2022 02:36:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:a99f13b8cb03897ae7b3f384bdf5d77d91060837326b3e956a6062d556e74af7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43212265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709ddd6fce1f7082cb9dd79471ed6d039d554ed669911e1f2f12a8c5a258b00d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:47 GMT
ADD file:6eba819e0e2efda877840d26ec82d97b5cc971ac347cfa420006e49d98af40da in / 
# Wed, 20 Apr 2022 04:29:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:29:54 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3f84d18376d0447d1292f58ace6bd0081a20c00a2682f97974e0bb2caa786dab`  
		Last Modified: Wed, 20 Apr 2022 04:37:01 GMT  
		Size: 43.2 MB (43212037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c10697208d9361ae5b3cc2f57693c758f3cf4c64ed56e86cedf5170c57259`  
		Last Modified: Wed, 20 Apr 2022 04:37:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:1a489638f5a66d02fb515f6586fdf06b508045d490a7adb74a4115409c890820
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46147958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c875f15cb642d65332b4add4022ecb80c3568415cffd12c64135406cb2fb448`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:16 GMT
ADD file:5c34d7058c53f0327bc7b12fc42fd6e752870d7b5b982bad1b9e9d0894d75d04 in / 
# Wed, 20 Apr 2022 07:38:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:38:22 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:79d3d2a2441cfff5e929e595c3a88d3e53fe158136cd9b6443fe762ef335980c`  
		Last Modified: Wed, 20 Apr 2022 07:46:10 GMT  
		Size: 46.1 MB (46147730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ded3c2b5a3a6183ee4bdfc5fecde2a7e759750bedfc100ed008b97a2f26551`  
		Last Modified: Wed, 20 Apr 2022 07:46:20 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
