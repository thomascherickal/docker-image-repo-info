## `alt:sisyphus`

```console
$ docker pull alt@sha256:ab6b05d95315e4d85491608fe221c0636d05b5261ab27c467a56669ae549b04f
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
$ docker pull alt@sha256:f7b819218c2dcdd9a891434cd5cc83383fe279abcc2ce88474a23ce6d65c3e90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40465011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d40c73c0745816bb5664f2d8794fee0e390aa7ad39e7fb66e195226b5526ff3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Aug 2021 22:28:37 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 19 Jul 2023 23:20:37 GMT
ADD file:19ddac8e51abe2241a4b4f6bfe90dad9838c8d1658bebd1746e685a40e0b37b3 in / 
# Wed, 19 Jul 2023 23:20:38 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 19 Jul 2023 23:20:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:188450edefdd410a0d1e58be6ea183a9b704d681bf5caf292dd31fc6b6bf9910`  
		Last Modified: Wed, 19 Jul 2023 23:21:18 GMT  
		Size: 40.5 MB (40464820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0486df7c5bbbf8a15e8e79933c2835e867432fe1f7ab0513a1e8a6be01015a`  
		Last Modified: Wed, 19 Jul 2023 23:21:13 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm variant v7

```console
$ docker pull alt@sha256:71f9b95fd028b4821f5fbbd5209a543e82a1f7f188d5b291889a4e3b0fddd4cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37365930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421208568a3897b86324fd6d4a4154f054866abbb9be224087cb7423ad6d6e35`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 13 Mar 2023 16:13:31 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 19 Jul 2023 23:57:37 GMT
ADD file:8d9cbe86162f5986c16e5fc83bf893f40c0ec043f27512fb8441dadc19e48f8a in / 
# Wed, 19 Jul 2023 23:57:38 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 19 Jul 2023 23:57:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:12208bb6fe46a2e2b2f1e9acf1160227ef9af04a1936a852e45aaf9e7e5d4e60`  
		Last Modified: Wed, 19 Jul 2023 23:58:17 GMT  
		Size: 37.4 MB (37365738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261742c8101d0708ad71c9169f50a4a33531ac0b165570ecd0430612cceae352`  
		Last Modified: Wed, 19 Jul 2023 23:58:11 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; arm64 variant v8

```console
$ docker pull alt@sha256:f544153ca70345037f7b96f6146b8f0ea9abaef4a2e8563d60568fe3e2894de5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38849597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb64942701a898e0995217f64511508e5084b5a41f63680fbb9ab54f04f36a1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:39:36 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 19 Jul 2023 23:44:40 GMT
ADD file:f15f1d9afae47960133823ab7de848d63290cd6fe2994fdaf5b108479b8463ec in / 
# Wed, 19 Jul 2023 23:44:41 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 19 Jul 2023 23:44:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e0f18648debac30a5217e72c213cad95c9578c9b88622de1d121b38918c445f2`  
		Last Modified: Wed, 19 Jul 2023 23:45:17 GMT  
		Size: 38.8 MB (38849407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8271bbf08f85e96b959f6c18ecfd1a7a7c95b57a292e3e6ccfe96a58fa64880c`  
		Last Modified: Wed, 19 Jul 2023 23:45:13 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; 386

```console
$ docker pull alt@sha256:a6100b874dd30c33f0b5460538978bc8aa03d5a184c9ed1623eb8b0f122c916d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40632982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5f1f8790a69bd3fb2dddc5a742733d59ff079fb6db5ea1db5cad357221cba9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Jul 2023 23:38:46 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 19 Jul 2023 23:39:09 GMT
ADD file:0fa6b359de624e4076d274c559396de736d2337c956729c93df17ac0a6598ff8 in / 
# Wed, 19 Jul 2023 23:39:10 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 19 Jul 2023 23:39:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c9ffff7f34c96866e0fe66169bf93a2b177fdf3dce30f1e8fa78d84d00100fce`  
		Last Modified: Wed, 19 Jul 2023 23:39:56 GMT  
		Size: 40.6 MB (40632792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf6e58abb187f85668c3bc5ec7ebbb48202cd02fac0df3bbd7cc8171446d10a`  
		Last Modified: Wed, 19 Jul 2023 23:39:48 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `alt:sisyphus` - linux; ppc64le

```console
$ docker pull alt@sha256:edf091a895a80878a7cb8c2ded7432461ac5b4b11eb89c994fb888738bfe8ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42771813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2338ae42101f0bcbf6bd2af529acfecdf8291970ecb9b7ae7d436a12cb939d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:16:44 GMT
MAINTAINER [Alexey Shabalin <shaba@altlinux.org>] [Mikhail Gordeev <obirvalger@altlinux.org]
# Wed, 19 Jul 2023 23:25:11 GMT
ADD file:6057a1fb3352c82bd7a102d31bdc6974b66f7aa2cba0960351502cbe531e0f47 in / 
# Wed, 19 Jul 2023 23:25:14 GMT
RUN true > /etc/security/limits.d/50-defaults.conf
# Wed, 19 Jul 2023 23:25:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:31fdd6f51f73634ec97fffcb8b717c7ad505c570938bf638e070ad29ebfb984b`  
		Last Modified: Wed, 19 Jul 2023 23:26:24 GMT  
		Size: 42.8 MB (42771621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308214b9452ed2fdc8f103a93cf090159fa64d5d86a1c7a9b6a366ed895afbde`  
		Last Modified: Wed, 19 Jul 2023 23:26:13 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
