## `debian:stretch-backports`

```console
$ docker pull debian@sha256:99a9ed05c64a947c40de52e18f036f25b400cb43d9d4b2b9bf8456bfa30386d1
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

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:b0b6b9dd8bbe059f3cbc39e4c126448c14d42fd3168e3ab8caf26c7c020da7f7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45380884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6369148e40065c3ea5f04349a51fa7e1ac692f3b52f16db486fa91d40a24115a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:46 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e36a6dc5a5be36b639927c185415c5edbdb1dc570e2ca2da3df5d186b7958bf`  
		Last Modified: Sat, 01 Feb 2020 17:28:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d4f1c63e44c5ef5499f3672dacb554f7ed56ed5ec5f5bc38c0df30cf18fa4e75
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44073586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c19df21d9d4ba240a1f34e8c3b47b7d04cec91ecf506228eb59cae3fd919eb`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:53:39 GMT
ADD file:f229f8ad575dbe0eecebbaa4c410371dbbaf8a20b6dccecb7a73b2cfb6706372 in / 
# Sat, 01 Feb 2020 16:53:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:53:47 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4a136771265373b04f705abd2c190724eab8195169bce62483ae7ccf66454fbd`  
		Last Modified: Sat, 01 Feb 2020 17:00:43 GMT  
		Size: 44.1 MB (44073363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553906dcc3c47dbe1a240851d8408870c0e65c497c4f469f01652345705fa6a9`  
		Last Modified: Sat, 01 Feb 2020 17:00:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:af498c834434205a31095fa413ae458f73c81c207a8bb80f7e8f15a34f87b616
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42108594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d323f1785ba9f1e5773e531fe6c2e0d42fd7f49b6d13d4e865261791e35222`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:08 GMT
ADD file:b7fc54d004d962f2cfb469a1aaa9e689e46dfa2554e0cf44c33981d688adc31b in / 
# Sat, 01 Feb 2020 17:04:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:04:17 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cc3b08e804cce7e88d9df954b76be506569775afe9cf36316f2fa6c5c9bf3d5c`  
		Last Modified: Sat, 01 Feb 2020 17:11:13 GMT  
		Size: 42.1 MB (42108370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80529876566f45bce8da1ffb798572327cc2b9c53b980cf38a456f1106f142f6`  
		Last Modified: Sat, 01 Feb 2020 17:11:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b4063c3c88a429bd757fab407b0c349692c120d27db0dfe79e3546fbae53aa17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43166975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:874b261cf279001823b313e4e65efefec643ea474eb4ae968cb4af503948a518`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:01 GMT
ADD file:1618e6474dbe6462a610ce7eed99f0bfd087ea37ddfc287bbd69def5c24ede47 in / 
# Sat, 01 Feb 2020 16:43:02 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:43:09 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:df3de44c7096ba135556a1e7044f9e1feee3ef713ab96f0416f71fe78422cbf6`  
		Last Modified: Sat, 01 Feb 2020 16:48:40 GMT  
		Size: 43.2 MB (43166749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f21c7f6152674e2fa63f331fb8ed6d597f0386265cf8ec805f99b044d6d732`  
		Last Modified: Sat, 01 Feb 2020 16:48:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:feaf65f94627c134decc7939fc3fa4c86fd0f1a7d4b5bdf1d275f9e00c31661a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46100240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba1f4673b5652f571944d6469e730eb17d77e17897e59a3e2251dbb5cdf0f32`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:53 GMT
ADD file:bae1646c4e3069e717d1ee4f6c312c249e96a21d795a639cdfaf338d645c8be9 in / 
# Sat, 01 Feb 2020 16:41:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:41:58 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:97067fdacc0601fe58a5f782cd09d3c58a214c43b8629a2d92bd7025f46fd265`  
		Last Modified: Sat, 01 Feb 2020 16:47:15 GMT  
		Size: 46.1 MB (46100017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7d7ee8ad89ffe71ef229d00822b04281728de649307bbb0f1e1c4727837b5a`  
		Last Modified: Sat, 01 Feb 2020 16:47:19 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:ea91f3b378de138190ca2a7f37627534993c2765897fb046172ce2a20e8af323
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45652525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d0617410562ce54cc92a31b491e48172b6b1829005a6fc994efb030e6390738`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:12 GMT
ADD file:ebcf4b112436fa7be8efa5ef204cc174c0d1af648c6ab4af968a71aa2ab2cf4a in / 
# Sat, 01 Feb 2020 17:20:16 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:20:29 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:072f803f12e35b1a40604b6081cb448d46529e3eb1d453ebbf56850c211f5bdb`  
		Last Modified: Sat, 01 Feb 2020 17:30:44 GMT  
		Size: 45.7 MB (45652299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cf0aa458375b912956f3c7a7e7a11b946d9a441aed169339c3ad4370ed8c92`  
		Last Modified: Sat, 01 Feb 2020 17:30:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; s390x

```console
$ docker pull debian@sha256:37c9e2b092e6debb8670be6f7b55980cf83a8d53e75ad21196932af5692592c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45241807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40e53fcdb184ee6eb6c79d843a415943fd3d5f7e4ca4d41f33cf15d88f75f605`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:43 GMT
ADD file:17af4834ca99365d5ecf14eb938572689bd3c3ad5fd8a88da12c4c3474975771 in / 
# Sat, 01 Feb 2020 16:43:45 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:43:50 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fb54e9d54b34d992a5c6582a6fe3836692cce3589a408748090bbb916a4cc63d`  
		Last Modified: Sat, 01 Feb 2020 16:47:28 GMT  
		Size: 45.2 MB (45241584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303efe09e0d0ca7045a71be0dbb67085e0957a5a85f69c0ebb56c9a6c523f432`  
		Last Modified: Sat, 01 Feb 2020 16:47:37 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
