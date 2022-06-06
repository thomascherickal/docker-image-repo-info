## `alt:sisyphus`

```console
$ docker pull alt@sha256:bc3f2617882f3e08f2629a650075f0be5e1ea4911a61aad7f6a77d55ec079e3c
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
$ docker pull alt@sha256:89411c50d74de52e7c154ad2cd7bfc5253320868639f015f19ab9955dcedb9cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.4 MB (39402189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d48f4644518cd96ffe1de6cd0333d2abc8312c0e4449e03b58b1d480f0f5905`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 18:20:11 GMT
ADD file:c766f7ba01021947eff8d45c9ba6f3faf222e21110bcf25c511b40356d1b9ead in / 
# Mon, 06 Jun 2022 18:20:12 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 18:20:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:12717fd4baa07f26f23b37553ef73b522213e0dee2759d8d9458e10df2f8d25f`  
		Last Modified: Mon, 06 Jun 2022 18:20:58 GMT  
		Size: 39.4 MB (39401997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b39ef1520ddb0b77af8989d108023f5232aa8b9ecb6f39b53e8445a97931716`  
		Last Modified: Mon, 06 Jun 2022 18:20:51 GMT  
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
$ docker pull alt@sha256:a4c7e3ce243984d79097d4c4a85a1b485460089c64360a2d22b62fe9824f5760
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9defe8a91d3b2d155938cfbf4b032b33a57d7e5f859fc968c4ceb4eadc5fb1c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 06 Jun 2022 18:22:29 GMT
ADD file:8b4194698b84b02c22795e52973915083085322730a94dc1c0d1c3f092b088cc in / 
# Mon, 06 Jun 2022 18:22:39 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 06 Jun 2022 18:22:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5a3903d47bc382470ed3c3ed7b654b952f648c5644d8b8bcdae36e3ae435d5a7`  
		Last Modified: Mon, 06 Jun 2022 18:23:52 GMT  
		Size: 41.7 MB (41671341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffad4170ea721393e9ee67f27834e1be6afd208d79b1ece1e7d719839e91f65`  
		Last Modified: Mon, 06 Jun 2022 18:23:44 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
