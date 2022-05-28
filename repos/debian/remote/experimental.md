## `debian:experimental`

```console
$ docker pull debian@sha256:801bf04edc5a1e356d42761d828ddf33d7cc6a7c639c1115d1051580ac05ef6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:2095c07731658e625e2d1c5ab9b6d8d20d15765b777235f29bd3ee3df703a478
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53162201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d23b2663661a6a952ae3d09254efee9a17eccee4b7fd70633b99242e865f337`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:22:49 GMT
ADD file:03d36b06287d3c15ecf341e79223be3c2466a06621d871225bf3bc50e4629dd4 in / 
# Sat, 28 May 2022 01:22:50 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:23:00 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f5e1f8c89883083ec55e0fdeb4bf250bfe90a925a5311b14424e6de63fc8625e`  
		Last Modified: Sat, 28 May 2022 01:30:00 GMT  
		Size: 53.2 MB (53161980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724808e91286c41b803afdd235f8da465ea6108236b99d3fee65b159188df447`  
		Last Modified: Sat, 28 May 2022 01:30:23 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:bddb06b0f6965ac4b7ded82ced103322547df94ecde0a7e6eeea612a9ea6d959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50940069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc8b79f0bb68044d2ae1551b33743f9e106125cbeb6804cfaabb3a67ea6b8d53`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:57:31 GMT
ADD file:3b98d75470b5342f06179d466794e6a231be41b0a3d3c94b6ae0efbdcbb9a74c in / 
# Wed, 11 May 2022 00:57:32 GMT
CMD ["bash"]
# Wed, 11 May 2022 00:58:04 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:be71d4ded79eb5a181be2fe43c5f3f8e0e79c48fcef2a4b538396eb809b84547`  
		Last Modified: Wed, 11 May 2022 01:15:47 GMT  
		Size: 50.9 MB (50939848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5c84c2be9c8faed852a449321696e10b06f0cb595e2ab1c0048bdfba46abb2`  
		Last Modified: Wed, 11 May 2022 01:16:27 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:7062a80b975a4d2557e0aa06a9ff545c5df77de4ba31abe452bfa706a4b9fa3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48693712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5cc1531b4c25438adaadb0c2ddf73ca402c881e5533c26385b66ad5b4ade4f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:07:25 GMT
ADD file:98c2a5cb7c628a857e47ad8ddf413371c4bf785f13bd9113334981f92eb59708 in / 
# Sat, 28 May 2022 01:07:26 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:08:01 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b3183b7b01b9f303f838e63108cd9626ee2f8418467acffbb847bf8a81127905`  
		Last Modified: Sat, 28 May 2022 01:24:10 GMT  
		Size: 48.7 MB (48693489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8d0179b04113cc9d2c23e29198f6479ad5e78fe3d3d3701bcb018a912525d1`  
		Last Modified: Sat, 28 May 2022 01:24:44 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6a80a32d1b374717811012a410dfc52e619238796c8eed8116f33258e7c1942d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52261470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db6de65e52754902f3581327bd312a08b529c22b64919cee988055cdb4a17a88`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:43:35 GMT
ADD file:2872959d1380a162e11a052911482db0c296636653647605fb8b01d15b6b84c4 in / 
# Sat, 28 May 2022 00:43:36 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:43:51 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:586b8a60c851194f5e17a9f5238244c2c05921eba7aa586e6c5c0751b9eb1313`  
		Last Modified: Sat, 28 May 2022 00:52:52 GMT  
		Size: 52.3 MB (52261249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ad4e25696e72a1d8837a91dbffa0c00af68f2b910b61506a6a361dd85b28f0`  
		Last Modified: Sat, 28 May 2022 00:53:17 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:d857809421963c75bac0df791a24fc502a9aca4db33b6fc2f50d8e05c532b0e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54158934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83e5df1e94de4d15d6c0348d65f723a7987fe3b10b9ea2a07167642bf5a42b8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:42:43 GMT
ADD file:ddbbafd9c13cb3214a5f4ac7696a1e2849d91ecdb8c1b7c67e6adf47f5b19dcf in / 
# Sat, 28 May 2022 00:42:44 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:42:59 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:45eb7531e9b10f431a1c01cc0540d78d698cf327a45b3c871e3d2cfda8cf77d8`  
		Last Modified: Sat, 28 May 2022 00:52:08 GMT  
		Size: 54.2 MB (54158713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d2389f7326fa2ce9a33fbb150ee45d7cfcb4e82c07b7d8e164ea9715bf9158`  
		Last Modified: Sat, 28 May 2022 00:52:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:3bf613226a7904f38f2828063f0e406e4cf0ed9554b912cd83e4b835c5c31013
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52283238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a365d68d868eeaf7910a3715bb4cbc948858b2a643cdca5f17c29020c9f3887`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:17:29 GMT
ADD file:dbba26506e42130aa791d13fd85536c141576485ef78ee734dfd43d3dfe40e8e in / 
# Sat, 28 May 2022 01:17:35 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:18:09 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:742852dbe147dbbfd586055269c9e61c0207bf33b0d09f6551023f6aaf1f29e1`  
		Last Modified: Sat, 28 May 2022 01:28:34 GMT  
		Size: 52.3 MB (52283014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d74156248ff5b9f4614b556a3ef9d68e65dade56ac1059d154c00512bf4435`  
		Last Modified: Sat, 28 May 2022 01:29:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:5ffc0a23608eae07176b417afde972f7fbbf541d179ec91da33028b8ae9c106a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57378677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d928a639d5800c5056844dc46c69174b1222752bfa0e1813489e1b802f358cd2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:27:27 GMT
ADD file:c6b19654a4be927699ec0d0a3e18426bee6def1337e956f4bd3c7ecea57b9cf8 in / 
# Sat, 28 May 2022 01:27:31 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:28:04 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1aee6e348acca1ed1f3a538014e26ae7c214d2252b70569c32d605a8168b70fe`  
		Last Modified: Sat, 28 May 2022 01:37:12 GMT  
		Size: 57.4 MB (57378453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7aca69d11709b1d5dfc0fa65de74485d4c2803ffbccdecff92a0024b5af64d`  
		Last Modified: Sat, 28 May 2022 01:37:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:290f4b3e44e5c54e77ba2094ca54bcfcc2fbfda492905588f244218d9eebfe27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49399169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98b6645cc1ee25eaee76dfe92f5eb930862067c856b740610cd95838ae2b23a1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:18:55 GMT
ADD file:8c89b85e7d84efeb2327f7e697d1dba388b7df92b95b8eecfd98215d54600e32 in / 
# Sat, 28 May 2022 01:18:58 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:22:38 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:260805c7f1441e2f6380a7e8641588a06baaca764508ad0ab2932a1328fc25d6`  
		Last Modified: Sat, 28 May 2022 01:37:23 GMT  
		Size: 49.4 MB (49398941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c37b5ac8d2e8a83c1e72848c1c2ca5eacc64357dd7b56efc8901f19b020608`  
		Last Modified: Sat, 28 May 2022 01:40:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:90add0686b81682f4afa2adad119afbeaea8dee4f6f73ef6c6d44091264a430d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51703461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eacac0f07bd4e56d2687ca7ceedd966f6d54cad580588b1c1fb018fbec07d532`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:46:25 GMT
ADD file:ca2f9e70e62257fbacb0eb455cee1752c9404754ca7f5149c70058259220b8fd in / 
# Sat, 28 May 2022 00:46:28 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:46:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9fb199d2a2726467db59cf4e8de4009b204a5bc0adf9d148f49c09fd9a992e28`  
		Last Modified: Sat, 28 May 2022 00:52:19 GMT  
		Size: 51.7 MB (51703240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8e8f2b28b94c6e77dd3c005049957ac0cb79b7127f87f3fceea85f39a22ddf`  
		Last Modified: Sat, 28 May 2022 00:52:37 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
