## `debian:stable-backports`

```console
$ docker pull debian@sha256:1f96557a315ecf9048e5da3050a6ba121caf2c023a49692927fb5555166742aa
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
$ docker pull debian@sha256:4c44ed4cfcc576ad53b4fe48c02c3edc17be44785cfb8a327dadc0ff466d5bc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49561810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd75205615c761b9acd17e95e98df6378cb672d0d366dd19a883f5d1fbf0df4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:24 GMT
ADD file:974e64d5811025cce8d9e989a8392361edbf995c23a3a768924fe3ddb4e3383c in / 
# Tue, 19 Dec 2023 01:22:25 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:22:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:002532ca787c14148f31b15b032c7c1cab3a5b6097a69a63c8b46324718cf247`  
		Last Modified: Tue, 19 Dec 2023 01:28:26 GMT  
		Size: 49.6 MB (49561587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e977ecd26b07cfcbf8bc4c56cac9e2e218b09c7016c90bc9016671637a9d203`  
		Last Modified: Tue, 19 Dec 2023 01:28:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:ebf4e11a6f637285634fae42ecad185767dad37de8b86e6261cc418c6c1c720f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47319443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f07cfa07b66d353d99c26bcc1add3542bb4409452faeea3843b1b7d7a2748b4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:56:15 GMT
ADD file:c97b8b18bc510a36fc7568227a3dc9feeab9f27529c81042603bf29dc7f868a7 in / 
# Tue, 19 Dec 2023 01:56:15 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:56:18 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:114f046377e0fe6ae226c6bcb57d65fbf59d7ebda9579444167c5b1933e27de6`  
		Last Modified: Tue, 19 Dec 2023 02:00:56 GMT  
		Size: 47.3 MB (47319219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a000a423cb1dbed74096adcc37d7b957d40a99be2dbfecf24f60958f76fb5407`  
		Last Modified: Tue, 19 Dec 2023 02:01:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:e8ae2c15e32327b6d5c9c1d491e328f3746643c7090c12f45afe5dd46853fe43
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45156936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62194265470d73d50e057eb84a1e1e2f73b4fe4804f2a8774becde4ea3d12dba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:09:27 GMT
ADD file:ee4d048c7fe2cd2866185248d209d9143292b1539617f010a0b6fb506fa23c4d in / 
# Tue, 19 Dec 2023 02:09:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:09:31 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cdb5b6e4f71744eacdc3bda9431299b7a114db2ee34ce4785db405db9c500c38`  
		Last Modified: Tue, 19 Dec 2023 02:15:02 GMT  
		Size: 45.2 MB (45156712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87ff3da6545ef5f09b826a9b7d85eaffc255369c4f2aba06ae40f633067b06`  
		Last Modified: Tue, 19 Dec 2023 02:15:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:34229a7108edc5af7cb33b80840a58c0909bce213c7c37ff7e590dfd62dff362
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49592467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b62f8e78edc116660289e28295e373dabbe7ecb9b0c41897eb0eacc8cea203d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:26 GMT
ADD file:006303c48e11ab9bbbac583efcf7f43617bae74e8cb11dc00076189eaabc1a8e in / 
# Tue, 19 Dec 2023 01:42:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:42:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c799c94ce8e4f581440e2e3757ab64202cde97bb7234ecca8eabdf005d89acd3`  
		Last Modified: Tue, 19 Dec 2023 01:47:49 GMT  
		Size: 49.6 MB (49592244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cde444bc543d1f9af711233b73db63fcdf1d33a3228104c39aeee9a98ac31a`  
		Last Modified: Tue, 19 Dec 2023 01:47:58 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:d12342087ad5ff012009c44c754680c16aa6e0bf16c862da94052496c6ef7c0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50582512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313544fd1d06a3e3abef97bbc67e59614bad7dfab935068af860a0a4d058c0f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:06 GMT
ADD file:928dec1dc8385cda860622eab7a5637b4209dc1815bf72efdc9daa42c87ef48b in / 
# Tue, 19 Dec 2023 01:41:07 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:41:10 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:985bd0cb96ff99f303bf1684f14b4755022f384e8342dbf1d60a98c1032f559d`  
		Last Modified: Tue, 19 Dec 2023 01:47:33 GMT  
		Size: 50.6 MB (50582288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74029a567f9ae1e1d4bea72d24a4a13732b660e84fbf9e114b1b1d601e06247a`  
		Last Modified: Tue, 19 Dec 2023 01:47:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:d225659b3bd9fb0ee029ed54621d23dcdc4bff696fa44c488f3446d5d5546ad8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49549059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b147c8e20c2a9a65ebb65e18c0d5dde7f3b28f81a3d4a970ace142627c5fae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:17:46 GMT
ADD file:40cb7dfcb17af001537b29ec525e728c5d7ecefd02aea526ec78353a00ead913 in / 
# Tue, 19 Dec 2023 02:17:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:18:06 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:46b017b6e0d4580709a27c8d843d926d9ab2bfe7c2ca2a4a0899a3e7651a8803`  
		Last Modified: Tue, 19 Dec 2023 02:29:12 GMT  
		Size: 49.5 MB (49548834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a728078a0b9426ddd1c98ad9fd29a2f1ec8562d533124a98b1031fbe859408`  
		Last Modified: Tue, 19 Dec 2023 02:29:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:084ec186ea31cded3e97ee579b9fee2781372ff6f3e4eceb2700484b7103d992
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53557996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718de308fc35a7ed537146576854d528c287c920bbdc0eb4608c87a88347fceb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:23:23 GMT
ADD file:2c624ccc003d0f4104b35cf3bf6cccfb35c9a0b709cab7aabcf1ffb0f719c5cb in / 
# Tue, 19 Dec 2023 01:23:26 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:23:30 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:22d8c758808e8ea3211f06e4878a686b3a00746270bd384d9f1149eafcfcdfae`  
		Last Modified: Tue, 19 Dec 2023 01:28:51 GMT  
		Size: 53.6 MB (53557770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89559c3fceda95cabf3bc28d81e650670c61411008392b2d15c37c2be1fe37e`  
		Last Modified: Tue, 19 Dec 2023 01:29:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:1d0db160cf5b5f49e6210d9c75123cb9ac19a634e2c60e72b5952918a126e67a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47917900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d27d3f0bbdae6844d052a9b8ec40acd809958e875eec7723b69b2c26252825f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:44:24 GMT
ADD file:0c60c17ec958129c457b177efb3a02b9aed5079a6063502e7a569ff0d0e446a4 in / 
# Tue, 19 Dec 2023 01:44:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:44:36 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a009a03321579bfa9e1d2f2e39000c66b62221105b6b0d80f67a5af06b8285a4`  
		Last Modified: Tue, 19 Dec 2023 01:49:05 GMT  
		Size: 47.9 MB (47917675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dfffc600871a62f4c7966ce9f31540f967d210e0870cac450f65e02565a9c1`  
		Last Modified: Tue, 19 Dec 2023 01:49:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
