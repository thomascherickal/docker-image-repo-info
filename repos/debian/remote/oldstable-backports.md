## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:5851606ec5d293f6f9208ddf87570cb004901384080ebcd0d30f3375b7c6e5b7
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
$ docker pull debian@sha256:c3227e68d32269cd1417f5b49d8ce4910c53b74a97c039e968b06286e8b3631d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45377764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba51cbb49e16a847a39fef54521434adf3b0078627627ae3d08fd66fa5b939e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:07:18 GMT
ADD file:31fb86c570072fac2b8564f70ad7f17543d70ce5fc8eb8010b37792dc2806d60 in / 
# Fri, 11 Dec 2020 02:07:18 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:07:24 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:380d723a9de117159b9c4efeb81d860cfc464f6e65ebf7f54b134edca5d3dccd`  
		Last Modified: Fri, 11 Dec 2020 02:13:43 GMT  
		Size: 45.4 MB (45377541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdb80e5e4b4cea3bd2b61af6fb97eb600e0340f9e4fed5730501834e0605c9d`  
		Last Modified: Fri, 11 Dec 2020 02:13:49 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:5f50c1527c642705ea52a66426b958a59911b998ccb39c95d46797f2c224c19a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44089786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3869060e8d3d22ac00673406742d7e952039050a405e986f4940c59e8a3e45a5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:44 GMT
ADD file:c61a807cc5b26d2a3bf6ecd8f195b5315212820ea0bc008870c1963f6fcb7e41 in / 
# Fri, 11 Dec 2020 02:06:45 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:07:02 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8e1a116db0d10283a32828a3d5b80ed412a5b0cc7d43b80c89885d907b6bc376`  
		Last Modified: Fri, 11 Dec 2020 02:16:32 GMT  
		Size: 44.1 MB (44089560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c529daa3f0985d694737871c7ea96652044e44e368bb024b86b743c53457c2c`  
		Last Modified: Fri, 11 Dec 2020 02:16:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:877c27f0a5a5fe7d30215e8768ad82cce37b523f4028ffa3613c436da96c6754
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42118162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a760eb01162eb09dd7defc1e7b16a5359e0088ff654d11bf3b05a4ed724478`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:25:44 GMT
ADD file:61b04cd61f39e49a19b30db1bca44fa0aead2080554f231ba77a2f7b1245bb07 in / 
# Fri, 11 Dec 2020 02:25:46 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:25:54 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0a9ae06c3c226905ca79d9b5af5b4426f8cf8bd0a1dcd4579ee501b89be35321`  
		Last Modified: Fri, 11 Dec 2020 02:34:47 GMT  
		Size: 42.1 MB (42117937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5071fa907f093d375231d01091dbeca2e13dc2c45976828580e3cdd0ac3655`  
		Last Modified: Fri, 11 Dec 2020 02:35:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c021a8840f8725e42c78166124369bbf8dd7a20b9d4313d30898586398032291
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43176251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8498744d6fc7b3e697ddc8ba4d1b859c871d8a13b5696d69f825997058eec1c9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:46:12 GMT
ADD file:cae2710fe2ce68aa1148afb8224905a25233bc3841649cd379f2aab0bb31b9da in / 
# Fri, 11 Dec 2020 02:46:16 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:46:25 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:add31b086a36ab8f2c65be1bee039f51fb2c6318d278bbe428333e2d65e43954`  
		Last Modified: Fri, 11 Dec 2020 02:53:33 GMT  
		Size: 43.2 MB (43176024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9da850a8bc2df7e71c133e0144c60cf70a5d021f001821d0f114d273ab0bd54`  
		Last Modified: Fri, 11 Dec 2020 02:53:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:dca1b63063b344a8dc947582b81e6853ea5ad577245b5e6e6202f85076d29c4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46095379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7efe7220180b33886dfdfc4061f781a9ad8b65f9425a947a09dadce80ce491c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:12 GMT
ADD file:f923e11666953431b96e816a4f4f8774cd12c69e4967716bb4c24410b989a4e3 in / 
# Fri, 11 Dec 2020 02:04:12 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:04:18 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:618c63dfdc014147cdc17cd7e36581ddaa2bd59f767b9d15ff728679f7cd937a`  
		Last Modified: Fri, 11 Dec 2020 02:11:18 GMT  
		Size: 46.1 MB (46095155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb665a0fb9cea64019e66aa79ab8a1277494332228fa99340f6c0966b568f0d`  
		Last Modified: Fri, 11 Dec 2020 02:11:25 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
