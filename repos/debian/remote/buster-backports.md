## `debian:buster-backports`

```console
$ docker pull debian@sha256:43b6f76030ca501a0894fca46d4db030afa8da4da2955a762eef09e43927c558
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
$ docker pull debian@sha256:6e5795313a16bf948fcf0b460755308b38a49e315c0982bd36ed4c3e7ec52e87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49290830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6911fc14dadaabeef566d157e7060d25d706dd4baa0c77aee29d344dd3322d2e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:00 GMT
ADD file:d9e56538de5f967fc9a8327ecb4e67562f6f95e56b455b9494e35d3b57c89332 in / 
# Thu, 07 Sep 2023 00:40:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:40:03 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:26ee4ff96582b6c5e191414a6b74b283e3039e003d1b6f546cc00d6b14ff8abb`  
		Last Modified: Thu, 07 Sep 2023 00:43:57 GMT  
		Size: 49.3 MB (49290609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16cd8bf5ec63039b618d06f1b67ec41dd2d473d4ef371376332c4aa8c5770d0`  
		Last Modified: Thu, 07 Sep 2023 00:44:10 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:5fdf787974b17215b91fd0ee82943c2099b78ed91c5727c42250d1622b206d1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51255345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c819075ad42fefc3469cc0b9421f7a958407ffc784660c9d132163b0321808b0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:35 GMT
ADD file:e361f508945f7d4a295d9dd30a26c2eec74e47dd5a1b49328c7a6a7ed2d94d63 in / 
# Thu, 07 Sep 2023 00:39:36 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:39:39 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fa64faf93a921e8d6df313df0ab0ce8255885730dc1fc137cb62b66633477d02`  
		Last Modified: Thu, 07 Sep 2023 00:45:01 GMT  
		Size: 51.3 MB (51255123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59486d085d53ec51ad63d7e8c4aa061f1f7fd365a67b8c23b358aaaf314925fa`  
		Last Modified: Thu, 07 Sep 2023 00:45:14 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
