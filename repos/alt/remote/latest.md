## `alt:latest`

```console
$ docker pull alt@sha256:e4a494493586361cd2e9a6198157735e6e7e541d391e84514a8f1cd0610093a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `alt:latest` - linux; amd64

```console
$ docker pull alt@sha256:666b4a11ee22271b752f80729373a6a857d67837d6f552f8e6450733bfb7b6a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42530436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33cc2269df5bc937df4e9b412104d8e74939d0094d96936fecb4924a58d0d0b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Aug 2020 20:19:59 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 01 Feb 2021 20:19:45 GMT
ADD file:3dd849f8ac6cabe235f598f331a40467af01717533210592ef4f4e0e6bf48bf2 in / 
# Mon, 01 Feb 2021 20:19:47 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 01 Feb 2021 20:19:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:59b06b72fecf1e58df7ff0dffcc1e133da63c34d54a46af620e1585f7c401bdb`  
		Last Modified: Mon, 01 Feb 2021 20:20:34 GMT  
		Size: 42.5 MB (42530246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3007a52edd48aa2315e94c595d1e8dfcc6bc18211e51fd3361e7eeff19881a`  
		Last Modified: Mon, 01 Feb 2021 20:20:26 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:e955faec3f8f11324dfa4a4d864f5f45868e9c5460e8c294ca9fe798836c18b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41328146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85087d3e094759f08d977c43f5a6e907fe9e308e496458f6378c7f7a1d05b3da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Aug 2020 19:40:59 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 01 Feb 2021 20:52:52 GMT
ADD file:15b783f7dc1dd5e33ab77cc1e4bc05cc6a7f516e22cada40d2df962b89235dfb in / 
# Mon, 01 Feb 2021 20:52:56 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 01 Feb 2021 20:52:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1e9e2110c1578c23fbc40cf07677a803524a09a39306a63240de0361e7a35a3c`  
		Last Modified: Mon, 01 Feb 2021 20:53:35 GMT  
		Size: 41.3 MB (41327955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5a3b500af59411ea0f64e8ee388f1ca42112878bf00c372a07bc1f6d1629d3`  
		Last Modified: Mon, 01 Feb 2021 20:53:25 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; 386

```console
$ docker pull alt@sha256:21069f509a7859230e8bd72a652374e451e04919935384c1ceccaaafbf9ab23c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42722346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e37a6a8ed1c0e03021ab4ca119fd5bd5961774ce28ccaf217916742638b8a5e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Aug 2020 19:38:56 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Mon, 01 Feb 2021 20:38:35 GMT
ADD file:f2adbea45d64b87c5724e14daf4caed76d290fcae4241c84ad4075968261790e in / 
# Mon, 01 Feb 2021 20:38:36 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Mon, 01 Feb 2021 20:38:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:23fd38d00e7523296f6450cb8ce0d4d304f476a74ca7fb369a34813fe674a9a3`  
		Last Modified: Mon, 01 Feb 2021 20:39:30 GMT  
		Size: 42.7 MB (42722154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbe2879e0212cd7bdaacf93c22f3029e654e0014ec423a6557079f4c21f459f`  
		Last Modified: Mon, 01 Feb 2021 20:39:18 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
