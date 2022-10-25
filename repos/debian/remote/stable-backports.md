## `debian:stable-backports`

```console
$ docker pull debian@sha256:99d8e44468a44083aaa4b0f4f34a30854bf422c7851bc9ef21579d994b725de3
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
$ docker pull debian@sha256:19f2f2cba4862eb12c1fec937fb07832850b7b9a0f54df567592a1067f8a2357
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55046577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f42075c7867812c41ccee6f5aec514ba9952e462403190d496802a208b40d98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:59 GMT
ADD file:eb0fae6cc9ae20c0b4bc19663618c9ccfae7108a10ba50b6871d0813aba15a26 in / 
# Tue, 25 Oct 2022 01:44:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:45:02 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a8a0e642eaa9e08096819dffa91eb5676ca8f05d60577ab1887b2368c630c6ae`  
		Last Modified: Tue, 25 Oct 2022 01:50:13 GMT  
		Size: 55.0 MB (55046355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0161a9c82cc1f8c3f9537d2c1d6dcd108f33d1edb2e8c2cc50c5a4124eaa8943`  
		Last Modified: Tue, 25 Oct 2022 01:50:23 GMT  
		Size: 222.0 B  
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
$ docker pull debian@sha256:60817a639240d8cfbb880610a702d6f4fb90d8330dea28ff53355673f33b4c48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fa9a5f8b00bb55524ad83626d6defea163a7c6ffb9448d2f2a5ed46b0d2555`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:15:18 GMT
ADD file:1b01648d65d9b1c7ed1894e357e1b51d87a2c86c8e5a5a7051f8773a95b7d9f8 in / 
# Tue, 25 Oct 2022 01:15:21 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:15:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:facde612a2c394cbe497ea9610c4e1f37a765e53d3bf62a88620338fa8890860`  
		Last Modified: Tue, 25 Oct 2022 01:19:43 GMT  
		Size: 53.3 MB (53279173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54b062704f5375d79ade07d3309be1ed57ac2c1f4c2183298f8ee6baad932eb`  
		Last Modified: Tue, 25 Oct 2022 01:19:50 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
