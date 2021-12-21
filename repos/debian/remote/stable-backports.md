## `debian:stable-backports`

```console
$ docker pull debian@sha256:369878ece1ba8267ad26463124b9504ad1d90bab3a388ff124e49775dbb14d54
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
$ docker pull debian@sha256:07b27106f4ed7fd54350a1d95a5832f4087c1636f4dd41bc7473d78d4f42ae06
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54919274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e2ea0cbd8c26fadb1300997c960a70c7acbc453e96b98698ab2bcfae1ca11a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:11 GMT
ADD file:9378b685ba5d4d29919e2c751e51e9a375e8f77e04325cc6c39e530f59b41609 in / 
# Tue, 21 Dec 2021 01:24:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:24:14 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8bb8ae9b0185f5d889dc74832bccc98639959d52f66fa45c7afd30917bb4e60a`  
		Last Modified: Tue, 21 Dec 2021 01:30:38 GMT  
		Size: 54.9 MB (54919051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d48b6a0e9c67d9fe549f3d4acc3953ff9f0ba63bd9d07b53372dab0682feb9`  
		Last Modified: Tue, 21 Dec 2021 01:30:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:4acc44d907bb3547c6143aa11f9d4fad4b6dcf51ac4deff7ca2af12adb928bc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52453721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b2b40911fde04a64cd859144b5ec8e4b1847727b564c7ad90b3049b143cd47`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:54:37 GMT
ADD file:4f3f22afdfdaa22f59d1efc385d16b52868d60756e17fd6b26394e1d5be7f850 in / 
# Tue, 21 Dec 2021 01:54:38 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:54:50 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:956145b992cc940fbe651aec596803c4a6aa0af6d3d091062d0fcb3cdf18264a`  
		Last Modified: Tue, 21 Dec 2021 02:11:48 GMT  
		Size: 52.5 MB (52453498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf3a27f9a8c7a80d308db7996f715e085712416a78714b101913090e3568346`  
		Last Modified: Tue, 21 Dec 2021 02:11:59 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:3b9d7a5e898b0dc129d9e3a41becbb306e47fcefb98f1a2ed4cb9887d958f35b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50134475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1477a0e7e7d58e64624d8706f0f1b42eb6a11db85b962f8c41454abf3321b1d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:09:40 GMT
ADD file:544c822f836f49f5e182ed70d111afa02054c3f56a9f3a24a0256dfb9b28455c in / 
# Thu, 02 Dec 2021 09:09:41 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:09:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f0b1154e6665dd07060d16b5ad6b925d011f05938e36d9956a816a3e5607445c`  
		Last Modified: Thu, 02 Dec 2021 09:26:43 GMT  
		Size: 50.1 MB (50134253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e900ae0d6eaf4287f4122bc7354d2f2be9baa70f71ac689f2f29fc5e17dab3`  
		Last Modified: Thu, 02 Dec 2021 09:26:55 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b01ad767b5b4003c5dbe8620b866ad897d72facce39ff0c7dc1de0378477a8fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53604804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:beb29c18e2752562335590c8135636f0624c9b4ce6d97a00cd1fa3e0cede7bdd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:03 GMT
ADD file:7f6adb94fd06bbaa06d615f8d997a5dea3eea2bfe451ea6af5a85010bbf6ce56 in / 
# Tue, 21 Dec 2021 01:44:03 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:44:09 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d39780c72a13b02b33aaeb60c4d3e849378d96e0a6e0578b855a5f5becb8cd14`  
		Last Modified: Tue, 21 Dec 2021 01:51:57 GMT  
		Size: 53.6 MB (53604583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fee78b69a0ae5354c82366cdaaed9ab501288c646a2a3cd65e322a40c68f1f`  
		Last Modified: Tue, 21 Dec 2021 01:52:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:9a0a0cff9ae70e80fadcfb1283d4ea22de85272d2145c91a90e62a44cf4380f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55925573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60a0299c560d7055ee1b385597b66e9f30fa5cd0d660b07864645af5d323edd5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:38 GMT
ADD file:efe6538a62fd559c8b5b161326aa8d88a559e80bbcac8326bc2797b4a8755112 in / 
# Tue, 21 Dec 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:42:46 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:eeb955a987714dea410926ad2c657ba42f543f9c87f31c3c6da72ac6f8da3459`  
		Last Modified: Tue, 21 Dec 2021 01:52:34 GMT  
		Size: 55.9 MB (55925350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696dd31ea2a8b6b036f64799f4773ab88add8a3cbb58a2d08c8d6efffd8e76fc`  
		Last Modified: Tue, 21 Dec 2021 01:52:44 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:651fa3ef9190164cd4beb2dba71a4ee72e0b20f514e5249b3667a7a64982a16e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53184080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:575a117ee345e272252a856b5e78cd770e37911edef9d5d268bc6aa365b79522`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:12:13 GMT
ADD file:edc7c8309e49aea9304c225740ae1ef4a331832bfaee41c524df95ab29f48795 in / 
# Thu, 02 Dec 2021 03:12:14 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:12:21 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a25baf1522352f088acb1da1b108d77b0bcb49d0271d4182caae670825e713b7`  
		Last Modified: Thu, 02 Dec 2021 03:49:56 GMT  
		Size: 53.2 MB (53183854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f3bd27519e72e81d694f57537f30df2a572a6a732ab53c55893891b50c6fc1`  
		Last Modified: Thu, 02 Dec 2021 03:50:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:612a23a8d5168b14c5fa70032097565488aef2dedf12f094bc58d9052d982960
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58819817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540b93cb23ca4080d4610498609e20f2715cc09c816160639f9c2404fbf7c549`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:24:11 GMT
ADD file:c3d40efaf33d2455dd6715c1167d413e62556f2f94475afb72e120d99841bc62 in / 
# Thu, 02 Dec 2021 07:24:16 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:24:31 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:672360b9a6ab75e79b4d477b6e4c3b29bfdf938b152f44e6d1a93e7e18edda54`  
		Last Modified: Thu, 02 Dec 2021 07:34:35 GMT  
		Size: 58.8 MB (58819591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efc5f6b428c035886496c11b594e0172e25a4182c755ad3e10e87220af13fa7`  
		Last Modified: Thu, 02 Dec 2021 07:34:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:9cd507b82d2040e0aa5b257e8706538619dedcd351ae6261582b7e8abd24722f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53194893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a794a8359e5f59e7a15c7400f55afb17e05bc73072cf13205bec7476d143a53b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:00 GMT
ADD file:16e8e0f2c31bbb1175dba1423169ce15b023b8d964ab8aa7d94b78431a2fa60f in / 
# Tue, 21 Dec 2021 01:44:02 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:44:09 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8aac6c6e3d3fd37ea4df120da2a600b462626de6fb0d0beadf30fc203e5c093f`  
		Last Modified: Tue, 21 Dec 2021 01:50:05 GMT  
		Size: 53.2 MB (53194668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319c559de6e487e673ed78305a67fbed5fdeae75ad913d7de453f1cd5fd4b0ab`  
		Last Modified: Tue, 21 Dec 2021 01:50:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
