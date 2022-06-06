## `alt:latest`

```console
$ docker pull alt@sha256:3ec80c11a8d27ffb8fe623b4bbf8f069c6eabe59ea8f89146a9b84428eb790e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:latest` - linux; amd64

```console
$ docker pull alt@sha256:0a0e63e37adcefe8c44d5252582380b38d4096be944c96c73c88ffff0d793154
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41956635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5233dec4a33662efe7fc8ca31e1226c0f4d862dc0cf05660b6df697368e57b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 18:19:53 GMT
ADD file:7da049293364e41e28c4dfa7726081c793305f575bf42f01aef8038a656200da in / 
# Mon, 06 Jun 2022 18:19:54 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 18:19:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b78b46836363a42026d28fd62d0a291aa88c57f84285775b5f741aac740a77fc`  
		Last Modified: Mon, 06 Jun 2022 18:20:28 GMT  
		Size: 42.0 MB (41956443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30a04c8a5bb234876f129e9ba5bf89d0e2e33616a7e6a181d990e536889dd88`  
		Last Modified: Mon, 06 Jun 2022 18:20:22 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; arm variant v7

```console
$ docker pull alt@sha256:2faae5e72852503bfc0529ffa24f7dbbf246af0c84379238269a9de916c815b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38449188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:530bd5ff54abf16e74dab65e1c81292942e09ec8cf16470db680ec632933d1b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Aug 2021 01:09:27 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 17:57:57 GMT
ADD file:a29a57d8b696b1047accce9a350ecd76ce9f43812fb3219d82193c7400ce54a5 in / 
# Mon, 06 Jun 2022 17:57:59 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 17:57:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:85532c23a233e89414ef3835217fe5a50caa581b9e6b88dd1f998f222fb3ffef`  
		Last Modified: Mon, 06 Jun 2022 17:59:45 GMT  
		Size: 38.4 MB (38448996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e888d917a95026812324080f16196005b8bc334a42a55290f944e8a2810eae`  
		Last Modified: Mon, 06 Jun 2022 17:59:19 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:99e64abdfd6d2b783d6aa2dd7bbfb655bb0d911a092599ad51028786e46c7170
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40922315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abbba9fb6efa7b1e7a9828003a18ebbcec604ebf6688da23b608b3b4fe85318b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Dec 2021 16:01:29 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 17:39:44 GMT
ADD file:bf21138d2f7d4747aa4b46bb88b549639c56c9ed50b0d6f7944ebce35c112dc6 in / 
# Mon, 06 Jun 2022 17:39:46 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 17:39:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f9a43b79cc159f9f7605e2f78ce2f4dc22b4ccfd5be651adac7f10249313f274`  
		Last Modified: Mon, 06 Jun 2022 17:40:29 GMT  
		Size: 40.9 MB (40922123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d1722b07ca53fef39f9980ff96ace2895e46f09028b67a566d4665b17780c4`  
		Last Modified: Mon, 06 Jun 2022 17:40:23 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; 386

```console
$ docker pull alt@sha256:1acaaec1104c12a92b0de5e9808555e67a545746cc581c15f47a064492007e86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42654623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e3abd278ad8be0390b734d69929c2e6e9ad832600c923a2ca83cdb0665a1b1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jun 2022 17:38:38 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 17:38:42 GMT
ADD file:f402299181273834f95e0c5fa0752eaa1d34ae83fa414c913636d467155714a9 in / 
# Mon, 06 Jun 2022 17:38:43 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 17:38:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:66413a85b9435e372031641e16cc87490db1c76dc51bfece65def618259053a1`  
		Last Modified: Mon, 06 Jun 2022 17:39:26 GMT  
		Size: 42.7 MB (42654433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af7275a199df4a96ad3fd669388b9e8c82ffc68390269d9c30493bce8c8d145`  
		Last Modified: Mon, 06 Jun 2022 17:39:20 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; ppc64le

```console
$ docker pull alt@sha256:d13de7662c45c23222a4a04e141739becd5625b686555b7bbebfc5b633998a60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44727291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:973f0df8695ee4a112cab88ad945744b3179411de61262e834675ffc9bc227d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 18:21:22 GMT
ADD file:b033eeff06c036113d90ffe9bf5e20ec1d5a95505a30495b23aacf02f04a5959 in / 
# Mon, 06 Jun 2022 18:21:34 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 18:21:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:38aa62cf6ea2e03de7a783a86e6c26697dd8614760aa524cac2f74d6ec610fa1`  
		Last Modified: Mon, 06 Jun 2022 18:23:13 GMT  
		Size: 44.7 MB (44727098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c876250b97f5360d7ccc4a008c63215130030160d39645808ef55b8e39576a`  
		Last Modified: Mon, 06 Jun 2022 18:23:04 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
