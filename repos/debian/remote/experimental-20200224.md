## `debian:experimental-20200224`

```console
$ docker pull debian@sha256:ce40ba5cd56c433d9047205f2264583c5ae2ff742f7c360c0d25a2084a78e5b1
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

### `debian:experimental-20200224` - linux; amd64

```console
$ docker pull debian@sha256:f33a8a0f4aa992010bb2722d5198762525beeeed482d3b94cfb22b99bf634b60
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51852640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1728b69424e8de722fc4e9ae2611284e2bd7502ace60988fb6cc8314f9d67a64`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:42:35 GMT
ADD file:ba619c369bcbf3fb390c2ef2f6c1446bd61526e768cee39e2eaad1d3a0792c45 in / 
# Wed, 26 Feb 2020 00:42:35 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 00:42:56 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c882ee8ee4c4dbe319ea606b406aa1789ffbe57844c5b8347141fc68f3af379c`  
		Last Modified: Wed, 26 Feb 2020 00:48:15 GMT  
		Size: 51.9 MB (51852420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ab8eb8d7d7ed23986a36218bb1f55eec36e250300a74e60310aaadd29f78cf`  
		Last Modified: Wed, 26 Feb 2020 00:48:38 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200224` - linux; arm variant v5

```console
$ docker pull debian@sha256:e3924f178cd9c8e407910344c35b4bada4677aed615a1273c773652299939db5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49854802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1c158e1e067dc2e9e8774419b8a0809ac192ed3810c7c77e19c19d76aec69a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:55:54 GMT
ADD file:bd165c118542320f80b40e59c32fd4eb40c4c50a74e0ea3ee6854103628d8828 in / 
# Wed, 26 Feb 2020 00:55:59 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 00:56:47 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ce3ab28a005b417d4692d16b4fcf93cd126763dcef449ac885a7b2823cb1e75c`  
		Last Modified: Wed, 26 Feb 2020 01:04:43 GMT  
		Size: 49.9 MB (49854580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c1e0ec40d2178938b6878ef7e8f61420518d8bede691d43227a0bc663c833a`  
		Last Modified: Wed, 26 Feb 2020 01:05:06 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200224` - linux; arm variant v7

```console
$ docker pull debian@sha256:2cba7c819879939db6b77aea3153b6eb1aa896f1bd211d8d0d3397881b49c42d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47587256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102ca4ca08161b7ba816e1573a59c5915e5215baa236fa24eb27ec726e4fcc5e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 01:03:38 GMT
ADD file:42deb4899e2023658071a412417f8bcae6af8f71d8712c6828f492429d6cf1ae in / 
# Wed, 26 Feb 2020 01:03:47 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:04:54 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:38b40204df3dbc47d35b5c1a433707e5f84c3ebb38e5d51d7da09f267a0836ed`  
		Last Modified: Wed, 26 Feb 2020 01:12:54 GMT  
		Size: 47.6 MB (47587034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d6ab3ba4122fb794ae19a9d502ae025c50ba121421f2109cec1af5e9942587`  
		Last Modified: Wed, 26 Feb 2020 01:13:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200224` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:571604dbc1f1660ee7511c86960ba3b67ce1f689aa6292bbf4ec5edfbdb7afea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50825340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9903e22e529de328bf05bf6c1f46badda52c6c14d7f10cf0cac752bd04fddcab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:47 GMT
ADD file:45b0bf38929542776b712acf57d6bb864b988e78c51e9aa3aa379bf350aaf1e8 in / 
# Wed, 26 Feb 2020 00:52:50 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 00:53:45 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:28437fdb5bde91523026f69fbbd2192d251796689c95fa802cc0d7aa44b311a1`  
		Last Modified: Wed, 26 Feb 2020 01:00:14 GMT  
		Size: 50.8 MB (50825116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7100571b29d09295c0cd7a2493fe02a56c727b212aaf7a6fec9cd962b7dae7`  
		Last Modified: Wed, 26 Feb 2020 01:00:44 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200224` - linux; 386

```console
$ docker pull debian@sha256:40de0ac07cc3c36ff85df99ded8ea17377d3c9c96057fd195bcbadbf89e7005a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52999796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79b44f9dd5bec05227df03b643054918a10ec74d874c5e343714f8f45805630d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:36:34 GMT
ADD file:5955a629c35b1206468485798e83690e152f5d8339418318b4bc5f98767d2df5 in / 
# Wed, 26 Feb 2020 00:36:34 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 00:36:53 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5367f3e8a07cb0a9f87933b63de70f98eaa2c832490cf96072fa70efc87341fa`  
		Last Modified: Wed, 26 Feb 2020 00:42:59 GMT  
		Size: 53.0 MB (52999575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7ecec61c6a38b9086cfd38dbbb7deb338135040dd4aaa6e93e1eb9d859121f`  
		Last Modified: Wed, 26 Feb 2020 00:43:18 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200224` - linux; ppc64le

```console
$ docker pull debian@sha256:ab1d3e87b30988079e04aa9d1201b9ea42dac9381b2f20e48f0820c71944883e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55686368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32432b4085dab8fa7510d579739e3975e8a268d566ec53c128f42bd7cc0b0771`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 01:39:38 GMT
ADD file:28e17bae2d5a63ee1507c3d0a0f6120ffa183c605e2a029d50131aaf5d689f31 in / 
# Wed, 26 Feb 2020 01:39:46 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:40:31 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:bfa76a971c58dbe3ac1eb9dd6191eb23dc6abb4f0ba95fd0bd2b15f1e37952c4`  
		Last Modified: Wed, 26 Feb 2020 02:09:43 GMT  
		Size: 55.7 MB (55686144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55029004da5a9521fb2d6f5c27b2b27bdb1b0f278b1a07cebcbf5ba3b6e98d94`  
		Last Modified: Wed, 26 Feb 2020 02:10:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200224` - linux; s390x

```console
$ docker pull debian@sha256:4608748f734f59d589cdb9edd2d8ad35da9e7355a19bcada137f271c3ff24c02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50488689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df25e8145c4dca365929444f978e9d75d3569accf42140ca794339684ef0d9c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:45:55 GMT
ADD file:02b4768389ffe5f711ee7a08aa7f2f582a284587edfedfec32905cf79de1db58 in / 
# Wed, 26 Feb 2020 00:46:04 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 00:46:22 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e3e208ba6a0bc3a8e6197fe0e64ea85237d8d08d5c6d4dbde3629878979a3683`  
		Last Modified: Wed, 26 Feb 2020 00:50:01 GMT  
		Size: 50.5 MB (50488467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0c86ee983e1d5e035d89ee6a3226fad2c257e6ec9bd2ae296aa71aa2fbf1f7`  
		Last Modified: Wed, 26 Feb 2020 00:50:16 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
