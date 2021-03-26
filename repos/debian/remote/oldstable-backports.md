## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:94c47d683e154725b42ceadcb910f16e4d4c54e186eea515ae4306a6078092cf
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
$ docker pull debian@sha256:42f80bec45c438e7ab3cd6cc7c573aeeb577875e3594640f0aa9f5e55b21097c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45380408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ead06e63092da1cd29cb0d8da9a25507e38c10bbdf02306c36facbe4482c86`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:21:29 GMT
ADD file:66a3c6c69d180deb58eeb9304c5993525431c79605a6972911cd0fb9c84e055f in / 
# Fri, 12 Mar 2021 02:21:30 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:21:35 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:af2fcd3ed59171fb41a7682292361b44af7829492e944d9dee2b162db1f862b9`  
		Last Modified: Fri, 12 Mar 2021 02:27:51 GMT  
		Size: 45.4 MB (45380182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28848dfbce005200f2d4f9efbe8c2220ab11e57eef92bcfe47aeb78d20125fb4`  
		Last Modified: Fri, 12 Mar 2021 02:28:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:ccdc73a3104eb5221f9fb4d680af689e53b88791ac1d770f68a0e379965cfda8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44092185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c299d5ce050a4e3b0cc190b5b44c6f7cf3453f29e2fb20ed3511087531aeca10`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 07:53:29 GMT
ADD file:7554d0c81e5e1d3e54b83a099e8cd1f9da2e6de5db0f444b9145148552edea0a in / 
# Fri, 26 Mar 2021 07:53:32 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 07:53:39 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:826816ed9e9ae31e48238b0103a0d184bad49e73a0bf05a1dfc44053264da84b`  
		Last Modified: Fri, 26 Mar 2021 08:02:09 GMT  
		Size: 44.1 MB (44091959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ea490077181446b6acd825f96e00501db94731645fbffb71734dfaeebed6e7`  
		Last Modified: Fri, 26 Mar 2021 08:02:17 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:74490159aa48c121a867fcc926d665ce8446fac1413b113138d36b763917259a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42120417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63bfbc225791d03341276afda178c8422b9332fe2e1fdf95d008ba97ec8821ee`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:02:17 GMT
ADD file:97a7aaab41692e534a19554f5bcc13862905e48ab6b10e9b1667b416d92d2d94 in / 
# Fri, 12 Mar 2021 02:02:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:02:31 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c11e3cdf0146d22f442b68f20e231d95f6dbe4ed2c4c93f87c421cb58a2868b6`  
		Last Modified: Fri, 12 Mar 2021 02:12:12 GMT  
		Size: 42.1 MB (42120190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db30ff01b654bd49dcd8e302e009ccd4845bf3c2852a99f10a4025107fdaaeb4`  
		Last Modified: Fri, 12 Mar 2021 02:12:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:78b2d69c4b5e5beed7094c3ecc6736f75f3fd9b18eb4d8f1cf6708e25116957e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43177774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e7c8affe998144af5c0cb4c6f5de361f027b8d5a9d3c4ecdeb4c2df7e3be600`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:54:14 GMT
ADD file:90830b3f84b11a5305acaeaf36f5524cd5ae11d28b64b454fb4dd4775c868c33 in / 
# Fri, 12 Mar 2021 01:54:19 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 01:54:29 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b4bc14244bc7f2d43e8ef422ad82bac8379d41d633b20eddaa53023aed089bf2`  
		Last Modified: Fri, 12 Mar 2021 02:01:58 GMT  
		Size: 43.2 MB (43177547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4cdec44fee3e6b9840a727f2511f29f676ffd383981270402c6a3bb599634b`  
		Last Modified: Fri, 12 Mar 2021 02:02:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:df38bceee60a01562e7eed900595f869817b2776049cbc49077748045bd48460
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46098392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf2ffaa95ccdedb8ed0459bafb57d9b9e77ad947137fb1f151fa4b9ed0cd6136`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:45:30 GMT
ADD file:1a81ad34e787e62fbc796c04c25bbd9c157340cd5e86b2b3b13637fa984187ad in / 
# Fri, 12 Mar 2021 01:45:30 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 01:45:36 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9d62a874454e25ae936ce947090ff00c9091fccd6c1326e3601c9107d7fdab7c`  
		Last Modified: Fri, 12 Mar 2021 01:54:15 GMT  
		Size: 46.1 MB (46098170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8397181de564243a088a97e80cd0f6afe5b3cb307020c7cbe9521e751d6abee`  
		Last Modified: Fri, 12 Mar 2021 01:54:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
