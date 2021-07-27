## `buildpack-deps:groovy-scm`

```console
$ docker pull buildpack-deps@sha256:5d45d1aa2dd5bcc2d994a37dbfa16035d8a27c67b05ba2861ae2c9eee926e74c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:groovy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7440ef2be4f936796d0c0522fe040f0173577145a3a514a471273f830dcc669d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95890911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2659a59a7c999902424b9360dbfdde2d86ba21ab2b274e003af76f18011c3975`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:47 GMT
ADD file:23ff7ae476ddf97e5dbaf417c06418ae4d8d49a88acb92738bf03fb4a22eeca3 in / 
# Mon, 26 Jul 2021 21:21:47 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:51:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32f3531c8415258308e8d8dda886004bc90cdf4793f9b97c6f33e7903036294f`  
		Last Modified: Mon, 26 Jul 2021 21:23:27 GMT  
		Size: 31.3 MB (31342970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f6d92cca49e420ae1a96a98a170c6c6f4d0cfafc25512a58edbb283cb30eec`  
		Last Modified: Mon, 26 Jul 2021 22:12:20 GMT  
		Size: 5.4 MB (5405030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975758a58780cd2adab51b5973557d092bcde9cdd6c9d23cd120f85919671daa`  
		Last Modified: Mon, 26 Jul 2021 22:12:19 GMT  
		Size: 3.7 MB (3664052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746170fb973f7fb3cefba229af451c7bd2ef9e1410913ef79ed93718b053ed8e`  
		Last Modified: Mon, 26 Jul 2021 22:12:41 GMT  
		Size: 55.5 MB (55478859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e8b412072b1e627f2baa5a6472b1cff517a4826df277dd2c0ea9c8f31b013920
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84595342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a09d99d4493d757bafb5ca8aa3bc8862809476fb2879ccef64e8788f65852a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:33 GMT
ADD file:80b5f21ffac906a8416f39204cb526afaf64f15559123cb3a8fb311e312a703f in / 
# Tue, 13 Jul 2021 23:21:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:55:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:55:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 01:56:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ad80ac50e31c20115b0366841c81a92d1916a7f2113255fe1125324250475e7`  
		Last Modified: Tue, 13 Jul 2021 23:26:54 GMT  
		Size: 26.3 MB (26312397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87836ed84bb5f0e1d7b61439e8458826efce0a52158d32f928c2efc41367ac4`  
		Last Modified: Wed, 14 Jul 2021 02:19:01 GMT  
		Size: 4.8 MB (4840704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4a0657bf22de96a1925b7c31d415ed9eff49f3b00971444459ee9b696832ef`  
		Last Modified: Wed, 14 Jul 2021 02:18:59 GMT  
		Size: 3.1 MB (3140633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e419af2ccab0c7223c92ce4cd8deaa2cdea7e08e02b9636ce5f7193b06162f6d`  
		Last Modified: Wed, 14 Jul 2021 02:19:51 GMT  
		Size: 50.3 MB (50301608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d8be36aeca7881f07606650471b321d1c03ff2e2a6e00eceecf98ee200369d2c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94354227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d5ff08f29c67d43acd111485d1b17a5d43727569816a4443a40b56be91cd90`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:49:05 GMT
ADD file:3a4e8fe51fe7ca76be749ef0b92043e9e9b241a7b6f196fbe2a8bcde49c5b3e7 in / 
# Mon, 26 Jul 2021 21:49:05 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:30:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:30:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:31:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06dd9de3e7a96bf4bd49de5d681cb7062c5b3012c0f1b1bcd9d059380f55a1d2`  
		Last Modified: Mon, 26 Jul 2021 21:51:22 GMT  
		Size: 29.9 MB (29876744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647214296e105ce8a92eb9ba4b666f72064bb32c3394b392673e54540e1f06d3`  
		Last Modified: Mon, 26 Jul 2021 22:41:30 GMT  
		Size: 5.4 MB (5372238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ff548ea8c26b94143a36cf8245ff00840af96ba22465a184cf4390eb135cb0`  
		Last Modified: Mon, 26 Jul 2021 22:41:29 GMT  
		Size: 3.6 MB (3634615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba06c5b905e953629da8a61f68f094e7248c4f5be8b4bc879a509cfa3c27bb0`  
		Last Modified: Mon, 26 Jul 2021 22:41:52 GMT  
		Size: 55.5 MB (55470630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bbe6ad4f8fd8f43dd50545a1348aa43910938be03a4f4698713566ca9e058474
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110868939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913ec8562330786224cf40283e34dd89c7684e6d1d7a0f1b4f1e95fde3e7513f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:22:45 GMT
ADD file:d810eebdcea73da6a0b9c4546fc356b13b60da24827c29923375b8e08f2195b4 in / 
# Tue, 13 Jul 2021 23:22:53 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:30:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 02:35:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97b0da8da7b9eb227e28852cb467ba3f76ac379708648200f035c072d3bbf4eb`  
		Last Modified: Tue, 13 Jul 2021 23:28:00 GMT  
		Size: 36.6 MB (36562496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19019a66a1c7600fb2159a63b0e68f36b9d9f55e9e56ae7b70139ac7565616c1`  
		Last Modified: Wed, 14 Jul 2021 03:24:17 GMT  
		Size: 6.0 MB (6040945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7e113d40008d7a4f01ffb65b6bee553ec1af6ea5935387bfc2677d6a9888ba`  
		Last Modified: Wed, 14 Jul 2021 03:24:01 GMT  
		Size: 4.5 MB (4522053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f499186162dbbd18ecdc41e48723d94384601a434160e441c62890afc5a08b62`  
		Last Modified: Wed, 14 Jul 2021 03:25:24 GMT  
		Size: 63.7 MB (63743445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:6f4a5d5e16f76d8f66d13a7ecf54e59a7960e1e3e409927c5a8332ff77524ebd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85351256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71693fd376bbe1711bb45be917fd68798a2dda4631d224c6be2d2d05efa83eeb`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:22:55 GMT
ADD file:b6af3eb17fceb12f32687c7392bcce88c50d169e89e08ce383b0d151f15e35b4 in / 
# Mon, 26 Jul 2021 23:22:57 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:04:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:04:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 00:08:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2854584d46af51653126c966b1f675e9fc2d73b12251e85306724f0c3caeabb0`  
		Last Modified: Mon, 26 Jul 2021 23:42:20 GMT  
		Size: 26.5 MB (26524072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22b0f3794b3c283f9fbabd391721114f4de25a212c0905b7daf2ebc9b710aee`  
		Last Modified: Tue, 27 Jul 2021 01:01:13 GMT  
		Size: 4.9 MB (4922828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fe037d460c34fe039d04c5bb4e64cc63b97f55de632b48bdbc5320d075dfb`  
		Last Modified: Tue, 27 Jul 2021 01:01:10 GMT  
		Size: 3.2 MB (3179172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8939850a31790ac98d18e8170f151d862abcd74592a8b0d488c2b6ea0b7d29`  
		Last Modified: Tue, 27 Jul 2021 01:03:21 GMT  
		Size: 50.7 MB (50725184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:53d6b22022c007f727fe7e889d59b77cf0877268f00b9a9ac5d1fc5276ba7cb0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (102032047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9def7103978beb68fb5f62404cb14ee9ed68eb5f4fbac0dcce350a0716a787c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 20:55:22 GMT
ADD file:2f05dac9c72fd83b64830702accb3e1582661b82178055406f437be01591b038 in / 
# Mon, 26 Jul 2021 20:55:24 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:42:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:42:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:42:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ebc30c62ba1234efc4428ed9d6d0f4f9b031ce916310c2d82b099cf9d02d1dc`  
		Last Modified: Mon, 26 Jul 2021 20:57:18 GMT  
		Size: 31.6 MB (31578338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe77f2c779c381b74f333923da8ee43a24119720802950c7670ba4d2f1b887a`  
		Last Modified: Mon, 26 Jul 2021 21:49:18 GMT  
		Size: 5.6 MB (5629737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac8e5f5f1362b078cf4da3e0b61a4088d2fba405fabc3eeca03b446a08e083f`  
		Last Modified: Mon, 26 Jul 2021 21:49:18 GMT  
		Size: 4.2 MB (4156776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02853a663b300cdcbfdbee7dbb15c142f5751d95622acbf369d1cf462a63385`  
		Last Modified: Mon, 26 Jul 2021 21:49:35 GMT  
		Size: 60.7 MB (60667196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
