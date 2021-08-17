## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:3cfa7195bd88ea3ffe10a975e81ed2b74cfba0e7a13afcc098226d36eb313954
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

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:ebf30f5c8f9f364b03cef13e995eafb9c59386a156775aa2ac5c00ab4ec0793b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50436434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762dc11d38d087fb08e886ad8beef45ff0cba36ca51acb86c2f632bcd0ecc848`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:41 GMT
ADD file:782a30fdd4a92cc5c9f88fd607212e16775dc81ea54f735842adb903ccb17537 in / 
# Tue, 17 Aug 2021 01:24:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:24:45 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e9a158a6995bb467800ed725e84e874e4fb79a67d40739941bb5b7bd7bd9b131`  
		Last Modified: Tue, 17 Aug 2021 01:31:17 GMT  
		Size: 50.4 MB (50436210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73eee919a1e781b67d7b4f2c114a56a3f91d9a401432220e97ea9231576592`  
		Last Modified: Tue, 17 Aug 2021 01:31:27 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:59574e0efc395e16fc5c6f82daefb6b1297b0c3b95f4024d655253530b4dda2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48154067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa1da31884d7d10883a22ec826f287f0abf2057de000ffaaf81339320bf76fbe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:58:13 GMT
ADD file:47c9d3a8a71aca881a5017b3b12665b8968b67537cac33ba55138e0c7ddbb147 in / 
# Tue, 17 Aug 2021 01:58:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:58:26 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:10e1e79aeb95f45f00aa6211fd5e8e5598fd555d58ad6cb382eb13a450745f82`  
		Last Modified: Tue, 17 Aug 2021 02:14:46 GMT  
		Size: 48.2 MB (48153843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64841cc6cb413315901af77c29f6661adf93eb341eaefdf654751a21b4f3a69d`  
		Last Modified: Tue, 17 Aug 2021 02:14:58 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:1293393546aeed55b2eabe2e4175091d9c7b1b5c95e4268dc14ed535349f49db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42120285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d4ccb65b7d22a10b94e940529dd4cc402c9bad96cfcc08791a4c233725fd76`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:04:15 GMT
ADD file:6b864b2dd4e2cf844ec83eadee2726b89823a127c9ef0f7c9f00f16e863f5180 in / 
# Thu, 22 Jul 2021 02:04:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:04:29 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ec949cff93b2a4256eb754c4312bcdf8b742eb6125fd82bb9be915f0f565a008`  
		Last Modified: Thu, 22 Jul 2021 02:17:01 GMT  
		Size: 42.1 MB (42120057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d1665ae61e2193d337ad14504b74b1428f7a1cff444485dec9e40a8e5c515`  
		Last Modified: Thu, 22 Jul 2021 02:17:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6160502d2e03ceaff6944915b573a8dec09482d9a93a3abb43bb96724ad84ae2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49222565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84a978c198e991daa5e7d4aeb23cd99a9948c48ff60e13b759f1b98e6b8f9971`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:07 GMT
ADD file:d534cd4e353ab98fbf7fd21a77f91fd46239e43d221c99469393631776ebd2a2 in / 
# Tue, 17 Aug 2021 01:47:07 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:47:13 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:264250b9d26982130691a29c1395d2e28a775a75816236f86d01e58e05e039dc`  
		Last Modified: Tue, 17 Aug 2021 01:55:28 GMT  
		Size: 49.2 MB (49222341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4fca801e5bf3221234c98b4a77ef99af99e8c86a09b1e568ef7e9150562e1e`  
		Last Modified: Tue, 17 Aug 2021 01:55:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:ed46f9c556e60366cd28e5a6e7fad27302c570d3a57823161fecfe64669733f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4acfb0121189bc1bf1e2d550c6ee025ac82e621ced3ab6749d05877fcf5cb5e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:07 GMT
ADD file:616e8da9480a930d5e63934e1abbe78b4ae59f0b67ca50c9507096a5090b70e6 in / 
# Tue, 17 Aug 2021 01:42:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:42:14 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:526c8a026aed5d2679fc8b6bc77573bb8636d7cb2d62f4ad511f7f6475d36afd`  
		Last Modified: Tue, 17 Aug 2021 01:52:08 GMT  
		Size: 51.2 MB (51207406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf83fea03a1bc514f2eb57d983032f5682a34a057a124cae5ece5dc33eaae`  
		Last Modified: Tue, 17 Aug 2021 01:52:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:69bd4950e68acdde5e4244bb1f6b568d5894265cec112878fe746f978af4b1e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49079810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0765f6affd464eac23618f2c699c6153ab31463eb084c6a2fd45221cbdbb3a30`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:52 GMT
ADD file:26642c6055f04d9d1b8841abd8a9bc950a3caf3465fa6698658c77c64b51da49 in / 
# Tue, 17 Aug 2021 01:12:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:12:59 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:52fe3dba9ff7f2f2409c38dcb273e05408535cee5ed77072ec57f027d5b90ab5`  
		Last Modified: Tue, 17 Aug 2021 01:22:28 GMT  
		Size: 49.1 MB (49079585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c01b5737709e6525123170a37156badf22eb9f40fe8105f3e6aa6700af10a1e`  
		Last Modified: Tue, 17 Aug 2021 01:22:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:6bc60ff7a88127475935491ce5c511ee3b9676965d15b4a4c9bb9dbc153b494a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54183279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b29fa88a1dc0bdc598555d7773ce602efd9b6464efa6044414d0221f06fe33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:38 GMT
ADD file:043c2971fe27e576bf6a6d4bb5be88577559ff5ea0689260ed20cd59ac7db615 in / 
# Tue, 17 Aug 2021 01:34:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:35:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0b864ff77b9a9941f35d3b463fc281681f4746835845357e7ba7f05d178fec35`  
		Last Modified: Tue, 17 Aug 2021 01:49:43 GMT  
		Size: 54.2 MB (54183053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7b9df3667ebbbbaa845b53beee8810578c9c52a08ecbd8f51afd592248f83`  
		Last Modified: Tue, 17 Aug 2021 01:49:56 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:5dfb0ab1c1a3cc814ad8bd58f8e7b1431374105fb41f77fbd9e9fa34e99250e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49004569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd40d7b3422a52666921f44ba63dfb310f78ed109b92272fedf464e59e969a19`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:50:15 GMT
ADD file:663d041a4a4b55df7705cb69b24f3bf274f7112225020f9e5b54bdcd18e0d183 in / 
# Tue, 17 Aug 2021 01:50:23 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:50:32 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ea4cabe76391fc22662c231bd975bad36de2e8f6c4ec682dfb8cf7e643fcb09`  
		Last Modified: Tue, 17 Aug 2021 01:58:30 GMT  
		Size: 49.0 MB (49004343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20a5e0200378f35b09fe0d0b2b3be5d0808f07506119183f6f9a10b22bbb387`  
		Last Modified: Tue, 17 Aug 2021 01:58:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
