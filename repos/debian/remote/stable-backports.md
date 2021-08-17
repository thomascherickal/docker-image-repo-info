## `debian:stable-backports`

```console
$ docker pull debian@sha256:ce99b3eec3294850a73f60f381f093e07f2b64303ff2f841e21d36a4774466b7
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:f67d2ba3f6f027a9f480c6b9e0957eb06202d1979bb21d1d749743a96ba5a274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54915181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1162604d338aa762554ad38f723a44c15aca88f28065bced673d6679c6b8c43d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:29 GMT
ADD file:d78d93eff67b18592997e4a9cfe93a931f491d5746b1395757900a8727a08e95 in / 
# Tue, 17 Aug 2021 01:25:30 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:25:35 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:605e0b7dff222134e8a75c955360e1f18f9d47f5126da3ba0944f0189b330254`  
		Last Modified: Tue, 17 Aug 2021 01:32:27 GMT  
		Size: 54.9 MB (54914960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd2e319ee0730e8c0305827411cd3fe8bc42e35b1c37f59a167385bd399ed36`  
		Last Modified: Tue, 17 Aug 2021 01:32:37 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:7f5e497f3fcb70c50152b6e5bf3217395ceec21ab2f49830a0d3665492e4c5f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48153474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3147152f60e647e2efb4a41ad545bd29fc7680162446c49e3f9a98b2b140cfa8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:52:10 GMT
ADD file:f3d7275062c305b42debf8dfb48fb5f7687526caadc936bd39be78ae659a8085 in / 
# Thu, 22 Jul 2021 00:52:11 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:52:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:21bfff09e1240faaf3850f5e2a8e7974e604b2ee5ad6e2bd6b1be5c63e2ca611`  
		Last Modified: Thu, 22 Jul 2021 01:05:23 GMT  
		Size: 48.2 MB (48153249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9633d3d1bd6fead031cdf0d43bcbe628e65b1e1a9dc2a0f8522009b1dfbcf48f`  
		Last Modified: Thu, 22 Jul 2021 01:05:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:49ed45085680a69d36c250586e03a84923add35ab77c3fda25f3dae663825dea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45917467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cbb0733e0193686872c35a9d07213d44938d9d1888684dbced3085f063b7a8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:05:59 GMT
ADD file:423828ecd1a5225b4d393c372890ff1e90a17fcbe15befc06b94a71fa843ff99 in / 
# Thu, 22 Jul 2021 02:06:01 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:06:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d0aea515a0eca88bed4155cf5a5ed0cd354b107f7892a3eb1d09d93bda2a2722`  
		Last Modified: Thu, 22 Jul 2021 02:19:22 GMT  
		Size: 45.9 MB (45917242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bfac2ff92d5ae0573f40cbd227b707227d5ff11fca1b5959ac52d92bcc6ba5`  
		Last Modified: Thu, 22 Jul 2021 02:19:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:4edc325a8e0f60086ccc3a92bd7e35b05f2457db47cad8de170fa482b24f0bb0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49222343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c3b50bfd1e6d9a6cf9c953d80b08dbae9fa8afeb44d888d30133d6ad9390c5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:04 GMT
ADD file:bc14393dda57541decd3b535650114a20bb2a646adbfcc2b0649fa41278df4e3 in / 
# Thu, 22 Jul 2021 00:41:04 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:41:10 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4aaffccfb3fc5a569f4c5f47d342577efb15739f35f37f3f3f8562b6971db6ad`  
		Last Modified: Thu, 22 Jul 2021 00:47:35 GMT  
		Size: 49.2 MB (49222119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d93e557a67ca58ca2f60eafa96251f128c986a181ba60f421e0bdd209a03beb`  
		Last Modified: Thu, 22 Jul 2021 00:47:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:2e2b742d36fa11427654404cd93a18008abdd5410d507aa2f630dbad83c635f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51206987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c366a11be44194c0f27edb8a9ebbb2eefc76b689bfe400ee3fddba3b10142142`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:00 GMT
ADD file:8e55b0e3d115c6366237668311c2356a0ba2a47cd0d7fb73723647f4087298e5 in / 
# Thu, 22 Jul 2021 00:41:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:41:06 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5383c85c156c662eb185840d8e39387ae2770c823e47ce2f3f5e6a9962980823`  
		Last Modified: Thu, 22 Jul 2021 00:48:34 GMT  
		Size: 51.2 MB (51206762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfb5f46bd54546045a11e1e581c2a069a8e7b004f7daa150c03a4429172e215`  
		Last Modified: Thu, 22 Jul 2021 00:48:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:9e3f792a7a581003b39cea0565aa7374cb960a6862f8c016b624c55eaf31e478
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53167500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8336ba2c2f4b4b1adaa10a0940958a48ee254a322909807e73a92e495da57508`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:14:35 GMT
ADD file:2d7e0632e94c14e727abd071c43f507064f876f70d39ed72cf3a825dd6c33397 in / 
# Tue, 17 Aug 2021 01:14:36 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:14:44 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:31d8f82cc0e98ad1cbee58906296b760fe8981a49c1cbf4427c97b0474d29add`  
		Last Modified: Tue, 17 Aug 2021 01:25:01 GMT  
		Size: 53.2 MB (53167277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028686d946fdb8948161eeb156cfdb0bd415412eca3bbb7355b06aab6e9d2b1b`  
		Last Modified: Tue, 17 Aug 2021 01:25:12 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:100b3e9120d22b878d6d53cbae425876a75d2b086a0ed416bb89fdafc8936e27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54182650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b82e5ec4a201452546151568c75bca681f6ab0d34911ba905e4c6ecbb496d9c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:20:10 GMT
ADD file:a10e852603be4a8537006299bc6490a15181efa7c6bdc8c2278dd664c5b4bf38 in / 
# Thu, 22 Jul 2021 00:20:18 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:20:39 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:faee74d5cbeba300698783b9582af087f649d5b17d4adeafea63f7482a1d2b2b`  
		Last Modified: Thu, 22 Jul 2021 00:29:01 GMT  
		Size: 54.2 MB (54182424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39d82f7fb457f0d1a67dfc1d8353ddf18164f873f5453650221bf15659f8bff`  
		Last Modified: Thu, 22 Jul 2021 00:29:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:3a0d66e9ab7f34385a8fa9d152a70b85c39245616c52d5921c7d0bcb79a55753
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49004003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c96d592d354e1ac45ec24a7e63778ca77ed4936c1d1e20e3d7a37c69ade7e57`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:43:30 GMT
ADD file:14e3a940c66c70d04bce67d35ac71518affc63c067b19c183538f60b13b0241b in / 
# Thu, 22 Jul 2021 00:43:34 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:43:42 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4c4c2e7cab9fd5c5a81bd5f2aec15170c676991a90a7f306054ee7c88891352a`  
		Last Modified: Thu, 22 Jul 2021 00:49:00 GMT  
		Size: 49.0 MB (49003779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0388fcbb49c0b56b9a63b7c68e2c598d4124bad01d68c211cf5140160ca53234`  
		Last Modified: Thu, 22 Jul 2021 00:49:10 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
