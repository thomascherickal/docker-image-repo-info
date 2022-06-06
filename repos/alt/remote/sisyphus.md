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
