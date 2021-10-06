## `alt:sisyphus`

```console
$ docker pull alt@sha256:4a6a1cb89556f2c9f67d1cfb78ced1d9a937d2945ffeb5b43f544b4ac18e50da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `alt:sisyphus` - linux; amd64

```console
$ docker pull alt@sha256:23d121ff1f0b4899779c115ed13a56d0f544574980126876caecf345f2b27f19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41968262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bd6443c924637e2d4eb570114dd8bb8f4037a03eb6bfcbe238f63431dd78058`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:20:08 GMT
ADD file:23a11d42a1efc414b56e2d0a970b9da6fe85f102f3c2ee6b9ea3842b5151005a in / 
# Tue, 05 Oct 2021 22:20:09 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:20:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2de1ef13e503da8b2ce4b9e2a12d52f082c57f13e729689bec0b3c4604dcf8d9`  
		Last Modified: Tue, 05 Oct 2021 22:20:57 GMT  
		Size: 42.0 MB (41968071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecde41fa05fcbc2bc7461093004f57f8fd6e30bc7ef43b20963399360463d2bd`  
		Last Modified: Tue, 05 Oct 2021 22:20:51 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm variant v7

```console
$ docker pull alt@sha256:ac254326f3164ad22fe7316467216248f7d0f16db2627007d6f3927814d22b38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38612193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bedbdc06e247944b408566081f1690e8d2c238088e81090cac6ddec54aaebd19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Aug 2021 01:09:27 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 23:34:14 GMT
ADD file:ee81978960b88085534d7c9ab24b43471bdb4660457e01483c19cbb904785b68 in / 
# Tue, 05 Oct 2021 23:34:16 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 23:34:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9eedb6a57e4fcd96fe2b31e3babcd6646646ac83cf8f53408d1764762e1167b7`  
		Last Modified: Tue, 05 Oct 2021 23:36:17 GMT  
		Size: 38.6 MB (38612001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af7c6ccc545015c27c428ff91bfea82868a8947ec66360a840e9ae01424f555`  
		Last Modified: Tue, 05 Oct 2021 23:35:53 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:67eba06940960a171938e546beb23a4f44bfddc196aec900383cd8127835bc22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40859960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87692fceca9c314268b1dee8fea1dbcd6e13d28d22f6b28c410202b5cf6ace6e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 23:11:19 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:40:08 GMT
ADD file:ee5acfecc85907b2402d0c02fb3760cd403cd3ea494773ef5c09fd351a71b31b in / 
# Tue, 05 Oct 2021 22:40:09 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:40:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:460ce4384fed12be2e1b021107561ee35cd1ec59424cc3bd30ed6dcb4487b021`  
		Last Modified: Tue, 05 Oct 2021 22:41:06 GMT  
		Size: 40.9 MB (40859768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc47075c25e9a725558ec066bd3e8fecbd5bfff1a91ccc97a3d3d9cd9508c423`  
		Last Modified: Tue, 05 Oct 2021 22:41:00 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; 386

```console
$ docker pull alt@sha256:f43752a433a92dc3e6f648b39a3b974959883ff0bc346ed53785b5b516b13e51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42460143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0ba0ef2c42f463fcacfe5b27b817cdba53ffc621e16d44284f118c9f495ce3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:45:24 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Tue, 05 Oct 2021 22:38:56 GMT
ADD file:618e851010a6813dee96534552c96c3fb71dd6158ad79094182d2ec0c7bdafe8 in / 
# Tue, 05 Oct 2021 22:38:58 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Tue, 05 Oct 2021 22:38:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f8f1b43b3fcfdd7da6037fee94e91acd8f8a01ea20f655495873b40b58004a46`  
		Last Modified: Tue, 05 Oct 2021 22:39:58 GMT  
		Size: 42.5 MB (42459954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3743ac4a7595caf6f43fa10b4f926c6dfa97e4f48bc21fcd5c0afdc07d38f48`  
		Last Modified: Tue, 05 Oct 2021 22:39:49 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; ppc64le

```console
$ docker pull alt@sha256:d1e86741366780328d41011f3f6b47b4952a5747ac382a8e9452ef898fa4f83f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44544413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4426e7a133bae48e6fda19ef98d4971571ead2dac074b4f1d4609303101216`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:29:43 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 04 Aug 2021 22:30:52 GMT
ADD file:d941821de800b392c866c83fb24f5743ef60a7ebfc9a85d084423f2bcdf86315 in / 
# Wed, 04 Aug 2021 22:31:06 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 04 Aug 2021 22:31:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5aea9ecf92cd1ea08204252b06906f016d538959a434604392383782a3acff94`  
		Last Modified: Wed, 04 Aug 2021 22:32:46 GMT  
		Size: 44.5 MB (44544220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49daf7270026bde36af0a2c43da0619f9dfcb146daf7c584824b936db54cfcd1`  
		Last Modified: Wed, 04 Aug 2021 22:32:37 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
