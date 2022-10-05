## `debian:stable-backports`

```console
$ docker pull debian@sha256:3bdae6b17d64fb4d7572a6817b81205061c992714ba4f3ab35113df7491fa8c0
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:05a0e435d68684fed615a42e1e2fa3378005098bf19c46eba8e986b19de0b391
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55046501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8088b0c785da73fc7f6eb7b04a677d404ea9352695f9275737b2389fe952917a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:52 GMT
ADD file:143b1f672b7a2c9ba881cf10aa3bd719d2097391d1377f3a87c9f5fc8b0cf45a in / 
# Tue, 04 Oct 2022 23:27:52 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:27:56 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:225ba7910a626c18380500b73b6fb1f85725553101ab41a46663a25725f81171`  
		Last Modified: Tue, 04 Oct 2022 23:33:03 GMT  
		Size: 55.0 MB (55046276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fce14c5b4748babb0b553c35847a2f2326f00deea64886bd66df220b5d155`  
		Last Modified: Tue, 04 Oct 2022 23:33:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:eb87634e79217f2531e24e7b66a9686f081847200e0f515d71041cce9ad9c699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52547434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ac22a3e12c76ea8ee7b0aa51aab348c098b9e43eb36dcd554741b17646d605`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:43 GMT
ADD file:7bd25705f1a93f8496d70658bdcd0925047b4bbc066a73ac5c6ea92033022510 in / 
# Tue, 04 Oct 2022 23:49:44 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:49:49 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7a4bcf0f8b89e3991faa28212ab07fc2e89a63fd710c139bd8fe0fbf1253a86f`  
		Last Modified: Tue, 04 Oct 2022 23:54:55 GMT  
		Size: 52.5 MB (52547211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68814a7fc3f8f9ce98a03596161aaf935d68afe343c0e441c72d8255899d07fa`  
		Last Modified: Tue, 04 Oct 2022 23:55:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:60e0056061f96ef43aa24d72558ea6232ab104d6bda84d11b1af81155f11521e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50209265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5fc759d8b725a3ada76438478844709d3f7711f34bce26ec55d7c2db027431`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:26 GMT
ADD file:f143df2424d48c18e0fc55e46c58e1404b6cffdffb7c1c8160378f2b83b00df1 in / 
# Wed, 05 Oct 2022 00:00:26 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:00:32 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:85f0f175e7693d07507322b0f2c84dceac752837070a45bad5558c6b7b43a64b`  
		Last Modified: Wed, 05 Oct 2022 00:07:43 GMT  
		Size: 50.2 MB (50209041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b33a9198729e20ea28492b92ffc995c0d385fa714e92a17ec450eb6dda79b`  
		Last Modified: Wed, 05 Oct 2022 00:07:54 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ef86292ada56103664a96d9591c3e98885913af72a2c9d9541e203f508890ac6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53700862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26390ffaf62fdc04a7bc552e952778d6b889a812bc38ae467c092888ffd6a777`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:46:08 GMT
ADD file:7432f9080ffb61ff1296169ced0f40910583cddc75781f01f3881da808070c32 in / 
# Tue, 04 Oct 2022 23:46:09 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:46:15 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:993be7e6361f35123f2a260d8c5268cbc9e9b61ca852da08a93a1c14051208d4`  
		Last Modified: Tue, 04 Oct 2022 23:52:50 GMT  
		Size: 53.7 MB (53700637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b34bb1cd7e6ce8b32b3324b404a5e485f4e74838a4fb1366cab02c6269cdb9`  
		Last Modified: Tue, 04 Oct 2022 23:53:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:a9c168891287fe0806cc0f3141e9be590c75503c60190c5b80b9cff2e6ae5fc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56024062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b0ceb0354c2f7181918ec78bc9fdcee0079d23fc1fca389bd09452e6035c325`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:41:11 GMT
ADD file:8d6c649763e8a51158b9007fcf3190ed3436c14fb276eaf31f403d0acd630f61 in / 
# Tue, 04 Oct 2022 23:41:12 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:41:17 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7e3304e1199b4dad2490fa4af580ecc0ef35ff168d083178611fa04c008e51eb`  
		Last Modified: Tue, 04 Oct 2022 23:48:02 GMT  
		Size: 56.0 MB (56023837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091a52c5055090966189af8ddbcdab63848387056605d65681e8fdf04ebe42ec`  
		Last Modified: Tue, 04 Oct 2022 23:48:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:db6391d8a69c6c7b2a3f5bd036d9e4a395607e53178f5c2b9043c946d5bf9efa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53266051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039e88e7d35a1cb7cd414d1813d5197296f1ab120e68be02fe2ee4ef7bee494e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:12:03 GMT
ADD file:a5fe154c8830989b9086566c70d43c8392077f2aad8fcd9ba028026c98283805 in / 
# Wed, 05 Oct 2022 00:12:08 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:12:21 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0001d895ca18d1d863f7db1cee733d5592b2a5a08d4a6fe8fcc44c35884e82bf`  
		Last Modified: Wed, 05 Oct 2022 00:20:32 GMT  
		Size: 53.3 MB (53265827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6ab0e583defa86e603ee0a7348220c69c30191fe64814d9e44c92d2a057d9`  
		Last Modified: Wed, 05 Oct 2022 00:20:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:b3b0cb12541cadc4ed97b11338a67f214d39903067d74b74d03284409543d113
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58917431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3d7d4d04bf47f43efdc643d5b3537c46181e31124398f24499632659c9013c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:19:00 GMT
ADD file:4c5d06588cb0c2a60726857cf01ad3c26ae006864c52163270a862e9f420a5b5 in / 
# Tue, 04 Oct 2022 23:19:03 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:19:10 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6856d5ecd2bd68ab421a3117cc2d1116a23ce7debac3979a1d3594e45e1fe166`  
		Last Modified: Tue, 04 Oct 2022 23:25:31 GMT  
		Size: 58.9 MB (58917208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4011be54e2ebb56bfdbf7f3fb6b5ae939be522a540f3a361340708634bee1a`  
		Last Modified: Tue, 04 Oct 2022 23:25:46 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:33ab815daaf099ef24b26a685f31583d5e6126040ff1172a6c15442d14782061
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d7ab2a1e31b17787c17cbd8a3b384c9616c91a7da43ce5908679dce069eb37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:43:19 GMT
ADD file:45d3cc064d2f6afeb7dfa34acac350480a9b76a883c529c52d8288770f804c1b in / 
# Tue, 04 Oct 2022 23:43:22 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:43:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6041be6dc51b702c022517ab0f6123fa06e79afd46f098ea9960cb52ac611404`  
		Last Modified: Tue, 04 Oct 2022 23:47:55 GMT  
		Size: 53.3 MB (53279766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57146020701a7da65cae507895cc8837a817f8d9242076d6c5952b771c73f40`  
		Last Modified: Tue, 04 Oct 2022 23:48:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
