## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:62e2d72e1d7255b54bf32f0f65306ffecf125e14811a69a6a852756452e25b64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:0bd4376852fe7dd4be7bcd5c0d5a0737d205f341724b3261d76bdf298b385039
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45367056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecb2e9ecc0fad6c047a6cf3d15d8bb7a4ebd6138ac009166cb1636c702ee1846`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:22 GMT
ADD file:bcea61d1dd734cca1b40957f8d1a3375c492d03243f6bf357d95190f932de0cd in / 
# Tue, 13 Oct 2020 01:41:22 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:41:29 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4ac0e8e0794399795fdd57c08754f1acef3461c6a7f55119ee62fac51de72c31`  
		Last Modified: Tue, 13 Oct 2020 01:49:31 GMT  
		Size: 45.4 MB (45366831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6d65472d71eb312b7724560c5d230db58cbbe5108d98b1ad9d006855c6a9f0`  
		Last Modified: Tue, 13 Oct 2020 01:49:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:08f0d1894ab9c443729ee850c27871144786d083d8357f91d994ca2560b9dfdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44081123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d949d840c3767cdae81592088eff9bf4689a73457ffbbf12f39336012f104f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:54:47 GMT
ADD file:a7385db42331f3ba3cc34634615cbe5510debf4659e99c5d7f24bb01c65cb55a in / 
# Tue, 13 Oct 2020 01:54:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:54:58 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ed98f31488aa671bd837996cd22803d3c1bd1182fe80768d3d8c4e196a30de15`  
		Last Modified: Tue, 13 Oct 2020 02:03:12 GMT  
		Size: 44.1 MB (44080895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77cd76aa6fac2b99f31a9a70d8680318a7df50f2da2bf0167adea3c89958229`  
		Last Modified: Tue, 13 Oct 2020 02:03:19 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:222d4b31b7cb9e4f5a3cd5ad501111abdfca2b946850c4d786f9d16fb199215a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42111524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e6fb338f8193accad5c08733c224d92e0b450fa6bda531dc0918c9160929579`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:01:31 GMT
ADD file:ba37e605abc79a05314cdeef7432f7a2ddf10e2d321aec9eb0d181c5a23c0194 in / 
# Tue, 13 Oct 2020 01:01:33 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:01:43 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a93818213293753765398b7ca12808d535714631c0bc32c44ea0de77bd41b0f3`  
		Last Modified: Tue, 13 Oct 2020 01:10:25 GMT  
		Size: 42.1 MB (42111298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50aacf45de4e513564b6d5e40acb41d34bd64910b3da88e38d4674d49bc2b679`  
		Last Modified: Tue, 13 Oct 2020 01:10:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c8f1a061a2de809fdc61d4b288c5bb4e5d1e7762804bd2ca8f63d09d1562e2c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43171754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18a0d8504d547be7778cffba216d5e8d38dd9ffa58a082c7ecabe85c2491bfb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:29 GMT
ADD file:386b399707c44e5819309af04b42bdc2b8f02bd4e473872d66b5d0122bb87a4c in / 
# Tue, 13 Oct 2020 01:41:32 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:41:40 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b314f6c3e34f93f010f1b24227675624bf5f1c8acd6d69f18ebc3f5d1535af99`  
		Last Modified: Tue, 13 Oct 2020 01:48:38 GMT  
		Size: 43.2 MB (43171527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7091c440b9b4fdffc775653d7544db0115cc7d794497f0ea818a4dabf51c6d2`  
		Last Modified: Tue, 13 Oct 2020 01:48:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:052d43aa3e9148f5cc7754af3f0e9a58d04e511182561afb8f50b06010475122
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46087138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:260c052e37f9a0dbeb7a445c9b362c948dbd3c6cef316a91cff29e3a3101b179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:56 GMT
ADD file:58120550e3aa9316082ca03291b19f3b201dca109dc6b916dc95ae908d7853d7 in / 
# Tue, 13 Oct 2020 01:42:57 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:43:02 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:088e036e5462e5867d4128e7297b790c77f1115327066c2afe8cb82cec8c8f97`  
		Last Modified: Tue, 13 Oct 2020 01:50:20 GMT  
		Size: 46.1 MB (46086912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa8cc6a3889501d3ec51226c7176186c1503a5d8d696c114b48c17beed9cc17`  
		Last Modified: Tue, 13 Oct 2020 01:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
