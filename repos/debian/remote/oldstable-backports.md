## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:390f793323c941b86ce8c69a1cd6cc8f698af5158cf77e9f17af3eebea63171f
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
$ docker pull debian@sha256:7ddb3af78391c17600c96efd07940ff65694a350e03183c9fc394268d0fe88b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50436477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8547007c1afefa659b51c5f7837220d252e27d6ad35adaf9435269154ee4ced`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:50 GMT
ADD file:2e534cb29f7663d54796547961291dc2ed68f76acfea9b1230e9e8435756292d in / 
# Tue, 28 Sep 2021 01:23:51 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:23:54 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:76faeef923bde74843eb96e7128eeef07c2b3e730a26cd6e30279560f8fc29ee`  
		Last Modified: Tue, 28 Sep 2021 01:30:41 GMT  
		Size: 50.4 MB (50436254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042c161e99ca7f57b845de0fbf43c1faeb378b6ba0e1476b886d922cfca1e3e`  
		Last Modified: Tue, 28 Sep 2021 01:30:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:11c3fda81bd459a94fb9a7a04bfebe6ad268538e4c8c428110818d3164909212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48153975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5492d44a679b2f402b227f113750d1086d6e6455b3f7d1f8750882a7e757395e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:53:13 GMT
ADD file:74438a9206fc0547d98056e300568c95fefdebb549ab0e1511ac530413e3c785 in / 
# Tue, 28 Sep 2021 01:53:14 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:53:27 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4fbdce7b75f5a51e079e0306750abf59caa73269c6e1a08c4169a11203d26634`  
		Last Modified: Tue, 28 Sep 2021 02:10:04 GMT  
		Size: 48.2 MB (48153749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2b438fb0de66eba70315e14331e7da4873edd6568d4f87c1fc62b8e45e7b38`  
		Last Modified: Tue, 28 Sep 2021 02:10:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:89ab43965e778fffb0f63f7d5cdd0794d92c9187cd0f677745abac94a1e0f2d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45918086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e04f51206503a5a274ed328398b694f3ed2c94dc1158e6e49a725651bbdaa7f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:05:48 GMT
ADD file:02cd46aedad203df6594749ccd43f07173d22b9a1cf040562edac044c37ccdb8 in / 
# Thu, 30 Sep 2021 18:05:49 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 18:06:00 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:033144e7430bcc10f3ee814e3b3c2e90e9acc37ce0ac7354b8a2c8b68d64c61a`  
		Last Modified: Thu, 30 Sep 2021 18:22:45 GMT  
		Size: 45.9 MB (45917861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb4ce538a57115bca164c2817597178d7eaf1c4bc49bf7ad803aa60f9b3f030`  
		Last Modified: Thu, 30 Sep 2021 18:22:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:df0557f2a8580f2319383d445a9ef6bc343a3c6e3daa1ce4d09142b18707e606
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49222574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fbe2ae784359bbf65a0ce4436452aefd7c4b30f391a6a86222c547b220f22f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:52 GMT
ADD file:1e53836266c94bb5380ad8ddd081de2f0edba1c25bb2cf0c923ab2664ecbbf9f in / 
# Tue, 28 Sep 2021 01:41:53 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:41:59 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5c94be4fbb653265cbca3b3228fb23214358d4bcc2772cfad97594b9c0a92169`  
		Last Modified: Tue, 28 Sep 2021 01:50:24 GMT  
		Size: 49.2 MB (49222351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2830fd0260a2dc443d2ffd88efb9da6cbe1402d1b1c088128cb25ed0ffafc26c`  
		Last Modified: Tue, 28 Sep 2021 01:50:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:7a7f91ca80dcb00e48c7f28eff785601d776c2ed1c69def15b600dfa69c66a4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a685397227450ec33cfb4bcfaa5ae6b1298b313cbcb96a91aa000ff6a672caaf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:42 GMT
ADD file:9a052d104d56e0b9d847870a89ca0dbf3ea5d5c9cef3be65b5299ced7cbfe137 in / 
# Tue, 28 Sep 2021 01:41:43 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:41:49 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5d52f24f8631fecfa6ece230564add5d46cf4edc834f3fdf1a8891f57fd71d50`  
		Last Modified: Tue, 28 Sep 2021 01:51:18 GMT  
		Size: 51.2 MB (51207413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8a803a1b9002e46f41d2f10a4e64c19c8e03fe0099a88921b917234330506`  
		Last Modified: Tue, 28 Sep 2021 01:51:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:74ea4ecb8bcc0ce5eea72f05803d77d40c5ad5a8c81a74698ddb153f50c3d3bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49079890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f249fe00a44871eddd22efede0122b4b111d9ad6bbd93e26ddf014330ec40e9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:12:13 GMT
ADD file:10e4c23879818c55fb94597d1ed9cc6f3667f240496c28b8261abbc6379efcc2 in / 
# Tue, 28 Sep 2021 02:12:14 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:12:19 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:291c2b51f95ae3a3e45273bce7dc2a5b8404fe3fe31810dda556b8ded5b50713`  
		Last Modified: Tue, 28 Sep 2021 02:22:51 GMT  
		Size: 49.1 MB (49079665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6cc627195adaa26665903f38f751d3e3c153f801f30872104e614db0d5402c`  
		Last Modified: Tue, 28 Sep 2021 02:23:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:44b40ab18a1b025c71b6b25c8daeba2a7ed29edce0657d436b1c6377ed754c94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54182888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c694c2b9723790899a70fb6d7866e97109b7a9393dd14f0267abdf2b94d62fc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:25:01 GMT
ADD file:0de8dbd369ea8a734934d859b2127ac2d170c7c67ed97b1969a240f3a20f0806 in / 
# Fri, 03 Sep 2021 01:25:14 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:25:35 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ec7b038dfffa75a312736217d90bbf467ce4af7129e08320361872aa43b27d4`  
		Last Modified: Fri, 03 Sep 2021 01:40:50 GMT  
		Size: 54.2 MB (54182660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d84750a2ec9d770a90f06a4971a6c6d26e845860843dad9ca2f724556fc877`  
		Last Modified: Fri, 03 Sep 2021 01:41:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:685f06c5b541c1c506804fdb237c7f8e272f28eac267bb6d4cfb5b33ddb57aa0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49004533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d113dd593f13b947bdd4495621dbaaf1311600d7c82552af932ee7e3a4a3995`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:42 GMT
ADD file:0d48c6cfa43326752a72a81e480683e805db4db24c44de2528d026c30fae4662 in / 
# Tue, 28 Sep 2021 01:43:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:43:51 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c774ab9b5b870bdae66a7cb4897b04a09bc8a32b6b1b48b388d308fd37c9bcce`  
		Last Modified: Tue, 28 Sep 2021 01:49:52 GMT  
		Size: 49.0 MB (49004310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd3fdeaf46f1dea9263881541454bd94af8d0440038982aed0e06c4b5ef0fc2`  
		Last Modified: Tue, 28 Sep 2021 01:49:59 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
