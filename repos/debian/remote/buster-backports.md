## `debian:buster-backports`

```console
$ docker pull debian@sha256:46653df4de477aab61afab0d346d45ab5c621fc6ba22fd040f24a5670fc6745a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:bdccb9d74304cce4a1ae3a7bf765daf6247eceda6852aa6d2a04de0675510932
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50435840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61766c02abae2d3cf15e6172a83fba27c2110d13858885c86f14ee890750f0e0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:20:31 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce21183e17ccb1849cf522e102982793d882ca38badfce9f7bfb38d7e73fcfc5`  
		Last Modified: Wed, 23 Jun 2021 00:25:27 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:ab722863706be91dba0db8396b45e3b38c85a945572b3de1c3e97e02cf292af4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48153922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feebdefcd1191c3e05f7725d7eecea5db0af0bff9d419cf957f83c1de6938dea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:38 GMT
ADD file:cbb86580a65f84ec39691b126a21ef374bc4f2f2fe5c27979134aa940d6326f6 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:49:55 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3b0b1347a8a3d1156e417fffc79192d014d9cc985fa5e55a49cf67c21e7a81da`  
		Last Modified: Wed, 23 Jun 2021 00:00:57 GMT  
		Size: 48.2 MB (48153698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f67243413bc7a0638f4f53350fed3a372eececab8a91caeddb8e01eab432ba`  
		Last Modified: Wed, 23 Jun 2021 00:01:22 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:4e35ff30546682229d641509099904d28f3d9bf40bb01b2b754bc65a88f46e1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45917707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a0d4a47bb9af297115c8711d96cb2ad3f0b51cac2beee9369d0ed7a490a73d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:01 GMT
ADD file:3edc1a2322b55593b3cd8e935ca6d837e7618bcaaab27a09c9822728f8272ce0 in / 
# Wed, 23 Jun 2021 00:20:02 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:20:17 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a3ac2852d9d20585eb4d19973a45b69522d16832456ea5b52f0298b2937afc09`  
		Last Modified: Wed, 23 Jun 2021 00:31:04 GMT  
		Size: 45.9 MB (45917482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5511d08227384b8614a3930521e2f4b375af75f15575965bc46dc8b92b5390a3`  
		Last Modified: Wed, 23 Jun 2021 00:31:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1372c4eb93404f46864c955c3206f72021de9cc32f99815e038012394d9ec1e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49222208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50c68cde88b27d18544b60ee93a34f3da03b9a3c7d54c1645facc15fce1d55c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:49:32 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc63555c17683a6fb64297d43151e1bb791f57d459eb65cff2577054a8c52886`  
		Last Modified: Tue, 22 Jun 2021 23:55:12 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:23043c759f32364ebb6c6a1d827936912b2ca42b46d3693535eb0fac36a393fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a722b22f44dddf7bde9855e957f7064b5925987958f9c28c64b1512af4100d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:18 GMT
ADD file:e69bc1dee51190c812075d4b4e8ba1e67f67250af9f2ddbaecaf2c9316a07bbd in / 
# Tue, 22 Jun 2021 23:39:18 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:39:26 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c4109247a8f9a72ed1435270480f72d6db8d6f038c6941d86a94f4dd0be8f789`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 51.2 MB (51207098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e640814753453b0742d69a823165604f872287052e84c312c7e9649f4806f3`  
		Last Modified: Tue, 22 Jun 2021 23:46:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3e743d532ff3db021448b54952d7a5e8638c210e7b44c84f07ef507c40e4b84a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49080560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fa8d3995ee15c6e8f92efed6b13ae4e3825a15992da0a436431f13931af95`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:06 GMT
ADD file:4673ab387e5a746227250295a00343ac2d03d6aafdc28d019a9bdf26bb97c8c8 in / 
# Wed, 23 Jun 2021 00:09:07 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:09:14 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e3f0127f2925aa298e3074daa756fb98cf945e5aa11c7dd3cb6d66cc3ba2c7ac`  
		Last Modified: Wed, 23 Jun 2021 00:15:06 GMT  
		Size: 49.1 MB (49080336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7aae626f93d9446478735ef48b994caf52154b8a82196e9d09e0ea3d4f42c4`  
		Last Modified: Wed, 23 Jun 2021 00:15:24 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:e2babad0b2f8faed5223d0cea73798503c3035b20a6f17022fd8a340b07ec56c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54182688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2110b95f18b6feb6efee06d567d393702825eb45fa89086ae3d51b410f36dfe7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:05 GMT
ADD file:b73f8d66b8be6103349949991124c7d82e38589b2db6212e920cb3b6d5ceefef in / 
# Wed, 23 Jun 2021 00:30:13 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:30:28 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:83f72610ec8bc58c0c3a70f0bdf9d866e8d0156845a9aa24bc0ed2fdaf0fd8b4`  
		Last Modified: Wed, 23 Jun 2021 00:36:35 GMT  
		Size: 54.2 MB (54182463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35d57cf5349824f448ba6646dce6fd5a59e08d946df1982c9922fee0aa76bfb`  
		Last Modified: Wed, 23 Jun 2021 00:36:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; s390x

```console
$ docker pull debian@sha256:1c2238b8faf013dc40c17c392b7ae5816d37e5d212d930a3da72f2b42aa4ed39
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49004149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2b8af74b5af8b2b160c8cde656cc44bfedf3117507183e553c294376d00edc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:14 GMT
ADD file:b935574081a3fbceb534880a35e5245e10c52a3b9d70224811e221b4c6254cfe in / 
# Fri, 09 Jul 2021 02:50:15 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 02:50:23 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2b8d113de06cefaa0768df3e10da0c3b8272e15922e18ea75b0bb4dee23b551d`  
		Last Modified: Tue, 22 Jun 2021 23:45:28 GMT  
		Size: 49.0 MB (49003924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d86765516009e98a3e9ce1dd62ae501fa231b981b61f1f9b6d54fe5b01db9ba`  
		Last Modified: Fri, 09 Jul 2021 02:54:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
