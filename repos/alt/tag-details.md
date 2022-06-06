<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `alt`

-	[`alt:latest`](#altlatest)
-	[`alt:p10`](#altp10)
-	[`alt:p9`](#altp9)
-	[`alt:sisyphus`](#altsisyphus)

## `alt:latest`

```console
$ docker pull alt@sha256:2b3a142c7313529526ba5a2e4998f5761d475efb5d1edaa5a8fb57e31075491f
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
$ docker pull alt@sha256:0054b7dcda3129adb591780aafa94cb707a27a6017f50f06e84e4089a5a3a5c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41851870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68b2b53e813f5743de937458b5d7e22bbdd5ebc6f0de65be020718710baa42f0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 09 Feb 2022 22:19:49 GMT
ADD file:11e7012d33c06e547e6f0c7050c32bd4747261f3b07e4096adec660fed669e4b in / 
# Wed, 09 Feb 2022 22:19:51 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 09 Feb 2022 22:19:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ccaf2fae478c64c9c51bc3ac8c0066b6f0a61444bd3c22d0d0ece5317d4b9281`  
		Last Modified: Wed, 09 Feb 2022 22:20:27 GMT  
		Size: 41.9 MB (41851677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f64ac690d0b5b33d640b678b3666e65d37559a3309d65c7d7d53e9d3a7860e`  
		Last Modified: Wed, 09 Feb 2022 22:20:20 GMT  
		Size: 193.0 B  
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
$ docker pull alt@sha256:1baf30444fc00d6d994bb52f8cbee11fbc73b89afbe3f46eee74abdfb41c367f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44664023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:696e86df5719f2f89a9897f22e1ecbbb6b8abf0c87f5f047651b356f97c508e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 09 Feb 2022 22:23:30 GMT
ADD file:b27281c63dae2e0067286c0d584a2ae761072d75c968cd067c440fa87327ad55 in / 
# Wed, 09 Feb 2022 22:23:42 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 09 Feb 2022 22:23:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:73d67dccc54e0dadc0e7c48320aaf1ee7adf55abc728da94c299ba1209883630`  
		Last Modified: Wed, 09 Feb 2022 22:25:17 GMT  
		Size: 44.7 MB (44663830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb08477591ec9af6cba91bdeb7702ce3b0da6c323cb046f14759600d34b76d3`  
		Last Modified: Wed, 09 Feb 2022 22:25:09 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `alt:p10`

```console
$ docker pull alt@sha256:2b3a142c7313529526ba5a2e4998f5761d475efb5d1edaa5a8fb57e31075491f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:p10` - linux; amd64

```console
$ docker pull alt@sha256:0054b7dcda3129adb591780aafa94cb707a27a6017f50f06e84e4089a5a3a5c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41851870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68b2b53e813f5743de937458b5d7e22bbdd5ebc6f0de65be020718710baa42f0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 09 Feb 2022 22:19:49 GMT
ADD file:11e7012d33c06e547e6f0c7050c32bd4747261f3b07e4096adec660fed669e4b in / 
# Wed, 09 Feb 2022 22:19:51 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 09 Feb 2022 22:19:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ccaf2fae478c64c9c51bc3ac8c0066b6f0a61444bd3c22d0d0ece5317d4b9281`  
		Last Modified: Wed, 09 Feb 2022 22:20:27 GMT  
		Size: 41.9 MB (41851677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f64ac690d0b5b33d640b678b3666e65d37559a3309d65c7d7d53e9d3a7860e`  
		Last Modified: Wed, 09 Feb 2022 22:20:20 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p10` - linux; arm variant v7

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

### `alt:p10` - linux; arm64 variant v8

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

### `alt:p10` - linux; 386

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

### `alt:p10` - linux; ppc64le

```console
$ docker pull alt@sha256:1baf30444fc00d6d994bb52f8cbee11fbc73b89afbe3f46eee74abdfb41c367f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44664023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:696e86df5719f2f89a9897f22e1ecbbb6b8abf0c87f5f047651b356f97c508e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 09 Feb 2022 22:23:30 GMT
ADD file:b27281c63dae2e0067286c0d584a2ae761072d75c968cd067c440fa87327ad55 in / 
# Wed, 09 Feb 2022 22:23:42 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 09 Feb 2022 22:23:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:73d67dccc54e0dadc0e7c48320aaf1ee7adf55abc728da94c299ba1209883630`  
		Last Modified: Wed, 09 Feb 2022 22:25:17 GMT  
		Size: 44.7 MB (44663830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb08477591ec9af6cba91bdeb7702ce3b0da6c323cb046f14759600d34b76d3`  
		Last Modified: Wed, 09 Feb 2022 22:25:09 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `alt:p9`

```console
$ docker pull alt@sha256:19aadd07cac63ff584d6c306779d5fe2f024c8adce19062ba0c4727fcc667be7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:p9` - linux; amd64

```console
$ docker pull alt@sha256:f8624fa51a85cbc5e91d502f1d1084ce11100de9ccbe50274329e395df6975ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43052138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25768925d0bb62425e3df7d088536d8578c1f4cffe4e276ef8a4cf63e9808660`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 09 Feb 2022 22:20:00 GMT
ADD file:cd817fa0285f86a0f888784ff576dc4d349bb88b24f9bf942ade982fd5d35967 in / 
# Wed, 09 Feb 2022 22:20:01 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 09 Feb 2022 22:20:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ba90bcadc6ba199f8174c6bae18dd014394b32da0b34cee83d658ef25c071994`  
		Last Modified: Wed, 09 Feb 2022 22:20:42 GMT  
		Size: 43.1 MB (43051949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687d252296d1e247bb9033b5426f0efd2b8f7c225aa1dc72ab19f61bf25a4c47`  
		Last Modified: Wed, 09 Feb 2022 22:20:36 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; arm variant v7

```console
$ docker pull alt@sha256:5f6e50e6c980ab84bfff59e6f392949ba19a9f0c90ef25bc2036bc55d674453e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38617663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:516b8c094f7f290d26bbfeb5353766c1b9446e9aa57fe7cfa72633764eb6944b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Aug 2021 01:09:27 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 17:58:23 GMT
ADD file:4915390df5586ea7d0b637783936196908facf3922fa8db69f3fb39d7a95ecac in / 
# Mon, 06 Jun 2022 17:58:26 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 17:58:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:821e215670c1f25909eacde0295daf91a2fd53fa3ac6bf4003ccfa6ed4e1fb92`  
		Last Modified: Mon, 06 Jun 2022 18:00:18 GMT  
		Size: 38.6 MB (38617471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18dd65b0c14ff195b400d9a87850a6e9d90125d607e88d8075c31bee8befc7f`  
		Last Modified: Mon, 06 Jun 2022 17:59:56 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:2da182b691e6b91f5b9460de1f2e1397a9532a92c38f232528be1d08c657e916
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41909762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0f29a7da37424c795a464116fb9fe1597e61de8cb427a9d014f05be0910145`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Dec 2021 16:01:29 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 17:39:55 GMT
ADD file:6c76bbb2cac15c7486a1a6e833f3f7f35a0f0332c00a2896bc75e134a0093148 in / 
# Mon, 06 Jun 2022 17:39:57 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 17:39:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:66be0241a7903dfc5f98922c16fd86cd7270cfa7082ad47a66fe3fada8ee1c8f`  
		Last Modified: Mon, 06 Jun 2022 17:40:47 GMT  
		Size: 41.9 MB (41909571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ac77e1433ac53a6e86c15280a0159c36e799327f306e93a666fae6711abfd`  
		Last Modified: Mon, 06 Jun 2022 17:40:40 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; 386

```console
$ docker pull alt@sha256:47f8626c83db8c79a065554c0a7dd61da8d76ec8f35597d8126241c453155129
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43251715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9168a51fc4500820f97bf052592b5f3cfc3fb985a64ffc6d5d284c02178f14d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jun 2022 17:38:38 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 17:38:52 GMT
ADD file:2c7ac744053752c2eb294394ca698fedec80c4af2d2feff4781947ca0f21d270 in / 
# Mon, 06 Jun 2022 17:38:53 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 17:38:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ce5ee804e260ab81ea6cccec5fbfbd258e7832dd8e0af32c5a13919d538c6efd`  
		Last Modified: Mon, 06 Jun 2022 17:39:43 GMT  
		Size: 43.3 MB (43251526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90969c85e33d2b84295aca2e8b00377fa08c95d9611278b37329b217deeb48ff`  
		Last Modified: Mon, 06 Jun 2022 17:39:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:p9` - linux; ppc64le

```console
$ docker pull alt@sha256:008cc57a321cc26302f795d6ef4109640e644320a0891e471edea44b22a32961
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46785466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e299492bdae17fae2b168af13070de37cd2496dce1db4fcad8bde3c6399942`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 09 Feb 2022 22:24:10 GMT
ADD file:44bdfa4ab5fa246180def4ef97c1f80a94c17d26366ae21262e9e0e19c443f42 in / 
# Wed, 09 Feb 2022 22:24:22 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 09 Feb 2022 22:24:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd261e465f329dea41ea59148a786f5cd367c56909f8946c08d5dbd31a255e24`  
		Last Modified: Wed, 09 Feb 2022 22:25:38 GMT  
		Size: 46.8 MB (46785272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d9d9493430553a622e1b3e5977165480116e80dd961100d224157584b20db3`  
		Last Modified: Wed, 09 Feb 2022 22:25:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `alt:sisyphus`

```console
$ docker pull alt@sha256:522fc56cab87c24b385e990dd2471d77cc57bf1590013885f9d4d8348f84472b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:sisyphus` - linux; amd64

```console
$ docker pull alt@sha256:bcaf63d09de0e1e2e42a04817a2a7e541e94f8858235a03789a6c00c9151c54c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42101073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da81890842f38eac308ec785de82dcfedd5c1b174482e4e7386a3ff537c0bcf5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 09 Feb 2022 22:20:09 GMT
ADD file:fa6b11057bb920616089ae6766f3d1b7f8d49555a9a7541d533c6c62ff822b11 in / 
# Wed, 09 Feb 2022 22:20:10 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 09 Feb 2022 22:20:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b9cb3d64353589bcb25d988689617e9dda18d6bb15fc228910d1748498c0799a`  
		Last Modified: Wed, 09 Feb 2022 22:20:55 GMT  
		Size: 42.1 MB (42100881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a5e87d5a50caa36a0e4c4347cb6717e2728facfe342a1a75d6178215e0047f`  
		Last Modified: Wed, 09 Feb 2022 22:20:49 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm variant v7

```console
$ docker pull alt@sha256:04587ea6dd52d70bca70e2efeaeb113e994dce5ad776ac964a79c43c64bad4fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36206422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891acf808fbc18ec80f30c8be01dfded9357463b8dfd6c69fde7340b85638701`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Aug 2021 01:09:27 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 17:58:49 GMT
ADD file:80830eedde472da8dad47b57ef731737420916b54feb91f335aaf4ec48be202e in / 
# Mon, 06 Jun 2022 17:58:51 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 17:58:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:023a1f5f184ced595e85d241ac5c10ac4378d885b737a2911506977dbc2821df`  
		Last Modified: Mon, 06 Jun 2022 18:00:48 GMT  
		Size: 36.2 MB (36206229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f0750e2698bf9ed5dd0ea639a16bfebd3fc51cc5085c695d1b1037f023e171`  
		Last Modified: Mon, 06 Jun 2022 18:00:25 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:7acafbb419c6d6a373e5ff2eb3883f53a94b99e298b73d9c18beb3df3e502307
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37727549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2c57cd81a7b08da443854569761cc62de551da95f86fed9c16fa6450fe16c96`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Dec 2021 16:01:29 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 17:40:05 GMT
ADD file:052a12dc3a8ab0a79622f2e95c4808c9f4458caeb516bdff12cd08443b9beff4 in / 
# Mon, 06 Jun 2022 17:40:06 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 17:40:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9e7c77f5d9542d8d4f1e8ce941f1fe1cb52ce90a2322fc928028c79e21676d3d`  
		Last Modified: Mon, 06 Jun 2022 17:41:00 GMT  
		Size: 37.7 MB (37727357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c2e8c3dcfff42a4d6b930074e9e18e0162f3573bb908389a70f9fe3cc4c2d0`  
		Last Modified: Mon, 06 Jun 2022 17:40:54 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; 386

```console
$ docker pull alt@sha256:21b03ed000320583f729711fabbd3b6e7a1076d3914055b90530dc8d3250247e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39515670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d81aa88a70c5c2ae7d309d0fbea27d72ff0a04df4eb08c06a3c48ee7abcc22a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jun 2022 17:38:38 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 17:39:03 GMT
ADD file:8f22eb8ada92feac739b470e6359d69438755b40b3934c99ece5018d36a7db41 in / 
# Mon, 06 Jun 2022 17:39:04 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 17:39:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:96673e6879f8a007749c492e77ffc37b0e9398259e99de5a9afc99a23cb51c6a`  
		Last Modified: Mon, 06 Jun 2022 17:39:59 GMT  
		Size: 39.5 MB (39515480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f670abd7b17f72395fa8cdae7205fe3f445d7f5df994a7262042141b785e0ec7`  
		Last Modified: Mon, 06 Jun 2022 17:39:51 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; ppc64le

```console
$ docker pull alt@sha256:fcd7841be80def833bf20150a44dc36de6bd203edec439839b3eb1e326e93022
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44859644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b92dc0fdf4018d5c678bc2e65e8758f30894313b0c65ee8683496e6a1c3a3f9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 09 Feb 2022 22:24:38 GMT
ADD file:0e95b682787f1ae30d91ad1bad192ffa42728f818fd1cbe8b5f916334b0afdfe in / 
# Wed, 09 Feb 2022 22:24:49 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 09 Feb 2022 22:24:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cda4c58921d124961ae872951d44169f3d545c9e580698137746e448d8da5ab8`  
		Last Modified: Wed, 09 Feb 2022 22:25:56 GMT  
		Size: 44.9 MB (44859453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659f8ae4991b1203646966f80800b9ee37339042f15fc3b51b2d3e6657d7968e`  
		Last Modified: Wed, 09 Feb 2022 22:25:48 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
