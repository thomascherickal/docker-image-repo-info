## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:29f0141efa692175c841dfe70006d839933c5a58a9841fc62d14daaf3467814d
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

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:7488722a560ea073acee8d3c7f4c4c8712a1d2345aadef81ca0b857c125cfa8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55055387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47255619a4bf3dab7a21ba6e80f2de09b0fd314de51977253c81fed949ff1312`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:22:09 GMT
ADD file:8f63148e2901c6b81288ae717107de2cc4b9542d50152ca1adbd36766ecafa87 in / 
# Mon, 12 Jun 2023 23:22:10 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:22:14 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:02587a5560601dc972094a14e0b4566e94f3dd6c8eb01b891b7d128f6d6893f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:58 GMT  
		Size: 55.1 MB (55055164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffd6d92c0462be4920a871ab3d09721604ab5120711927960fdc87d3aec63ec`  
		Last Modified: Mon, 12 Jun 2023 23:28:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:9fc14b91ccddd883325e0eea1b20691258a05a7abe3a3b35e526684c004eca64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52556949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73b61193b33ab8aa03ce5ceeef0f73e70f1f8fc732f1223f0f1c8f64f4af21cf`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:55 GMT
ADD file:6088a46bd83715e439ff103baa166c90b4291d6a6d801b8782b04b6ef59633af in / 
# Mon, 12 Jun 2023 23:48:55 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:48:58 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c9247b4a050b6ccc6580ec2d5a190d22c18c733985e0261c35df59cd486b932d`  
		Last Modified: Mon, 12 Jun 2023 23:52:24 GMT  
		Size: 52.6 MB (52556726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490aefb38563cf752e96e43d5fd2a5d4429f952a714e8bbc7bf5e070d3a519e2`  
		Last Modified: Mon, 12 Jun 2023 23:52:32 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:25fa8e50b910935cdac7e71c06660a092afaaa709d8791936a5d8d68c158207c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50218368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7064e2bf242bf2ac33c83b3b7caf3b8f0b5ff8ee05011dfa4f30975dd8da9b18`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:00:05 GMT
ADD file:ed6082afb7e79f937519be1b64a89ba1545434ec4eb53be3d61ede8227dc29aa in / 
# Tue, 13 Jun 2023 00:00:07 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:00:11 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:170929abcc5469d9a04004189f2b69f8391f01b25107555ab03204276163fa63`  
		Last Modified: Tue, 13 Jun 2023 00:05:57 GMT  
		Size: 50.2 MB (50218142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ebe4ef32332a475e1310d1880f6e6ae51f5cf18243ec81e4121e539f400c87`  
		Last Modified: Tue, 13 Jun 2023 00:06:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:2a72082730db0cb71915af570c26dbc5985f629d887804a50fb9f229a83a7fac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53704360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b87f9764fbaee205aeadca4d957466acfae235f3a19b96facbd003095dd12be`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:41:19 GMT
ADD file:525d4a723059e94c54fa517ad8d380e5b646b152543b2e6d64a5c9bd8c9383ed in / 
# Mon, 12 Jun 2023 23:41:19 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:41:23 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:63e136dc7035327be8e0a84a6d2cc6de70453480cb4e3fc92f3820b48012a73d`  
		Last Modified: Mon, 12 Jun 2023 23:46:07 GMT  
		Size: 53.7 MB (53704137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e266e0f7b4db7968ff3bd34c6bfce9654fb32186507ef0db5b433fb21ee84b12`  
		Last Modified: Mon, 12 Jun 2023 23:46:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:cde041831350ecebe0ed1877ff4f03c6bdbce86303a58e8797ac3a1b4aac4c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56040890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3121db0ce46d95da25f97572a98c9c6cdddc38a2e99752bcc4de6654d7061510`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:41:32 GMT
ADD file:0cc200a7a7d7c92d2f4bc7b19958f411d1f57073d05930595ba7115772384284 in / 
# Mon, 12 Jun 2023 23:41:33 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:41:38 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c44e5869f061db310ba199f938096237aa712002788f1485df41fa9d2c8835a7`  
		Last Modified: Mon, 12 Jun 2023 23:48:48 GMT  
		Size: 56.0 MB (56040668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff0fac8bafe71f37ecae4caf4deb8a1a65e0cb29df2602082b6f5c2c35aa720`  
		Last Modified: Mon, 12 Jun 2023 23:48:57 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:356a743fffcf78bd73bcdf6e40533ee4e7a63722967d76e56faef2f34f7fa4b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53270638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6f68ceafe52b5781927634480d337aadc2c9cad6f0eca3da41b231b12302d48`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:11:19 GMT
ADD file:f94f0c896013de48a551579399fafc56829030f755b7dcd1c972b4f20170d964 in / 
# Tue, 13 Jun 2023 00:11:24 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:11:33 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4d3da61497adc99aba771598820049549f0c4424f03eb55ef5395b0fd1966635`  
		Last Modified: Tue, 13 Jun 2023 00:24:37 GMT  
		Size: 53.3 MB (53270412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3bbb8d40881dd54820cd11825afc284dacae84fb64b9e7fcd4840475c7e4ff`  
		Last Modified: Tue, 13 Jun 2023 00:24:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:7d860c33b78bfab246a21a46c71296a63a4c635f0d69bd218b38fe8211884e7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58927660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c79713a94f4e142ca8fbc91ba85fc757f238e25836d90a3a1eca05d1d3b0ee`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:43 GMT
ADD file:457c2a23dc40f3a46af1f133e979b03194b3a56c2ab82e6af814a6f0827b8ea2 in / 
# Mon, 12 Jun 2023 23:18:46 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:18:53 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cb457401614ccdbf757d37cf2caaf438b3e165987c9bc29ddd7854f791f4572a`  
		Last Modified: Mon, 12 Jun 2023 23:25:29 GMT  
		Size: 58.9 MB (58927438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec21e3597893f56240d4db7249a2f13139276e0bf90bdcb50a97afcd55b4ab3`  
		Last Modified: Mon, 12 Jun 2023 23:25:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:57429b419587fb224d09ee540df09dc86742450adb00ab222f8e355f5d6a83a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53288263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a8b4b038f8b9ac5f887f12b0db3728ee7d4a3734fba3141f0d70e8ac41b690`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:24 GMT
ADD file:dbd155532e76eaf9a1a1d0264e9b100a173a947f266e18de89072fb812b4adfa in / 
# Tue, 13 Jun 2023 04:30:27 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:30:33 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b65851d7a61a8e4602882ddf076cc95a597019b416e23170f30d27d780731b8a`  
		Last Modified: Tue, 13 Jun 2023 04:35:03 GMT  
		Size: 53.3 MB (53288042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36506b0b5bba5138668e591f5a81a2f94a354983ffb6c11d2396091651f7fd7`  
		Last Modified: Tue, 13 Jun 2023 04:35:09 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
