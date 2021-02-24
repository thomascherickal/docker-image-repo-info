<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03.0.20210126.1`](#amazonlinux2018030202101261)
-	[`amazonlinux:2018.03.0.20210126.1-with-sources`](#amazonlinux2018030202101261-with-sources)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2.0.20210219.0`](#amazonlinux20202102190)
-	[`amazonlinux:2.0.20210219.0-with-sources`](#amazonlinux20202102190-with-sources)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:9bd78c849b25ff2367dfdc1341cb30a7918db0bb452a1373afc37722559fabe1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:4608bf17c7b691c5a81ae7f599631055bce8bd5ad8b43e85613c00802ef05ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62221008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68556ba4ccd0c17cb55f71a283997e5e2b4c85ce2a17318af297411a426be024`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 27 Jan 2021 22:20:25 GMT
ADD file:0e86c898f076c0be7554fa629ffd98f1581cc0aeadd702b3876c03b300495006 in / 
# Wed, 27 Jan 2021 22:20:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a441db1e9917658028bdaa8d10a00f6d24aa1f4de352b6b3d327b627207845db`  
		Last Modified: Wed, 27 Jan 2021 22:22:10 GMT  
		Size: 62.2 MB (62221008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:61b78057f1b5b75be20e3e904e60e157dfd51c4112ffef53b607f83c6261fe52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2a59ee8b4934195156ba8b6b4539d632dd8f79b598747a54a08c9122d58cb3dd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449079131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57cdbc7f9d8a3e4fd1dc16736e612142f013423d3ec448d21dd8c8d8db0bb53`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 27 Jan 2021 22:20:25 GMT
ADD file:0e86c898f076c0be7554fa629ffd98f1581cc0aeadd702b3876c03b300495006 in / 
# Wed, 27 Jan 2021 22:20:25 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 22:20:49 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-c05e579179c56d65b75577c4714e241c43b021f6c5595e79ec5f5d693c3e697c.tar.gz"  && echo "a5a576edc920ac864f63ecd88bca4eeeeea9721653e7f1b2eba858721057e122  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a441db1e9917658028bdaa8d10a00f6d24aa1f4de352b6b3d327b627207845db`  
		Last Modified: Wed, 27 Jan 2021 22:22:10 GMT  
		Size: 62.2 MB (62221008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5cfd22c9150a319ed2655cf628b2d5725a7a4704a2ed9003798ea147e02057`  
		Last Modified: Wed, 27 Jan 2021 22:22:33 GMT  
		Size: 386.9 MB (386858123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:0cdc09882f5bc2fe506a6f5ba84ab01b50787c12bcea6a1e4762ab6174450a37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:b288803ecb4fe526981317f7574cc87160132f635300eb3325859e9cb4a75eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61935160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935e8db88df5c8906a27e29bf38705c932802cfcfccd5cd39abf408554badb97`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ff0a8fe0a702ab535f1998bcb0a2460e1a71ccc81075f1abe4d1dc7a2b27922e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63624537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18a544ac7af627f79538f576bcafa956ff023063e30ced7e17a26d4c95ced9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:9bd78c849b25ff2367dfdc1341cb30a7918db0bb452a1373afc37722559fabe1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:4608bf17c7b691c5a81ae7f599631055bce8bd5ad8b43e85613c00802ef05ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62221008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68556ba4ccd0c17cb55f71a283997e5e2b4c85ce2a17318af297411a426be024`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 27 Jan 2021 22:20:25 GMT
ADD file:0e86c898f076c0be7554fa629ffd98f1581cc0aeadd702b3876c03b300495006 in / 
# Wed, 27 Jan 2021 22:20:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a441db1e9917658028bdaa8d10a00f6d24aa1f4de352b6b3d327b627207845db`  
		Last Modified: Wed, 27 Jan 2021 22:22:10 GMT  
		Size: 62.2 MB (62221008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210126.1`

```console
$ docker pull amazonlinux@sha256:9bd78c849b25ff2367dfdc1341cb30a7918db0bb452a1373afc37722559fabe1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20210126.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:4608bf17c7b691c5a81ae7f599631055bce8bd5ad8b43e85613c00802ef05ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62221008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68556ba4ccd0c17cb55f71a283997e5e2b4c85ce2a17318af297411a426be024`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 27 Jan 2021 22:20:25 GMT
ADD file:0e86c898f076c0be7554fa629ffd98f1581cc0aeadd702b3876c03b300495006 in / 
# Wed, 27 Jan 2021 22:20:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a441db1e9917658028bdaa8d10a00f6d24aa1f4de352b6b3d327b627207845db`  
		Last Modified: Wed, 27 Jan 2021 22:22:10 GMT  
		Size: 62.2 MB (62221008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210126.1-with-sources`

```console
$ docker pull amazonlinux@sha256:61b78057f1b5b75be20e3e904e60e157dfd51c4112ffef53b607f83c6261fe52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20210126.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2a59ee8b4934195156ba8b6b4539d632dd8f79b598747a54a08c9122d58cb3dd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449079131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57cdbc7f9d8a3e4fd1dc16736e612142f013423d3ec448d21dd8c8d8db0bb53`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 27 Jan 2021 22:20:25 GMT
ADD file:0e86c898f076c0be7554fa629ffd98f1581cc0aeadd702b3876c03b300495006 in / 
# Wed, 27 Jan 2021 22:20:25 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 22:20:49 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-c05e579179c56d65b75577c4714e241c43b021f6c5595e79ec5f5d693c3e697c.tar.gz"  && echo "a5a576edc920ac864f63ecd88bca4eeeeea9721653e7f1b2eba858721057e122  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a441db1e9917658028bdaa8d10a00f6d24aa1f4de352b6b3d327b627207845db`  
		Last Modified: Wed, 27 Jan 2021 22:22:10 GMT  
		Size: 62.2 MB (62221008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5cfd22c9150a319ed2655cf628b2d5725a7a4704a2ed9003798ea147e02057`  
		Last Modified: Wed, 27 Jan 2021 22:22:33 GMT  
		Size: 386.9 MB (386858123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:61b78057f1b5b75be20e3e904e60e157dfd51c4112ffef53b607f83c6261fe52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2a59ee8b4934195156ba8b6b4539d632dd8f79b598747a54a08c9122d58cb3dd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449079131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57cdbc7f9d8a3e4fd1dc16736e612142f013423d3ec448d21dd8c8d8db0bb53`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 27 Jan 2021 22:20:25 GMT
ADD file:0e86c898f076c0be7554fa629ffd98f1581cc0aeadd702b3876c03b300495006 in / 
# Wed, 27 Jan 2021 22:20:25 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 22:20:49 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-c05e579179c56d65b75577c4714e241c43b021f6c5595e79ec5f5d693c3e697c.tar.gz"  && echo "a5a576edc920ac864f63ecd88bca4eeeeea9721653e7f1b2eba858721057e122  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a441db1e9917658028bdaa8d10a00f6d24aa1f4de352b6b3d327b627207845db`  
		Last Modified: Wed, 27 Jan 2021 22:22:10 GMT  
		Size: 62.2 MB (62221008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5cfd22c9150a319ed2655cf628b2d5725a7a4704a2ed9003798ea147e02057`  
		Last Modified: Wed, 27 Jan 2021 22:22:33 GMT  
		Size: 386.9 MB (386858123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210219.0`

```console
$ docker pull amazonlinux@sha256:0cdc09882f5bc2fe506a6f5ba84ab01b50787c12bcea6a1e4762ab6174450a37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210219.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:b288803ecb4fe526981317f7574cc87160132f635300eb3325859e9cb4a75eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61935160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935e8db88df5c8906a27e29bf38705c932802cfcfccd5cd39abf408554badb97`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210219.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ff0a8fe0a702ab535f1998bcb0a2460e1a71ccc81075f1abe4d1dc7a2b27922e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63624537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18a544ac7af627f79538f576bcafa956ff023063e30ced7e17a26d4c95ced9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210219.0-with-sources`

```console
$ docker pull amazonlinux@sha256:265fe7751a52d6417642fa98d1b4ce32252251b5fbafd3ce3122874d308a132e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210219.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:f0dbd0cc8700d8f2e52d18405f6dfe5977f2ab7bbf901e85cd0ce07a0eea8dcf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542801255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2cefba199f86a2ef9bf699de2d6e3ecb4f979f20a369a7a65928e0b34336d21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:20:21 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-abc7929fca91cdb8ef05600baeb5500309ad7e959bdc5801e05e960937a1887a.tar.gz"  && echo "e0f5a2c5b165bbebd736a75582dc89040c9f64c6d1ddfd84b0421bc44e46de5d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdaa1128d47df628000ceea076363b38d2eef08ce7d1c0ab5303f2c990bb90c`  
		Last Modified: Wed, 24 Feb 2021 19:21:23 GMT  
		Size: 480.9 MB (480866095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210219.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:255e2711fddbc90e0f7c16eff50c2c60b152b173272155b3156f7b695d67f711
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544490662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792b8eba21b647bfa2fa93de4a6f8efc6cdcec0ec21ffc227a7e8192165698b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 18:45:06 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-abc7929fca91cdb8ef05600baeb5500309ad7e959bdc5801e05e960937a1887a.tar.gz"  && echo "e0f5a2c5b165bbebd736a75582dc89040c9f64c6d1ddfd84b0421bc44e46de5d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad3b7efff34c518f97a45ee14bb41ef9f3cbde804a18a4a1e3f35ee7586bfc5`  
		Last Modified: Wed, 24 Feb 2021 18:46:27 GMT  
		Size: 480.9 MB (480866125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:265fe7751a52d6417642fa98d1b4ce32252251b5fbafd3ce3122874d308a132e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:f0dbd0cc8700d8f2e52d18405f6dfe5977f2ab7bbf901e85cd0ce07a0eea8dcf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542801255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2cefba199f86a2ef9bf699de2d6e3ecb4f979f20a369a7a65928e0b34336d21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:20:21 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-abc7929fca91cdb8ef05600baeb5500309ad7e959bdc5801e05e960937a1887a.tar.gz"  && echo "e0f5a2c5b165bbebd736a75582dc89040c9f64c6d1ddfd84b0421bc44e46de5d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdaa1128d47df628000ceea076363b38d2eef08ce7d1c0ab5303f2c990bb90c`  
		Last Modified: Wed, 24 Feb 2021 19:21:23 GMT  
		Size: 480.9 MB (480866095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:255e2711fddbc90e0f7c16eff50c2c60b152b173272155b3156f7b695d67f711
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544490662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792b8eba21b647bfa2fa93de4a6f8efc6cdcec0ec21ffc227a7e8192165698b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 18:45:06 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-abc7929fca91cdb8ef05600baeb5500309ad7e959bdc5801e05e960937a1887a.tar.gz"  && echo "e0f5a2c5b165bbebd736a75582dc89040c9f64c6d1ddfd84b0421bc44e46de5d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad3b7efff34c518f97a45ee14bb41ef9f3cbde804a18a4a1e3f35ee7586bfc5`  
		Last Modified: Wed, 24 Feb 2021 18:46:27 GMT  
		Size: 480.9 MB (480866125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:0cdc09882f5bc2fe506a6f5ba84ab01b50787c12bcea6a1e4762ab6174450a37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:b288803ecb4fe526981317f7574cc87160132f635300eb3325859e9cb4a75eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61935160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935e8db88df5c8906a27e29bf38705c932802cfcfccd5cd39abf408554badb97`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ff0a8fe0a702ab535f1998bcb0a2460e1a71ccc81075f1abe4d1dc7a2b27922e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63624537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18a544ac7af627f79538f576bcafa956ff023063e30ced7e17a26d4c95ced9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:265fe7751a52d6417642fa98d1b4ce32252251b5fbafd3ce3122874d308a132e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:f0dbd0cc8700d8f2e52d18405f6dfe5977f2ab7bbf901e85cd0ce07a0eea8dcf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542801255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2cefba199f86a2ef9bf699de2d6e3ecb4f979f20a369a7a65928e0b34336d21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:20:21 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-abc7929fca91cdb8ef05600baeb5500309ad7e959bdc5801e05e960937a1887a.tar.gz"  && echo "e0f5a2c5b165bbebd736a75582dc89040c9f64c6d1ddfd84b0421bc44e46de5d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdaa1128d47df628000ceea076363b38d2eef08ce7d1c0ab5303f2c990bb90c`  
		Last Modified: Wed, 24 Feb 2021 19:21:23 GMT  
		Size: 480.9 MB (480866095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:255e2711fddbc90e0f7c16eff50c2c60b152b173272155b3156f7b695d67f711
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544490662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792b8eba21b647bfa2fa93de4a6f8efc6cdcec0ec21ffc227a7e8192165698b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 18:45:06 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-abc7929fca91cdb8ef05600baeb5500309ad7e959bdc5801e05e960937a1887a.tar.gz"  && echo "e0f5a2c5b165bbebd736a75582dc89040c9f64c6d1ddfd84b0421bc44e46de5d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad3b7efff34c518f97a45ee14bb41ef9f3cbde804a18a4a1e3f35ee7586bfc5`  
		Last Modified: Wed, 24 Feb 2021 18:46:27 GMT  
		Size: 480.9 MB (480866125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
