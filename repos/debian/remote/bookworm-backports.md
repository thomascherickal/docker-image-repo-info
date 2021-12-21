## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:e38d96b5b0a5c0f1b32a3792fb7b55c0a88a131a524a2d8d449949d127af6485
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:1d8f26f94269c544c3c690fdd880ef33a026561fd2ded3114e70fcd8357580a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55599028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5554a6f460ec002fa1d82751f3015d5779c9ddb82aa5f7e6cdbaa4ff9ce09dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:09 GMT
ADD file:15e5b0a35c4fc7a5ae0bf08f713bde738d2cfb06a30b8bd5780fabafb91d934c in / 
# Tue, 21 Dec 2021 01:22:10 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:22:15 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9aa4f47c6909274e4d7f0b2429a7ad24598b19c01da78245a16a3176f9acf847`  
		Last Modified: Tue, 21 Dec 2021 01:26:44 GMT  
		Size: 55.6 MB (55598801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2099a22743fb705d95cc1f13086e834534ff8bd3a71afc9c2dec3dea55e3c96`  
		Last Modified: Tue, 21 Dec 2021 01:26:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:7d56543eaba8e307e816df58150f0042a4b313f4b8049d62d7bd4db9b3702029
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53058775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b84c7029d7768546426397242ac0333262c34a13399a6e1874761051f8bff66a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:48:58 GMT
ADD file:06611eba7b36a7e9c8c68f1d8c97d596b024eefb00a7b0638c9ccbeb8a6f9142 in / 
# Tue, 21 Dec 2021 01:48:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:49:12 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:13e93eb93ae4e3d37ac97bb105a341f9c56baf0c8b9fe4707b27ad57f5633247`  
		Last Modified: Tue, 21 Dec 2021 02:03:43 GMT  
		Size: 53.1 MB (53058545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9e64d64d05d715e319d8ece4129f593caac7ab6ef497e3d80cc31c845b4d3c`  
		Last Modified: Tue, 21 Dec 2021 02:03:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:754437f2d1b75e9104554e4472155f0dfb70d03e1ca005545b9213d9edcc88e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50668211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd7aca774f43f50b0740ba35047a72f2a8f435b879f1fdf96aeac3ccd6105eca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:03:39 GMT
ADD file:bd5233b326b625660d820fa962832e6c5413ff9a56f64a6f072b9a9adfc545b2 in / 
# Thu, 02 Dec 2021 09:03:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:03:52 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4dcb906f06af542b010e092a9a4d4ad8ccb110debf57beb0d4ded9baa51b82a1`  
		Last Modified: Thu, 02 Dec 2021 09:18:59 GMT  
		Size: 50.7 MB (50667986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fb9f8a8eeb1a11d5a1d14a1b1b29f5559ddd3f9cab664e2629883b147b5ebc`  
		Last Modified: Thu, 02 Dec 2021 09:19:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ef92d8dd8869716c25c8211f004ad7fb81b17536f5f01e4a6c6471b36844188d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54598302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f4a49f9f3d9135af0761def00dcb9fd3943451307f014576279da2ef2ed78e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:41:45 GMT
ADD file:c64482c2e0b0935b000b024e468499d2586b78ca5c64b035ded7ce33f1dabe14 in / 
# Tue, 21 Dec 2021 01:41:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:41:51 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:be902f523b4c4ddf53ea157e340cd7ce836ec2a0952d6f18602467352524e312`  
		Last Modified: Tue, 21 Dec 2021 01:47:42 GMT  
		Size: 54.6 MB (54598073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d613d2f08ea4778422bd2ba397bee84eaebf30ab00a6f71dd8a839176e4be3e`  
		Last Modified: Tue, 21 Dec 2021 01:47:53 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:340665a87da6a9ceecdb7323b9ed73f1bb71ea74f6fc3d461ce72e3cc86e2c4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56659109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc238df9b2c65d0ba3edbfc1c0c15bbeaada1afecc84fd894ea1e695617a9ae5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:06 GMT
ADD file:f5394800b665e61b6f319d6dffbccd66c1172d4e9fd1db6ba962ef5aa177c353 in / 
# Tue, 21 Dec 2021 01:39:06 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:39:14 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:75388d3fd5f848339be12f5cd41cdf79effd086f4656396bfbac934b7f1f715c`  
		Last Modified: Tue, 21 Dec 2021 01:47:16 GMT  
		Size: 56.7 MB (56658883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40897c697d656807f44be27613477b212da6f33281e2ed10edabecf54fbbc485`  
		Last Modified: Tue, 21 Dec 2021 01:47:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:08a20159ed23ba78318d847b7fb8a5454caa8a351f8a6095c9833ae3e4191981
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54269820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb1d2a8812283847cb5aa15b80cb4ed890154847feef633408f59f14cdfc4eb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:07:51 GMT
ADD file:2b78b392bcc6daef3d9c93dcae4adf8b84cac89c57ed08bd43854d23774078d6 in / 
# Thu, 02 Dec 2021 03:07:52 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:07:58 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8c4a35c3e932252ccb2418c1bc14531f11d21f13ba131d0a52cd9cb690dc9623`  
		Last Modified: Thu, 02 Dec 2021 03:15:53 GMT  
		Size: 54.3 MB (54269592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a8ca1adf7665d8b56eb5f4dee37f9b21d2c8d750c93da7939bf44e64c9d2e`  
		Last Modified: Thu, 02 Dec 2021 03:16:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:b4b32c9d948ab084825d28c7273a21a32145d53c80819d87c5b63009c030ac0f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59851596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64e1c9aa75865eb49b4409c88da5a5d5b7c24532c24a7b63da5a3fa1ac6fd7a4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:51 GMT
ADD file:b1221d684becfd74b167e24d774eb6099d264be14e0abd56599cb6a39c9eed74 in / 
# Thu, 02 Dec 2021 07:20:00 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:20:18 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ad94a9a32e9daafdd41e8b09d1671e7fd6b6d7cff42957db5b36cf5fe8276d1`  
		Last Modified: Thu, 02 Dec 2021 07:29:36 GMT  
		Size: 59.9 MB (59851370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bfb2b607328eb15d7ac51fdcb7b40674219e70a36bafea9f10c090e469c338`  
		Last Modified: Thu, 02 Dec 2021 07:29:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:b0f107fe07dc3ae4711e2e13552787614cb3fdde491d3b2f61d8719d4d96d9b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53888670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:464b229ccf544e5937092177ec5c892b18376a61d8639dc4dc55aeed45e9e3de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:41:36 GMT
ADD file:c9626c75e4b53a0e71f37a2a3df45699d003ae102e7e3eedc97afe7897f82180 in / 
# Tue, 21 Dec 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:41:49 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:341c5a56ba0f7b7f22f0613addb31ee3342e410686dda8753a049d0bd1f319f3`  
		Last Modified: Tue, 21 Dec 2021 01:47:23 GMT  
		Size: 53.9 MB (53888441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3798eab2774bbc8f051eeed888c6fdc1837bd54d7fae09de3dd744090b1da02`  
		Last Modified: Tue, 21 Dec 2021 01:47:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
