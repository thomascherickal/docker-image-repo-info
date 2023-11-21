## `debian:trixie-backports`

```console
$ docker pull debian@sha256:1599faa222abe589d8acdc0370a9e709a51bd33d2aca6ffa4f410fedada83e00
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

### `debian:trixie-backports` - linux; amd64

```console
$ docker pull debian@sha256:bdc804b709f9f08d29f5714c321007d3c7d73a4457818153ab6d197a49471281
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49487111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cc365e6d64f1fa99f644a3d349d49b2e0253b34a2ed505fa8ec0d47e4d579d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:23:36 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0cec7452f61de8db69b39ff009d17ba7e574e5f249fab5834ce1264cac1b59`  
		Last Modified: Wed, 01 Nov 2023 00:30:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:eec44d10ad7289adbc1d8144425243baf2396c837df73d7e26df6686099d3389
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47222495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18ee6eac93eaba22418a58c1809d9333a9433215f3375f0a9d0d49a60cfe21e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:24 GMT
ADD file:b3c8930f9373d4b494084a470670d4cc731173a6b8f430173b03a3352a74180b in / 
# Tue, 21 Nov 2023 05:02:24 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:02:26 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0e9f882881657ea279897d7d6f0016a79c0e107f1eb6d1fbcfeb6c31891d0af0`  
		Last Modified: Tue, 21 Nov 2023 05:07:16 GMT  
		Size: 47.2 MB (47222272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a4053bdef906def8bfadf7ca6111422289c8a153b20414788e9229c8d140a9`  
		Last Modified: Tue, 21 Nov 2023 05:07:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:a5bfadd62fedf5b277b58d84aaf66e222c74c4a6bcc147ce0a425b62836face8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45026003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c337f7d73e151dc97bb324b7df2a59493aea114abda44384c0511aa6588aed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:59:58 GMT
ADD file:59809e0abebdd1dc9132ad810fe8f3f2944fb2b6fa8df3e129a60d19cf0a0235 in / 
# Tue, 21 Nov 2023 03:59:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:00:00 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a13157ca2b3325f6cfce85c5d417fa81a8cf7c5536e5efd4164b11bece6ea33f`  
		Last Modified: Tue, 21 Nov 2023 04:06:34 GMT  
		Size: 45.0 MB (45025780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23497fd1d71fa03463053d8d11d92c5843ec558081c7625a6ca685950b3beefb`  
		Last Modified: Tue, 21 Nov 2023 04:06:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:4a93adbb154f1fad647745da547c4ff41af2d385204e6500415c5bd9c9418f7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49495451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d12d053b207ab6585fdfb5efd1d250f1a4cae53dcfb2429e466c0b0091b10e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:41:30 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4e8ed1638a7121f3e41c0aa7ae4707ed08f4e2eac9ba94a29c394ee1650c59`  
		Last Modified: Wed, 01 Nov 2023 00:47:24 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; 386

```console
$ docker pull debian@sha256:1332b8e8da61717031868b758122771d9216a72a7642e1afd6f842525203a057
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50516297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:200f6c93b98f5a011300ce0df8a34e823319e79b2dc66df112754a41c1f0aaaf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:42:33 GMT
ADD file:cd5c641cdd0f01b902e53dc6e8c380bde0d4e118a475c7cbd2cc8ea880bc0e3c in / 
# Tue, 21 Nov 2023 04:42:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:42:36 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c29bb061afedb9f8c32cdd52831b3e91bd7d756b7c2ec0d75c654790f577459b`  
		Last Modified: Tue, 21 Nov 2023 04:49:48 GMT  
		Size: 50.5 MB (50516074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec56883ee6e800496ddd72fda87c7df466ba7600b1d78b97d32eb8c91742a492`  
		Last Modified: Tue, 21 Nov 2023 04:49:56 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; mips64le

```console
$ docker pull debian@sha256:152c4da86da80278dc126099ad91c537a08847aa330b3d25631a8faa05377a9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49327743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed931655b248673a1837ac92e5054d33c1b64d63e996b73b45331b7bfa86f7a4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:16:18 GMT
ADD file:5a5a104714237ebb36fb780708ec93fc6f37e226c70a6cb07acb454559074354 in / 
# Tue, 21 Nov 2023 04:16:23 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:16:33 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d49b5078b4e69925915d9f9be6cb94f93e60122ef1d800b354bcd8216ec830be`  
		Last Modified: Tue, 21 Nov 2023 04:27:30 GMT  
		Size: 49.3 MB (49327517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7563a746deb7a45411ea950de0bc22fc344bd34fb9a9e5b1efc4ac318db0b4`  
		Last Modified: Tue, 21 Nov 2023 04:27:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:189a35bfc940f9e48f2e1b32984097d90a68a9329e497715a21ecfebf0d1b0c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53438105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e5167401a760c3b7989ada565072179103bf140a4a6cf899990f56bf1aacf4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:26:49 GMT
ADD file:dc6f1d4d555ba3f35237b7e67b320c18ac6e1c8d12a95eedb8a5230f42402844 in / 
# Tue, 21 Nov 2023 04:26:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:26:56 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2c7e2ccd81c8e1fab8cf4a7e3dcfcc9c9057946f10830bacc66f9e35e00b25e3`  
		Last Modified: Tue, 21 Nov 2023 04:32:41 GMT  
		Size: 53.4 MB (53437879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41977c95fdc4e070972cb47e0001d5b2d851d918504762f85aa41479d4242d02`  
		Last Modified: Tue, 21 Nov 2023 04:32:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; s390x

```console
$ docker pull debian@sha256:7bb65e44ecb2bd0e629cd6f012ec56653d44deac08cafb0b43bd643338884a15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48970458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254ceb715f4e16688111cc71345cc0b549b867e967f916b3f1605d9b5a4294a8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:07:59 GMT
ADD file:d0b90d4f8aa4259bbd6e1887bf2da65394e444995622363495d2e13ad00154bf in / 
# Tue, 21 Nov 2023 05:08:07 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:08:14 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0b094bae18b4460a8208634d7220fba165e3979b123ddcbdd060fb9c73c37f2b`  
		Last Modified: Tue, 21 Nov 2023 05:12:26 GMT  
		Size: 49.0 MB (48970235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a42c652d341e88cf72b8066531e4cd9ffb6e544874ce65c1e9946902aed216`  
		Last Modified: Tue, 21 Nov 2023 05:12:31 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
