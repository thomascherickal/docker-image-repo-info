## `alt:sisyphus`

```console
$ docker pull alt@sha256:1bb710b811f7f2f10cde59ee80c4587f86a1ced20865b200a59154bdbcc76009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:sisyphus` - linux; amd64

```console
$ docker pull alt@sha256:c0211a75fcfd36fc52bd5eb32544ec96265fb8ecb970875433e4092b7bd87a88
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42375154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6e137c76ade141761c2243ddd880e958fbe821c29b67bfb437657865f675e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Sep 2018 21:19:34 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 13 Dec 2019 23:20:55 GMT
ADD file:4f19a38fab38f8360100bcec2e0408c25539602de95ec3382773825ccb3a3e8b in / 
# Fri, 13 Dec 2019 23:20:55 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 13 Dec 2019 23:20:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6f9beb08dc8d7d62afd9a55c11e796f14f2dede70476cbab99e62c7e47aad466`  
		Last Modified: Fri, 13 Dec 2019 23:21:32 GMT  
		Size: 42.4 MB (42374972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992f9a02479e4e2d93f26eedc14cd4613e83375b58446876769905ece910bb8e`  
		Last Modified: Fri, 13 Dec 2019 23:21:24 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:5b893675078f31b0bc7216ca2c90d73108302dd4a28ccc304ca96ae9186d39c1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41306108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029742de4e99c7c61c0eb63ca4148957946d1e9fa1cf1534b5cdd14a51bb3ba2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 May 2019 22:39:34 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 13 Dec 2019 22:40:19 GMT
ADD file:3a55fb343d5c1e9866c190a45f6ed01ab539e65b6af83484ec18f175ca741417 in / 
# Fri, 13 Dec 2019 22:40:22 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 13 Dec 2019 22:40:23 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dd75d82833b1ac700959183e216aa3f793f0389cb3b52a525657e925d879afd4`  
		Last Modified: Fri, 13 Dec 2019 22:41:00 GMT  
		Size: 41.3 MB (41305924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90c499664f67cb894d21a7d3b67a0b50ac47b76324272a0528ca7018438819`  
		Last Modified: Fri, 13 Dec 2019 22:40:49 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; 386

```console
$ docker pull alt@sha256:c446cf5e0eb73d3299c657c988c8d6f9820ef3fae534be8fd7d8e60845cc2f05
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42815645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2eb8e80005441f272b78dd04445c9edd982d8ccc74aea9947d26c78b59d05`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 Sep 2018 10:38:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 13 Dec 2019 23:39:29 GMT
ADD file:0deb4a2c4eb4a4b6633678dda0c6eb4643c6288351eaac95e39578e10f38937a in / 
# Fri, 13 Dec 2019 23:39:30 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 13 Dec 2019 23:39:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7d11a6378cd04a452f4d502d4e316187d4e6cb3596d57cf65e2cdeabb7ce15e8`  
		Last Modified: Fri, 13 Dec 2019 23:40:18 GMT  
		Size: 42.8 MB (42815463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e67533437752a6647661ab02af9cefc3ed300ab44873d4aadb2d0881d574da`  
		Last Modified: Fri, 13 Dec 2019 23:40:05 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; ppc64le

```console
$ docker pull alt@sha256:50dbab36635fe39ce0478d51359af0bacead1c871e7d0410db1112e2b2b444e2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45980294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b9a706fcc943446923d69f5e44bcec1e2324f64fd2c73c3cd827d7d5ce9b7a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Jul 2019 23:03:07 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Gleb Fotengauer-Malinovskiy <glebfm@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Fri, 13 Dec 2019 23:28:56 GMT
ADD file:775e42d8b94f8000aa91f09e044d81512bb39d132cd55da96571e659201dd341 in / 
# Fri, 13 Dec 2019 23:29:02 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Fri, 13 Dec 2019 23:29:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f21e5c19aa4a0e8af2854d79a47810deda11e779c7915a8b6a8821328bbf5593`  
		Last Modified: Fri, 13 Dec 2019 23:30:10 GMT  
		Size: 46.0 MB (45980108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4252e9e543879b0cb367d932e4e2e201c9056b919e3588a12bde9cfae0ea717`  
		Last Modified: Fri, 13 Dec 2019 23:30:00 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
