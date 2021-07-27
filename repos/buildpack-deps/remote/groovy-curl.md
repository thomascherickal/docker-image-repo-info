## `buildpack-deps:groovy-curl`

```console
$ docker pull buildpack-deps@sha256:64c19d1328bbd2a71724d8a1d825cbf400bc36474ad8eb2c3498bf4c0875a6c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:groovy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5d9333cc1ff3e13e012c194669faeb66271a68fc77b1a7684743d349ba539a31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40412052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3417e27ef3c763508ca0d64e45a7c5baa890eeee4e40e29e4ca8130cde2ecf17`
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

### `buildpack-deps:groovy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7536ccc1f755d8778266098ea95e4d657b401a554760debed405369e1c5ac3a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34293734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0601093a516c81d72db6edc44b40ba9ae8de46ed66ea5f297250ae4ef34b9bf4`
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

### `buildpack-deps:groovy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ae75cc271177b9d88708d7ae300982b5d9405f90f3efaf7a863626cffdd931e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 MB (38883597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34611324abf91520d4dbae4ce9a0a555011e5b3a1fe2f364b796cd24031d431`
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

### `buildpack-deps:groovy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d783add69d2804fe48bd463685ef867ddf1092dae7a72b456fbf651c912f286c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47125494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1786ea2c6d7caab11adaf79a4e4339f0da55a88538c8237b8838f61a885d8d85`
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

### `buildpack-deps:groovy-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:94465280ddfaa460b244d5cb7d8a3717979b2688414e684825240ab3d110c6bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34626072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f326ce387986bbb179c0caf30c0aa8c5346585bf9f45cbf54d6ab688e68f3320`
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

### `buildpack-deps:groovy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b8416a87b1796c7c9436490e394d83bedd8f5740600c219f6cfe9b441fe02a6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41364851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:824b28c19ce76bf1edf7c98803170358350e35efd22a8a1d63b77ef1ac04ef3b`
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
