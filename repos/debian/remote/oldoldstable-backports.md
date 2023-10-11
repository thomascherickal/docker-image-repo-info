## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:417f26693dd49d3f6b3672a651ce04a0f8ad7f08e9ccf2409af4655c8828f85b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:b83ec837da9114cfc6d9fb9f53d5f104394745542330cae0d75c833e1f7f7a10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50498385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e79a1b894610ee7b17f2ac95157df70bd5cecbda203d2a9d85c52f0b99ae4c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:34 GMT
ADD file:f64ab63dc255930e81f2e96163f32f2d728a31fec0480825144f9735136598e2 in / 
# Wed, 20 Sep 2023 04:56:35 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 04:56:39 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9c856da886d2b8776640bf119702f18c864788b4e096973c87e45a74c4270f9d`  
		Last Modified: Wed, 20 Sep 2023 05:02:03 GMT  
		Size: 50.5 MB (50498157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fb5a8b8c30c83ac9e5348aaf754b63fdf379b41210cd791e389f75ef10aca3`  
		Last Modified: Wed, 20 Sep 2023 05:02:12 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:0ea482d1b1275d44705ee386890a7e6a6d62a55a6041371a593b2cca1f056eca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45966572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce390eb3cb31d3e1e5155657a42bd041b9b48fece81e50c3bb4c042253a6c9f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:56 GMT
ADD file:1317738366a4d06c3f6fa22c055a4f67f7faf1514ab6dd3323566f638199017e in / 
# Wed, 11 Oct 2023 17:42:56 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:42:59 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3e9fa2be0c536b2717c1b34816504e850b67315fad7ad009fb7f0ef36a2f52e7`  
		Last Modified: Wed, 11 Oct 2023 17:48:10 GMT  
		Size: 46.0 MB (45966345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c199034c3fa806d7aa62a6e1b4681f0845e03ee57fec77e7accf7d06544e25`  
		Last Modified: Wed, 11 Oct 2023 17:48:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:86c95bc2e233769138cb04ffa304fd63a431733ca2c56bce2c58e158b6737ca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49291139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e810868a61c94090fc25d8e2504171cdfbf714b4a673624ede3f48767d7bcd6c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:48 GMT
ADD file:c668c7566bad38acdb4cf94903133ade5ae2602eaa3bb92123e69173e4d3bffa in / 
# Wed, 20 Sep 2023 02:44:48 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:44:51 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:51fc984e0490aa8d77ad122fecef1f9ce0ff384dd3acca4001f69a1ac8068918`  
		Last Modified: Wed, 20 Sep 2023 02:49:06 GMT  
		Size: 49.3 MB (49290912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c514941c74706b5272c0b3530b0a1941299b6c6eb3e4a388e550d173890da24`  
		Last Modified: Wed, 20 Sep 2023 02:49:14 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:55cf6774e1050865f21060601ac5c7d9a4aaae9b4bfb6d469aad4392f2fdbd1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51256298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1dbad912b73bbb3015137e87d464bb1fb784c85fbf044e88148ea4dddf6e732`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:36 GMT
ADD file:a95fac7e8d4f887905a3b2b79ae5cb6475f961ddff14f2e54997d438d02b170d in / 
# Wed, 11 Oct 2023 17:41:37 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:41:40 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:54e79de8c2b088ec9a4dc8d9a3d3d361812680987bbbf3a12ee529d5e98ed80d`  
		Last Modified: Wed, 11 Oct 2023 17:47:42 GMT  
		Size: 51.3 MB (51256068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39f596fae28ada227997705b31b190d2cbb07be89c80c4ab7ffe8effca9b790`  
		Last Modified: Wed, 11 Oct 2023 17:47:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
