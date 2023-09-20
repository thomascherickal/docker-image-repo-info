## `debian:trixie-backports`

```console
$ docker pull debian@sha256:7b2cdb7ddbcf98af12707fd4b96734657ff93ec9aa091457de939fc0780a37f0
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

### `debian:trixie-backports` - linux; amd64

```console
$ docker pull debian@sha256:259fa44d8d662dd38571d125ebbc19013906dedd0bfef64c5abf5e9c5ccb2025
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49514984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e714484ad17f6c3db573092a3fd18a20f461467541ffe7aa93f417c86cc1c9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:23:27 GMT
ADD file:34ee641d9bad402a9422c8f96269ac2c74e06369bc362a916c8cdb087156bf70 in / 
# Thu, 07 Sep 2023 00:23:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:23:32 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e32a7bcba7c1847ff42b03e176da563d6447b045a6f2d5a9ece6acdce60297cc`  
		Last Modified: Thu, 07 Sep 2023 00:30:28 GMT  
		Size: 49.5 MB (49514761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19671cda3819257e821f236a318b8029317bec3f4ab00f5f06597ee42790a259`  
		Last Modified: Thu, 07 Sep 2023 00:30:37 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:02b0fef62da83048656918de9dbe86bb4e8ba00c03404cc332119b9a84607d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47170304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63dce2d5249720881dc3d902cbbe7cfce273bd5196732ed855ddbfc2a63d35cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:52:20 GMT
ADD file:c6e1ebf545b4fe8a3d6b8e0eccf515df1d8291411d23a0e5002f40428db8b992 in / 
# Wed, 20 Sep 2023 00:52:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:52:26 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e7cf8ed3fa4a717011b456890e76475bcc7f559140833924436b7fe1266ee31f`  
		Last Modified: Wed, 20 Sep 2023 00:58:49 GMT  
		Size: 47.2 MB (47170081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c274f8408d62d3f35ed32f1ed61124f7711f0f3b6c8c57441b7ed67daffc1344`  
		Last Modified: Wed, 20 Sep 2023 00:59:03 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:480a60021ee57ea2d746a3f0fedc46e1a3cd350b774a46280500948f14cb6686
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45010719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c190965f46ad391a31ac02fef4044f6a9f1b1da69aa6363affd72cc0e1de1c5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:00:27 GMT
ADD file:56aa0cd11d12862eaf421a2ff6a2a518ae07f7d6180a2f0f58a9d10930215950 in / 
# Thu, 07 Sep 2023 01:00:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:00:31 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cbe28254d81156b7683ab6feb96334538a6b59d12717973205a1077d3bcabba5`  
		Last Modified: Thu, 07 Sep 2023 01:06:54 GMT  
		Size: 45.0 MB (45010494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75612bc00e38e620a86bc7f83e39c50acd61e033b88bbe565894514dc82682e`  
		Last Modified: Thu, 07 Sep 2023 01:07:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:0a4920e0ae737125747f8d0ba6feb8baf957137c17cb26a790a7cd237e525625
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49404723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dacc26ecfc7bd73e1212c9d1770f92debaa64c92afb4154f54a57f6ba522e67e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:58 GMT
ADD file:dc9be3a1e3e1904a1eb81053b568b583a58307e861fc56fb1b7ce9349d2faa18 in / 
# Wed, 20 Sep 2023 02:45:59 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:46:01 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4d433462e04ded836d58eebb0fee68803768bcf3c9f92338a2cdda77bf7bef8d`  
		Last Modified: Wed, 20 Sep 2023 02:51:30 GMT  
		Size: 49.4 MB (49404499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2971bd829e6d4cab6e239fae43246325496a884c068e59a494f1d8c31c6f3b2c`  
		Last Modified: Wed, 20 Sep 2023 02:51:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; 386

```console
$ docker pull debian@sha256:2e8aa15dfe39f91efccec6724beaf24b6b75622928c57111dee5c40a7a085278
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50485014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9eafd5bf98c3e8921e4cdf51e93be9d3381ddd32d5e8ff044b417e5fae93854`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:44:37 GMT
ADD file:9e992ca17751b113240a189433e8f77647c4ebe62d129da1b528a8d6a3702972 in / 
# Wed, 20 Sep 2023 00:44:38 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:44:42 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cd505a05e9a1d549793b6c0278e192920932cc3051d24604cbaee75803a68342`  
		Last Modified: Wed, 20 Sep 2023 00:51:58 GMT  
		Size: 50.5 MB (50484788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495160785dcfdd8c94db8ad1bb609f1a449ff3c675d0af7113ef956ce22714f2`  
		Last Modified: Wed, 20 Sep 2023 00:52:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; mips64le

```console
$ docker pull debian@sha256:fd75b20b33ce3c61e9e00dcdcdfbbc0c700555a43d73a1d7009feb2b3b57a7ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49357733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420c0e3b3e3eddfaa5f8cf23d9abdfdef7702c48524e17190860c85c32c3d97a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:15:52 GMT
ADD file:83fc4a798915040b0cd8aee9a3ff972cb051d033b36a5b578933e29e1b55dc9a in / 
# Thu, 07 Sep 2023 01:15:58 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:16:12 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2b910e4082f491e2e9e9e85a065d99a76c730b5911893631d48aebe5740c1e71`  
		Last Modified: Thu, 07 Sep 2023 01:27:12 GMT  
		Size: 49.4 MB (49357507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3e6d662e4d850714a68ea7cbbe46bb31e4ee1d67b71e4adfd37f48cb7c38df`  
		Last Modified: Thu, 07 Sep 2023 01:27:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:863634a609f64c12275b46cb88c8c93f4c88a7cba13de701c0436694538a1bb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53456239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f80acf3ce5ed814d9fbcdd7c6ba41b9d27f2743efa5df461c8aaba2b33b2117`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:53 GMT
ADD file:1d1937f8a4890754546a2c77f05e3e1d993bb4a60eeb0ed016941880313061ae in / 
# Thu, 07 Sep 2023 00:20:56 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:21:01 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:97f3d0760a8a2cb56d7bb85c16a268c56539a98f9e55ebfcfe233a88995c86d9`  
		Last Modified: Thu, 07 Sep 2023 00:27:49 GMT  
		Size: 53.5 MB (53456016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb718989ef7f449807cef0bbe90fad57e950da7dfcae3fb29597cb361d4123`  
		Last Modified: Thu, 07 Sep 2023 00:27:58 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; s390x

```console
$ docker pull debian@sha256:be8a86d30b3d566ee2770d995b97be414c749f8da0b24f4a1bcbda9023b7c345
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48761016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:725bee4a9e8209644464f12711e7934c3ead0a714aaea7c01b083ce23ef9fe81`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:57:24 GMT
ADD file:77b51e0abb2ed786e762b44ab5463930ac60fc37a4a4404ee62cf4653a99e1fa in / 
# Wed, 20 Sep 2023 02:57:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:57:35 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dcfbcf60cde4d1764ae5735832195c5a57365459959cebb93c0e57bd40fd54a4`  
		Last Modified: Wed, 20 Sep 2023 03:02:19 GMT  
		Size: 48.8 MB (48760791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acb268ceee4d4f110eb645722feb8a6e9ae8498ff921810425b00ff62d3bef0`  
		Last Modified: Wed, 20 Sep 2023 03:02:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
