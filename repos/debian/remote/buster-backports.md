## `debian:buster-backports`

```console
$ docker pull debian@sha256:d5f473fb1e673e2beb713bd711a37be823b02ece667f660cc01c98aed38ecede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:26a606c011d44136a2960d367c232be6227ee6b4a87106d6cac3dc9f559ec395
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50497824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ed18fcd49a5c98840283476d5f7884fc71c257ac00a31d7e19adc29fa3eae53`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:21:28 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035ead669a593978375a90546ea8b82dc83afd38965b870ac9928db9cca0c988`  
		Last Modified: Thu, 07 Sep 2023 00:26:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:e4682b06b2ff256d35903ce7837472d95cdb65bb178d665b26c621817831bbe0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45966342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54382a62fc88e7404098ddca507f8575dc668cf5209368ea4282a1fb6cb612ae`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:19 GMT
ADD file:7ec242a3962c31a67f54c602b7f422709b35916aa381a646dc41202360549761 in / 
# Thu, 07 Sep 2023 00:58:21 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:58:25 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:719d9383401f642312dab568888c86aa5069040b61dbe32fb40d5a7bc5fd5c02`  
		Last Modified: Thu, 07 Sep 2023 01:03:31 GMT  
		Size: 46.0 MB (45966117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57013c317bd62bb2a00a59d49dfcc2f702fb706c668b3298d1c64f70d239c410`  
		Last Modified: Thu, 07 Sep 2023 01:03:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:40564b071a06cf92cfc75676968cccb93712c96637129df5ac69cc72e9801ce2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49291109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea13722262708c2a01ecbb48806d3c93d50475bbadf90ac8d7274bddf92cfb68`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:34 GMT
ADD file:3ec160f0e210563bfac108f23e5034dda5bc7b513b824ee276e4fc6daf80c89e in / 
# Wed, 20 Sep 2023 02:44:35 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:44:38 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:acd8b5ac4bd39653c2ebe6bd243f4ad2ee504ec9f8feeda9ef727446baf30721`  
		Last Modified: Wed, 20 Sep 2023 02:48:30 GMT  
		Size: 49.3 MB (49290887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca7b9c16ebea7f5028919e69d1d425c3882d50736daba1bfc0ae33fca3242d7`  
		Last Modified: Wed, 20 Sep 2023 02:48:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:4da13c493b7a496aff0a087ca00773b400f6612f89f3079995ea39662422ca61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51255637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9fad0b1a8cf28c31d6dfea6195f984851d9e8dce35888473bdae4c0cf1ed02d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:29 GMT
ADD file:6603eb215d695ca693056401592eb42db80ae6d6fcd314b50322ceb7858c1f2c in / 
# Wed, 20 Sep 2023 00:42:30 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:42:33 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6be8533983dbe30a84ca98eed25142115c1c6e36639d1e5086fd77e3332abc10`  
		Last Modified: Wed, 20 Sep 2023 00:47:58 GMT  
		Size: 51.3 MB (51255415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eef73bf40b7aa6cd3e0c9d15e8f94cc4a8c5a1919f426ae164ee9dc891d94b`  
		Last Modified: Wed, 20 Sep 2023 00:48:10 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
