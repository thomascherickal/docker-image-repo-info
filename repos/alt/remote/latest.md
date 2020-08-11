## `alt:latest`

```console
$ docker pull alt@sha256:e7569229c8775deffa15a0f60f7a5b2a0bea99ea029b22b96383fbca24f2d634
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:latest` - linux; amd64

```console
$ docker pull alt@sha256:28143858965606980b048f66d0e0442b2cd4be4c46badba24bf049470b96add0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42511153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4177157040d644bcfd8b70f4a16fad1c43533c6569d986a4c58c0b1c42b4803`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Aug 2020 20:19:59 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 11 Aug 2020 20:20:03 GMT
ADD file:fa2206aa87d27af7e61782300c6c650e6cb4323662e94edd3a01a7cac25e5d40 in / 
# Tue, 11 Aug 2020 20:20:03 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 11 Aug 2020 20:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f5f59d3f04f02bf1298793f8e3d6b80e662997ec92b48601f6283bb76881c28c`  
		Last Modified: Tue, 11 Aug 2020 20:20:52 GMT  
		Size: 42.5 MB (42510965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73b5b8965c7e28823eab213685a3ebf3c43ae59a790afe57f119b68e4b1697e`  
		Last Modified: Tue, 11 Aug 2020 20:20:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:77b92aaea090ff699eeb824074a51041b1ade8e543c3bcd15becdca77da854be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41307828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da3cffb1bd3b7eb1d1e5d2192201df5a0aee07677ce20b6e542424ba75152aba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Aug 2020 19:40:59 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 11 Aug 2020 19:41:03 GMT
ADD file:f4ab6d4efd3461b5dfdb057d81085c5af86de7b9b74a9dbfbfe542853ffcb1ea in / 
# Tue, 11 Aug 2020 19:41:06 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 11 Aug 2020 19:41:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2bf3c037791bfa67227a82fe9d9339867c85207f48fd0506462c67eb8ab41a4d`  
		Last Modified: Tue, 11 Aug 2020 19:41:49 GMT  
		Size: 41.3 MB (41307638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e85a97f9f9ed7fb8edc944917addeee27d11fd6ded799cc51507b96011769f`  
		Last Modified: Tue, 11 Aug 2020 19:41:37 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; 386

```console
$ docker pull alt@sha256:48982ca6680ce1654eaa0a7fd09118000f0b0e5ffb4a4f1894ab1c10f91e5508
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42659652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83af6cde94ad521775634a89a25aff05a20d0abb16eb970e003eb9e61787c137`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Aug 2020 19:38:56 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 11 Aug 2020 19:39:05 GMT
ADD file:66250de649c8d152f1aecd61512f6c292c5ecad5ecde0b8c1ab52c2114051ea4 in / 
# Tue, 11 Aug 2020 19:39:08 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 11 Aug 2020 19:39:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:eed7d6dfc59ac45097a91b6551bde9c6cd86ddad12669247e2a35bdf8853b3d6`  
		Last Modified: Tue, 11 Aug 2020 19:40:02 GMT  
		Size: 42.7 MB (42659461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117805cdd0a72f4d8d4cfdc703088e441f42f2bd6c8c2b03ea10ce55e93aefb`  
		Last Modified: Tue, 11 Aug 2020 19:39:51 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:latest` - linux; ppc64le

```console
$ docker pull alt@sha256:4d8a128b7c2e19c413a1335b6ff2d061fe1915c3d1da6fd762485e756ca2c6bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46174380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8031fea98a988c38b1b71a3be296c6dfecd92adf8344628821c0f7ddd3f983c3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Aug 2020 20:29:27 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 11 Aug 2020 20:29:34 GMT
ADD file:27ea35c351886e161ec81f839ebf4ea563b8cc74a3ec0763a5af2964ca2fcb8d in / 
# Tue, 11 Aug 2020 20:29:54 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 11 Aug 2020 20:30:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c79ff3f45e8d56dbed10328416292bba1a02433a9394d7a568e92cd455f9bfec`  
		Last Modified: Tue, 11 Aug 2020 20:31:34 GMT  
		Size: 46.2 MB (46174192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcceb213bb5847674da8e3ea28b5aa90492e3fc3ba42636bd074cc569616f24c`  
		Last Modified: Tue, 11 Aug 2020 20:31:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
