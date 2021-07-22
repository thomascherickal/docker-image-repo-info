## `debian:testing-backports`

```console
$ docker pull debian@sha256:2a88beee4d9df21a1e28c7a6dc3328113be8be51df9efa5e565afdadbe8551ef
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:6a5d7b0f663809bba00ccec0796bd497ce9bc2160d64969cb3699a007af99812
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54904948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d73ed0950d35a1b785418cee2c4ecc5a012f8ec32197f83c57a3dcffe92bcf1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:30 GMT
ADD file:aefd1b2aad4a1d98fd82d86cab1e66f8f172c748e69090a4938ded7681a5fcfe in / 
# Thu, 22 Jul 2021 00:47:30 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:47:35 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7b303595d9b321a9020d0ddbf1dea4c83237e2367117606a8d5466c446714ba1`  
		Last Modified: Thu, 22 Jul 2021 00:53:44 GMT  
		Size: 54.9 MB (54904726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883bf758bb836115654e2248d90f04c1c1c43c882ca86109fbb7d11e2560f2c1`  
		Last Modified: Thu, 22 Jul 2021 00:53:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:1ad2a3dd5daf9368f90c94a5309f3be77ac67d875d2c5fdddfebb6c50b032f4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52443308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa5c89a05aaa06b3f192b2794e3c3949c92df2d2afa7a3fd8eb169a1c954deac`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:54:03 GMT
ADD file:5e19a4394904071529b5729e9018a5bb96db44252d06a1b3c648dc5c373ffd7b in / 
# Thu, 22 Jul 2021 00:54:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:54:17 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ba22fb506b8c979b86ff240abfb3d82fd7398d96105b769db6f5990c0021356b`  
		Last Modified: Thu, 22 Jul 2021 01:08:00 GMT  
		Size: 52.4 MB (52443084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc6de6916e21fa0913b7abe9fec6c95c2d5295eae02ff3e6dbe656e88b6c53f`  
		Last Modified: Thu, 22 Jul 2021 01:08:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:befdd2274269ab7f6b490d27a2ccf4181c865d2728010487fe0b3d7c3f0ed4dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50107792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7736081bede5e2c492d506ac7abb713b21571954d4ddfa6347ca56fdb008f96e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:07:55 GMT
ADD file:8e406ec082d83611c16c0769a00fb68a1dd965b5d93a99eb8a874b2bc5773d63 in / 
# Thu, 22 Jul 2021 02:07:56 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:08:08 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:28e5916571f73d9b8f9ba1e671b84158efcfccf96ee5f20c9b4626098c30e3e0`  
		Last Modified: Thu, 22 Jul 2021 02:22:03 GMT  
		Size: 50.1 MB (50107566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398c00f0430b5e2764e4f66431a420680ee5d164716183218205d6fe1f7485ff`  
		Last Modified: Thu, 22 Jul 2021 02:22:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:e36cc251b5b3caa35f8d758c0c6c81d4446d172c522761e7e00973a9ca5bf7b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53590428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a9a6d163bcc643e458b2b28f53efbd92cd57c2b6050b09cacc12bc6a29f2a65`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:51 GMT
ADD file:e33f1c12a015f577adbcae333030de59322c78d065b6a9bc023ebbe8137f3884 in / 
# Thu, 22 Jul 2021 00:41:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:41:56 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:219bbd9a92d615a2d512d8204c52d9cba7f032064387678c47123983ca063289`  
		Last Modified: Thu, 22 Jul 2021 00:49:16 GMT  
		Size: 53.6 MB (53590205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462f310a18c37d15fa7cb984d7d6e5519aad49132daddc0477ef132bb0275818`  
		Last Modified: Thu, 22 Jul 2021 00:49:30 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:f91c1262f81688e2f27ee2ecf3299be4b00af570cdca780d39724897842f102e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55913271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb7cc72d7dcf8eedbf82c430006c99be1df32f335674c6cdc01f163485e1454`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:00 GMT
ADD file:a222d166a6ec259be4acf5812990acf17066a5996e50c7a2ca3e43f3d78cb89d in / 
# Thu, 22 Jul 2021 00:42:01 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:42:07 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a7fc36854f9c662efae56a20832f2cbaf7bdfb3eafa64674961d60250f0e1ba1`  
		Last Modified: Thu, 22 Jul 2021 00:50:20 GMT  
		Size: 55.9 MB (55913049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaeb0d4c9b96ff714123d229db8bdd03ff83ab8f0708c2713fc68bad38cf532`  
		Last Modified: Thu, 22 Jul 2021 00:50:32 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:2151677995d6d035a13d0e583a1dc5bdd7f5aa210b313a0ba883f8e60f6feb4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53156488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1582da37b4f6e36e2fd15044fea85df4f4e843f3cbc35680c1410a34ad7e0bf5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:11:43 GMT
ADD file:3e600ef468144edc10d6c5f69c2b35ff5b004c495354b96030778c09dbaeffea in / 
# Thu, 22 Jul 2021 00:11:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:11:50 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e40d8e1fc952b3849ef186ecddbf8984db96900bd347edbbbc0bca19d2d917ac`  
		Last Modified: Thu, 22 Jul 2021 00:19:28 GMT  
		Size: 53.2 MB (53156264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd64bbfe313e36a508ccdac8e9ff623b76df61dccdc6d2a90797ea8d1ee7fb9`  
		Last Modified: Thu, 22 Jul 2021 00:19:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:5fd2afdac2596df7d99129394363ea2b8783b8ae8f15d352fbb0f27332d38518
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58813523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3b876abfc3cc159be1e6ebd01d411db761da25148d687706619d8f49361429`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:21:17 GMT
ADD file:609f34b74745c6e0ad3453b3e7043b6aa9a8bd1f08450e5dacc435f2e02cfdc1 in / 
# Thu, 22 Jul 2021 00:21:28 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:21:53 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a9effce78a0f7eaff718bcd66572e6000ce0a0c44f2947bbc1908696da72910b`  
		Last Modified: Thu, 22 Jul 2021 00:29:51 GMT  
		Size: 58.8 MB (58813298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8be79aa6bc6ef5fe2bf9ba46c407b0accc4a0b1e3aa1e50e39c4e690878e4`  
		Last Modified: Thu, 22 Jul 2021 00:30:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:59b6266382b1759e107daf55617b9eab87cdb2ba20a1ec3903469c222ae5b55a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53183701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c81ac028bef9c0144418dde395f539610cd7d445fb760484c2184b0fbeb5bf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:44:05 GMT
ADD file:21b5f07587901992012f9aba1a8fea81bde8e4d0178a7b01221b7a6070bec5c9 in / 
# Thu, 22 Jul 2021 00:44:09 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:44:17 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e3700ef60bb30345145fe56d1d43ec09db7b1a70ff7852b92d2431cc9cb59352`  
		Last Modified: Thu, 22 Jul 2021 00:49:37 GMT  
		Size: 53.2 MB (53183480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8750fe02457d6e7ee2d1462d3a6f55fed8e56ef1f49400d13d1b54e70b250faf`  
		Last Modified: Thu, 22 Jul 2021 00:49:45 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
