## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:ff263a29f107c37f995ebf835f0ef462f0553bb271a95dc44bc6b4ef7be5e5f8
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
$ docker pull debian@sha256:ef7812a599a58c346d949028ad5742a121bc4d6316aa745293a3e8d448eb85c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55055528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806d590d2f5b342480c8f6ab41e7cf886ad37bd0fd8cd90e5500cddec69edb1d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:21:25 GMT
ADD file:aa8ed94ddb59e4c0538b39dcaa7040aa0aa62297242af9074715df5e49310d5c in / 
# Tue, 04 Jul 2023 01:21:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:21:29 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:70705a13f194adda8510677de1e9a79a43350123f9bd3d7a7be637b9f7084f32`  
		Last Modified: Tue, 04 Jul 2023 01:27:13 GMT  
		Size: 55.1 MB (55055303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66222735b3343b5b6b4d785e66b8f874dfb990b0f598d08cd3081d54660f5b4`  
		Last Modified: Tue, 04 Jul 2023 01:27:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:a1c142aaf6010ed412209a6930b30a61454d97e222e475d389c7c11cf3339218
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52557004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4231655e7e94dd41818c717cf6ad97fade4aa67795febe1247db0de2e781766a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:55 GMT
ADD file:eedd41901674350e1e1469ed0910b376f827555b17b22e3e10f0110f86d62478 in / 
# Tue, 04 Jul 2023 00:48:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:48:58 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d4e822f3c7ca5566f101f8d90ca82f6f749f73c7518367686a1e48cb3d17f459`  
		Last Modified: Tue, 04 Jul 2023 00:52:58 GMT  
		Size: 52.6 MB (52556780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b7a7789c97a6d50342a32a55eb69b34d57a5a9e65f9dba2787d9b6a7f76d30`  
		Last Modified: Tue, 04 Jul 2023 00:53:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:aef5318ba503c33f45cf7a269cfb2e6f670e8175c9b00b0a8f6e16192b2893f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50218493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155602c72582ddb6094901a521ba97c5577a41c962da17679d86d43c4009170c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:59:22 GMT
ADD file:ea176a714b2523843bef5db3cdb0b649af02c3656e86f8c2c4f18054fae67225 in / 
# Tue, 04 Jul 2023 00:59:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:59:26 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:172a14bdbe7b3b2f83f795e8c55945aea2def70aa907d371cb1f32a71323d65f`  
		Last Modified: Tue, 04 Jul 2023 01:05:08 GMT  
		Size: 50.2 MB (50218268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d7c97b4dfbcb704327b6bfaae85ad8b672d6a7846f992b10fb34ce524a5699`  
		Last Modified: Tue, 04 Jul 2023 01:05:18 GMT  
		Size: 225.0 B  
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
$ docker pull debian@sha256:9ed26dd86c73f492bb27b64317b40d92601467eb7c592295eec86d7fd8ed7415
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53270703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f509d0d0fe4f01b734f2050b452568f8f751d5648994bae95967965f76ef932`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:11:17 GMT
ADD file:01e73873458ff017b9060e02c6c6d6e80dd596c5d69932be1af564907154c729 in / 
# Tue, 04 Jul 2023 01:11:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:11:36 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cad33424acd55ddf10c5c761d89e4e342d970ebf80cbd441dafc9c4afaf0224b`  
		Last Modified: Tue, 04 Jul 2023 01:22:03 GMT  
		Size: 53.3 MB (53270477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ce2a6c04567e0c79f2b48c9c4f3d13c777db985e3eae22f07a9289af88866c`  
		Last Modified: Tue, 04 Jul 2023 01:22:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:6a99017a0a473945817202052d513e7e2dbf48ca1a272e1bffebf7c58e0e9e0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58927961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1046574891621967c2362700f745937d96160d35c2e556689e72c42e0c71bf59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:53 GMT
ADD file:28017068c8ae84b6dadb06a194af584a65f0ea1966327d6ee4c66ff6b29bc8cf in / 
# Tue, 04 Jul 2023 01:18:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:19:01 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4a92e1f73b9a25672e5117ddfc8a47ace827a65a17ac563c3cef3151fe2f94cd`  
		Last Modified: Tue, 04 Jul 2023 01:26:10 GMT  
		Size: 58.9 MB (58927737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0704b61031f4c425841aebeb50cbdc2e0e681d3c24fdf2488782cb58109308`  
		Last Modified: Tue, 04 Jul 2023 01:26:21 GMT  
		Size: 224.0 B  
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
