## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:cb98618dc916e3509dd2446ae54a3a25ee678615c9ec4eec41b2488eafd61dbf
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:39bc93fd9d2315bb9356896a83f272adfc4bef37c51beec60710b7e39d4f16d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49278238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd949d4ea078e486363b535039016d50d778af3e906e17739565603058133306`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:29:51 GMT
ADD file:98917c081507795b8ce084d09f5df75e959c5365882d73ca7a52da226c93fdcf in / 
# Thu, 23 Mar 2023 01:29:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:29:55 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c15c60aea1a8c926f00ec7713f9ae1fcd349591095bddcc01ee5a6027b8a3998`  
		Last Modified: Thu, 23 Mar 2023 01:33:26 GMT  
		Size: 49.3 MB (49278011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734b18588143c724fe68071d73c58f7b55ff4db695e34f9c092252059e89999a`  
		Last Modified: Thu, 23 Mar 2023 01:33:34 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:db1319053a517aa8c4b30bd1a8eeedd29ccc9870ceb67f298c9a23477a0257e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48116983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba6c82538db36cc268215482b30b01c686426b0f3b90e8fd8311c7a653ad231`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:20 GMT
ADD file:db0e63af763d83bde06370ca01585b3ee9f44f7ed2882957bd550b09c5f1cbc2 in / 
# Thu, 23 Mar 2023 00:48:21 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:48:23 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:de716ea1518d1453b21c4aa4b1dd63157f88ebd2da72a9849cd248b6ba9dc14f`  
		Last Modified: Fri, 24 Mar 2023 23:21:59 GMT  
		Size: 48.1 MB (48116759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3eb08d5e043e482eaeed881cfdb8e940c25a6b44367245dcbf7ac554088b1b`  
		Last Modified: Fri, 24 Mar 2023 23:22:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:ad3a5826d0b163bc3c566c1f343bb360ecbc64d51a39738d3617fef3758cdcfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45889417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:241e449908a28aebae55d00619939b1bbe05429675fcc07b681bdffe2a2210da`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:09:37 GMT
ADD file:084e44d77ffdb8aad1f856ec10db87922bdba3a90e06f9f1cafcb6e4284c8ff7 in / 
# Thu, 23 Mar 2023 01:09:37 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 23:23:08 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0b14dce67c2fdb37d2b0eacccff5119e226c45c2906f12d6ee93d8850400824b`  
		Last Modified: Thu, 23 Mar 2023 01:32:34 GMT  
		Size: 45.9 MB (45889194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1b2b2dbc7bd8911066ee69ea80842760d7fd79760b4230ed9de50f050d53a`  
		Last Modified: Fri, 24 Mar 2023 23:28:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:4fd8f0003ee3744d36ecc4eaafc406b5db0907d482f1247ea5407e4fff8ed134
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49328503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0466c46f51ae77128f02600968654dfd793bae9ab1794a537c54ad1e21c1cb8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:48 GMT
ADD file:fc54d0a42f70d91c654d7ac03aa3d437fad192d9f4fd701e214da74c18630636 in / 
# Thu, 23 Mar 2023 00:44:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:44:50 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b813e5ae6de73806a605f44184f1b7d14569e88447b46841154803d1dd1eb646`  
		Last Modified: Thu, 23 Mar 2023 00:47:13 GMT  
		Size: 49.3 MB (49328280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b17967d612dc392ed52fed540e556b18298da158f7c9a2f576bc96d131f432`  
		Last Modified: Thu, 23 Mar 2023 00:47:22 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:460a44ab5412c9c20200c75fa547ede316ccd1ea03a421ab927e9990a595e25b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50324158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f679498ab7edc57c6bd1ba939837309b93837698ed55b082d7866242d5ca5926`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:38:46 GMT
ADD file:a8b128db07f7f5c47ccd2afe2595fdf9b31844beff2d07ae2ea0e204e2aef4c9 in / 
# Thu, 23 Mar 2023 00:38:47 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:38:49 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4dc30e65d953c72fa1dd5a25980f7eeea620434c102211fdb72a04706c06dd96`  
		Last Modified: Thu, 23 Mar 2023 00:42:07 GMT  
		Size: 50.3 MB (50323933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cf2d244fc0ceacc5b5f0799be9f3be977adee14abc6cb94dabcac94157ec3f`  
		Last Modified: Thu, 23 Mar 2023 00:42:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:afdf48d23bb36897b741677462f3afb8e60f1f11327a906be463daa5342cf17f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49291881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80855f2215f5503f6e049af40b21202c66d4887d122ad2ed57a9d7b2dfbbeff4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:15:54 GMT
ADD file:454bfcbdd9d738730885002e9124aea5e8eb4920ca5d3bf13bb9f4707023bd67 in / 
# Thu, 23 Mar 2023 05:15:59 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 05:16:19 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:70edc5cd98f5a2e589d309248c77122dabf95f437c0448b99513b15ef209f244`  
		Last Modified: Thu, 23 Mar 2023 05:23:55 GMT  
		Size: 49.3 MB (49291654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5a560b9e18333511454cc0784fa79545b470a54c240728f8cf98b9505575f7`  
		Last Modified: Thu, 23 Mar 2023 05:24:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:bdded0c1d372744870b414c8ac71d18ccac2b1338968ebe3dd0b022b77385a3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53290540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37995728cdb0ea4a5797b5258bd910d4fa3277f05fdcbec1fd7fbe343e0306dd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:18:49 GMT
ADD file:5e17f6075630657b8465309f99ecbfc57e325d159b54f58181b974526f2314a5 in / 
# Thu, 23 Mar 2023 01:18:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:18:55 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:60e68956630003599038e3cfe86d6dd09ee874e8c30d9ea29b8350e0d3fa8497`  
		Last Modified: Thu, 23 Mar 2023 01:23:06 GMT  
		Size: 53.3 MB (53290316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ac1321e26143240dabfafac550c4fa58963a6f8fa8fafd7de04745a1be617d`  
		Last Modified: Thu, 23 Mar 2023 01:23:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:c63ff8b19dec1f5380e763eb9313d772704a92d6ba93e6835d18ef933f2f0975
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47671261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eeee0290269cc8658da057af0ab2729901862f45a46855fcd6266b01af0371c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:43:22 GMT
ADD file:2114d04d7187ee787a64bd515adc18fc532b91c0272b95492fd44714772b3eb4 in / 
# Thu, 23 Mar 2023 00:43:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:43:31 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:09c6f64f2013e0d0258d4e75a51c004bfcc5479af28502ec4cbf6e25f28ee505`  
		Last Modified: Thu, 23 Mar 2023 00:46:39 GMT  
		Size: 47.7 MB (47671033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ce71ab9828c634a772b629abfa1a12ba9ce2a7d1da8b25e62b8c81060419d8`  
		Last Modified: Thu, 23 Mar 2023 00:46:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
