## `debian:rc-buggy`

```console
$ docker pull debian@sha256:ab069a0fa233adc07ecff5c3b448a7a2458092855cd67d8bfdbc8138f591e550
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:9d66ba41dfc994c5fc9422d7725de40f01c3c2ea4053e84ddb0e3014398d2c8e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51391215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:807e7e919e46442b54b4c280a6cb0e5ec468babac45e3dacdc0785e2080a3f31`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:22:30 GMT
ADD file:1b99a100214a4a86a413bf6a826c70d07fee06a8c4e6d1f3ed1550fb08f9818e in / 
# Wed, 13 May 2020 21:22:30 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:25:09 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:268c82fb25093fc20c25872a9f96ca2bef121a19a81a91079b62afb96b725135`  
		Last Modified: Wed, 13 May 2020 21:28:35 GMT  
		Size: 51.4 MB (51390987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9654326c409372b98f92f8ff1497c187e6e86558120867946596e22b3b73ef4d`  
		Last Modified: Wed, 13 May 2020 21:31:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:e5f87c78961828be7ee21000c81c1208f8f5ac99157bbdbfa4bb0a692e5e5dcd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49373176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3c79b56f06094e50ebe7519a9ed474707d6d509f6b677acb0faa671fb6eb02d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:40:47 GMT
ADD file:c2ef493946404baae91412a79e2336f831835f471608b615f053cc8cc1c1cb62 in / 
# Thu, 14 May 2020 22:40:49 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:44:49 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2d6200ebef6b4ed212e54012a0718d6122f96033e0dbe7fd95e64d7739c61b3f`  
		Last Modified: Thu, 14 May 2020 22:49:25 GMT  
		Size: 49.4 MB (49372948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd75f2fa7532286f58be886fc9b160a74af453aacabe35fe64bd380ff279149`  
		Last Modified: Thu, 14 May 2020 22:52:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:d218464dd93befb8e38ea902161a311d8d77a5b93f4951ffd08392f27575237c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47179404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45d79b5a74c75ac1d1a65f74c54b89e36c31f9b11d931c3647eefd4dc803aa85`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:04:08 GMT
ADD file:7bc7b5e94debaef8aabee3128de6e535c9867794ed42649aadb9ba63a66a547b in / 
# Fri, 15 May 2020 01:04:11 GMT
CMD ["bash"]
# Fri, 15 May 2020 01:09:29 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:921baaddbf45818850d057b247e93c5fa875838ac2dbf11e2913f526f5ac4d94`  
		Last Modified: Fri, 15 May 2020 01:13:34 GMT  
		Size: 47.2 MB (47179178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24f3b5ecb2215070a56dbea6fd88da36cd8dffc740c0871a2225ce9ddb02659`  
		Last Modified: Fri, 15 May 2020 01:16:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:467cede327a4fc696db16d293af97fe0a33a216648a1bb8873d97501951bff17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50328893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d5d332f6859b59f37365e60480e3eda0d2d299136af9c4c26f8badbc803280`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:45:26 GMT
ADD file:22517e10f0b5d2760fafa2367b5a187d7ecef96291f15a746c24bfa50f756219 in / 
# Wed, 13 May 2020 21:45:29 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:51:18 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ad0025dc69d6f0241b2f5b614e96cef6e1fd54c9ef07b726338235b4766714ea`  
		Last Modified: Wed, 13 May 2020 21:54:40 GMT  
		Size: 50.3 MB (50328664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf9e39147b9f9945af18a8bd0a5912c6850ccb4df60b4ce5aca105f64b125b6`  
		Last Modified: Wed, 13 May 2020 21:57:50 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:03bd9a88ba599d38f0c4b27581b08aae3895722367a361fa12615fffeb6014bb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52481796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:594c6a5318292642575156ceec23fc9eed88c7b8bca75a59d97bb9657d5ec765`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:18 GMT
ADD file:bbf57f6406dcdfbee8d207ada2ed9150a3e775fa2cb6e0784c3e35e1c3216d25 in / 
# Wed, 13 May 2020 21:41:18 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:44:01 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:430f489239f0254d72f3974fb8f614ac80ef76f642ab0bddcc4f20a8d4a3c68e`  
		Last Modified: Wed, 13 May 2020 21:48:41 GMT  
		Size: 52.5 MB (52481574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202da6ad79c19bb41cd09dad05760dcbbba97bdc75998a55a5d1733128b37e8f`  
		Last Modified: Wed, 13 May 2020 21:51:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:1be86168085ec12d7511f01744808935996a6754914562f7c39725452820184d
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50149231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7602825d9bd50128c75981669cad0c5d470b9ddd192bd5b9a93bd967cffb84`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:49:44 GMT
ADD file:2c7c92015da849bc75eb25960609c90178c9ac455dab05aa4ef031806d26ad64 in / 
# Fri, 15 May 2020 04:49:45 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:53:57 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:567e61b8ab78e586542d5b9fab62c3880de99927de482a73e9e8b5b304f5284c`  
		Last Modified: Fri, 15 May 2020 04:59:15 GMT  
		Size: 50.1 MB (50149003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599418705e47c0ac842aca6bfb5679c7c307ae0f7ae35b4ad0c79f8b75a76c4d`  
		Last Modified: Fri, 15 May 2020 05:05:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:c1bb0dc6b142e939faf12750f39463ccfda7c89c34fe01ebbf8596f2cca9549e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55112057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc2c7970746be77bb19c67edba8b06942b942aad25eb5511c9dd3f507d373be2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:28:26 GMT
ADD file:7e16c349b13e97e4784ee396bb36ab2d3a069714388b0803f18ceb8d526be36a in / 
# Wed, 13 May 2020 22:28:35 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:54:54 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b2aad5ee0ac7c9bdb0530f0a2f94bcadce58437453bcbdc7a2f20b5366c22799`  
		Last Modified: Wed, 13 May 2020 22:59:47 GMT  
		Size: 55.1 MB (55111830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d459bf1ca5ef920a92946f24ce94c83b13e5fcf17807c2e4a988652899071256`  
		Last Modified: Wed, 13 May 2020 23:05:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:13560af0416a147c50f6fdf40945b73113d797a49c365a63f4062d27fb1f3976
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50009165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53ed3ab33fa2330635187da77f6df9c4be2c28d3a311d3cd49a3f805654d7d08`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:07:25 GMT
ADD file:e200f47e248587a66670fcf47316228d04373cff77498412eb3cc5d6a1ec50a5 in / 
# Thu, 14 May 2020 23:07:27 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:09:56 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:11b5223327afa0d65cbb885c5383c894bdfd11269c346392cfb8a39f81aabaeb`  
		Last Modified: Thu, 14 May 2020 23:12:06 GMT  
		Size: 50.0 MB (50008939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04984612b682e9f7f62aa02d51bae48134c72d5c2e8bc88cfeb65df400b1c997`  
		Last Modified: Thu, 14 May 2020 23:13:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
