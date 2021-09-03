## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:58becc620c11b09f22a686b57f2625113e8fabc7fab65e1715a39a1c6f860d0c
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
$ docker pull debian@sha256:f55651e529a2f2d5c9aae4e2044d4fb50c26091d9b0960e81233b3c35b7442cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45380043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c9924a2ed888998df2a50133c2f7b55cc9e976f5bc28fc5d6f841ce1b59370`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:56 GMT
ADD file:75734a6ee48a4bc372f5f8248122afb6cd68c590504c1ea83d4afab2bdb2ab10 in / 
# Fri, 03 Sep 2021 01:21:57 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:22:02 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ce4fce3b6196c8a662df9f0e183e951249557c8912709fd009eeed4eb34a986d`  
		Last Modified: Fri, 03 Sep 2021 01:28:41 GMT  
		Size: 45.4 MB (45379817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2f1a75d5bfaf1267ae93eda830432fea989d274e35cdd51472efbd60162c73`  
		Last Modified: Fri, 03 Sep 2021 01:28:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:1256469aa6829781722ad64bbb67cf40ee2a10208f8141274aab6fb82e968fe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44091957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a355ceb4c9fec69ab1c5c4a2582aadc00618c0c10dd96a92655bb64cdcd9de8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:52 GMT
ADD file:27ed42fc2ceb6451112e35a4431f6bb2660940f226fd39db753f55d549f145cf in / 
# Fri, 03 Sep 2021 00:51:53 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:52:05 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:04bf0e1d74bbf79d6ef345a738d12610248a308a8efdefae6cd6152dc47241f0`  
		Last Modified: Fri, 03 Sep 2021 01:07:59 GMT  
		Size: 44.1 MB (44091729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a02ec2f784c9aca71d0731992e323e321d30608b33585adbc7c3b928f66e60`  
		Last Modified: Fri, 03 Sep 2021 01:08:12 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:6a6f87191e1eb9b2db73db011d28772e0fdedb14abd6eb13ff7dbb8ea9ae9610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42119781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27210cb7c2c2f2a0aa816c446e2244f9a28051687ed7ca8573e4d4740e5b12bb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:01:08 GMT
ADD file:94eb1749d95a7eae8a82c5397a1176b1ed49fe5850d139a7393e9b55d258ec41 in / 
# Fri, 03 Sep 2021 01:01:09 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:01:21 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:875d7ff68cc6cb195e710689c421f6c8432606878e0df2b6690191f4899933c7`  
		Last Modified: Fri, 03 Sep 2021 01:17:10 GMT  
		Size: 42.1 MB (42119552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1fac91d8e53c4fb65beb0154feabdfbade7d9dbff23333871fa2f2aaef9d67`  
		Last Modified: Fri, 03 Sep 2021 01:17:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:524dc85e9f3fbe99fd8a081a1878dde32324afd93baa8ac6cd8947ff66c1b688
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43178259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6b06bbd1c95d4cf09f2bc47e7771cf6f65b67f0d7c83dfe9a8415a6fa147c0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:08 GMT
ADD file:16630bd6e1bd9138c3013f9cbbfb82c4bae6882fd946ff10a57e8560da2dc708 in / 
# Fri, 03 Sep 2021 00:41:09 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:41:14 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:95be54fb6077dc099cbcd9391b859f68b1cd17e8cf17562baf6680a22a7128d0`  
		Last Modified: Fri, 03 Sep 2021 00:50:11 GMT  
		Size: 43.2 MB (43178033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7785eecc3a04741d6393d665f3e3089f529e73fece88d8c98fddf44f5224dc0f`  
		Last Modified: Fri, 03 Sep 2021 00:50:23 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:718c2a989521c8c96cb245cee2d2c2ae6aaae638916f3e59a773dead31d2f0cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46097570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54e7bc48f7006acc7c7ec06648ce2e99190d4908bc14596ff6d2ff9a120dc5a0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:38 GMT
ADD file:b3f2006307d97327ad7860ab48eb91a453d7528b1ef7350bc13d7e772f319e9b in / 
# Fri, 03 Sep 2021 00:40:38 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:40:44 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6b1e4d8832a8496dfa801314d6250ed633a8662fdee87bfd2cdf0d067ca3966a`  
		Last Modified: Fri, 03 Sep 2021 00:49:32 GMT  
		Size: 46.1 MB (46097343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d55905c0f72e9587d528cd023b033c2f79daf8556d6edfe1ba8a0eca0035d0`  
		Last Modified: Fri, 03 Sep 2021 00:49:44 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
