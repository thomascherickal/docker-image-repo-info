## `debian:stable-backports`

```console
$ docker pull debian@sha256:713c6d47a68d136a00cf26fccc060f63a03fd05ad9ab4de9d228e5a4015c83ab
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
$ docker pull debian@sha256:5da3c1908186eda7376c90fe065d3aabfed088048c6730a530aeda08b5500dd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54999645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20555756d69411fe29f657609491c5e61563c9bb7643b32f8b2f887e2659bcf6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:21:28 GMT
ADD file:bcb1ce267ba1b1299bb26cb6b0607643a46a017bfbe8333de7e3a37ae1d16032 in / 
# Tue, 12 Jul 2022 01:21:28 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:21:32 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d6d0c636c9e6d290934ea337ff3ea173a84e6714f24819eaedfd95b85915384a`  
		Last Modified: Tue, 12 Jul 2022 01:26:49 GMT  
		Size: 55.0 MB (54999423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b879d28db041b19736df4f71b35e9d36adcea57909c15d8586cd1ef0c39e8d21`  
		Last Modified: Tue, 12 Jul 2022 01:26:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:54549d00a7c21427e013ef210273fae7231ffefcc1c29a3940c49d37dd84d639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52537083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2864c3e7108acc44b7b618554d0a31c9465b218084b4411081b53ebcd5ef5b45`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:53:53 GMT
ADD file:02fd910cc563733b6b724cdb91c80a999c47ae6c9a1dbe9bb39a630159d4550c in / 
# Tue, 12 Jul 2022 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:54:07 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6853bb519f7a85c62eddef077f0ee097f64fe120a93583c92fddde2dc0706c7b`  
		Last Modified: Tue, 12 Jul 2022 01:07:53 GMT  
		Size: 52.5 MB (52536861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207a54dcbf5517accfb1e471b35a23ea89f64784b43caf8365d2e72c622d8ef1`  
		Last Modified: Tue, 12 Jul 2022 01:08:04 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:3492ae63f41fc39bea5c11d1e3ddfc907282120f4f389aff19ba86a960e55e34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50195134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d672057462335a5f96443abc2900bf75c12f8a8ee1deb5380d37f1c854156c66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:03:28 GMT
ADD file:ce3a635d2ec00c101e98c74a305991612941b0055614d9c777c5aa10ab6c8c79 in / 
# Tue, 12 Jul 2022 01:03:29 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:03:42 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0b51cd557560e414752831e67bcfd89cb430e20a2245d6de6b2e163ec5dad1f7`  
		Last Modified: Tue, 12 Jul 2022 01:17:01 GMT  
		Size: 50.2 MB (50194913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7cd45baf22e545e6b08dd1d49478117371d67851c3e625d00b8d073a6d8088`  
		Last Modified: Tue, 12 Jul 2022 01:17:12 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:4231f2ea6ce40364ca7d8d1f533a32cbd6c6e7f50e4ed665079ca52419ff038e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53683372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3ca347b365d84f677dac8188a5593beca4d71e73002680a95294c9bae12b8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:42:00 GMT
ADD file:0d6d31f56f31acdde787a277c21886ee3b25087b509730a2f2ad46110f0e4373 in / 
# Tue, 12 Jul 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:42:07 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:daa333d9b33fef63ba6f1f9dd9160e035cd096dcc8d747c77233c000262d3467`  
		Last Modified: Tue, 12 Jul 2022 00:48:50 GMT  
		Size: 53.7 MB (53683149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57180f860626256ba8267ebf3ff8dac4cd94890975e8851566b29832fbd6cb48`  
		Last Modified: Tue, 12 Jul 2022 00:49:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:26a0da71a2ba3591115c9878f5a5edb3baf102fe91670e35ccce524a73cf43d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56002005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e5f2e3c4271fc5c379b4bae9c58638df13547177bc534439692321fc9ce1c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:53 GMT
ADD file:c7bc307cd23459ccce030ca00fc0944a4a9088bc73c3a1694c92e163dc5f938c in / 
# Tue, 12 Jul 2022 00:40:54 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:40:59 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8d1153e4af373ce56f9df7ac71b093b2594b621cb8b6fb27893261bfaa17d958`  
		Last Modified: Tue, 12 Jul 2022 00:47:56 GMT  
		Size: 56.0 MB (56001783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae97a6fee82a6e2e729687e0e0f461c928e8c39d321fd00ba2f21fa46c29c60`  
		Last Modified: Tue, 12 Jul 2022 00:48:07 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:90a04283a91bacfd08fefb1f911456d05801649870a1ae46a7a6321616dfa266
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53263527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3591c0db2ac1fc601fe44b4c7147c22d0d122534c48b30391c0019ffa9dd66f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:45:06 GMT
ADD file:659356a7807ff0035dc510130909c221a049c585036989d0ce9f5027ad89c308 in / 
# Tue, 12 Jul 2022 04:45:12 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:45:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:135d9662eca45a17273c44e35394fd544be26103818019defda5f02b8eff1eb0`  
		Last Modified: Tue, 12 Jul 2022 04:56:08 GMT  
		Size: 53.3 MB (53263302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c831cf32da65d40ca9fb773233e5639424f0681c3925039793df5a66857b6202`  
		Last Modified: Tue, 12 Jul 2022 04:56:18 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:de2489e33bfa65ec99d018ddb35d48e24c5f2e89e2f5dd91322bf92acd13814d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58895907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c00f33b5d5ad91ce4b53e5f1bb92f343f445ce0553eecc59c701ed9db5fdfe43`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:28:16 GMT
ADD file:2212464e195bc1af7220bfadb9e7dee33af051ed5bb42b3f486d9ee2f9d727fd in / 
# Tue, 12 Jul 2022 01:28:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:28:33 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c302b0ef08e182e287cd8cb7c5c504c624efa1c1a0062485cd78ac7062137552`  
		Last Modified: Tue, 12 Jul 2022 01:42:11 GMT  
		Size: 58.9 MB (58895684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605487b5e5ad1284471f735f13c2952efbc3215310aa3d3a74732b32ce522879`  
		Last Modified: Tue, 12 Jul 2022 01:42:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:3b47334ed0d23c8e5eac5df84243d6a14aa97d43eabb34357ff97c3752cde27b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53269193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680a90575ab8e9d2acd12c9aed6e92c87c10e33acec6e42c610b82be5f92276a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:47:01 GMT
ADD file:ed009ff381c2a0d8393de98bf900ae04ba3fe2b17138f95be310ba8609739e7d in / 
# Tue, 12 Jul 2022 00:47:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:47:19 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:26177b6f29e3cc38c0e209539f17f4264317f877f4487bec96a274fdaf6d4c6d`  
		Last Modified: Tue, 12 Jul 2022 00:55:37 GMT  
		Size: 53.3 MB (53268968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f323d90a31f790b3f8a885fbcce068592a7409626f395d4dc2ffddb16dc50b71`  
		Last Modified: Tue, 12 Jul 2022 00:55:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
