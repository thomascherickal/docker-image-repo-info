## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:bfffe4a3acc134d001cdcf237d588a1e9caebafd5707bd0b9d392800a322b926
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:19dfc5e7628b593c8056b31cbe197a24fffbe1d35a9b17adfd2f59a34641a4d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72784332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07490f1b8ba2320e2026f3266933346b545ee1a5e75319a686e3575bac5b7f55`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:50 GMT
ADD file:1f62518cec36eb3320e38344c0d36779557214cfce8bc32eda000183a34a0ffa in / 
# Wed, 17 Nov 2021 02:21:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0fef5443775fe054990b02e8f72c4c5bc7792c6a5bf6ef8df110873a81676a87`  
		Last Modified: Wed, 17 Nov 2021 02:28:03 GMT  
		Size: 55.8 MB (55758091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63aa91be04004e56a4d31d70c789eadabfebe392e2f76a862eaa2fdd70dcfd`  
		Last Modified: Wed, 17 Nov 2021 03:25:48 GMT  
		Size: 5.3 MB (5269763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f625d605a0450d800b57ca6e2e0662fba5094348ccbf581c053a485802ebe1`  
		Last Modified: Wed, 17 Nov 2021 03:25:49 GMT  
		Size: 11.8 MB (11756478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:93a96196f940f2470a5f63e45ed1eea93d39f49454b3461ce4f86003f32e88b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68915524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0426cef40090f80992e6f69498065959d6e618dd140a8a21341a317c7ce7f274`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:67b214acbcd9f9a68874338a7751ff7c36fbfaf55bf4c8085992ae1d47249822
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66957300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a529394265f7fd2fbce68d31a42a78128feabb2a05da15f6db6613f9a9f76d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:49:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9096006210de2acfc2854bd14870e0046c7c41610d75f402e14c7fa186a10`  
		Last Modified: Wed, 17 Nov 2021 03:10:01 GMT  
		Size: 5.0 MB (5029921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864516b2a87655fdd355f203892d84f29fb0f553f371f37e7027ceb5017ec34`  
		Last Modified: Wed, 17 Nov 2021 03:10:03 GMT  
		Size: 11.1 MB (11067071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:739c39731b3c78675e5b07d31cfd783cbcaa98f52bcd3e90fcd44c9a307e6676
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71545945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03eacbbae2823342ae5c042212eaa4d8a7fd2b691788aca661c794de4be92dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:46 GMT
ADD file:6547698ce9c0dce5d390e739342bd015a0c3266dba4ef5828dc1b1a9eb46e826 in / 
# Wed, 17 Nov 2021 02:41:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:29:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:29:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:67eeb578521bba47ceed6d5c2de23409a33ec3c1c6fda03d83e22d74dc1cdb76`  
		Last Modified: Wed, 17 Nov 2021 02:49:53 GMT  
		Size: 54.8 MB (54767045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f777f34bfc0463ddee51fc9ba3a1f668f6072f8431123ab0571266c60fb89c`  
		Last Modified: Wed, 17 Nov 2021 13:38:51 GMT  
		Size: 5.3 MB (5253448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e720a8fffb7aadf0b926dc4c5b3d7cb21c21c6ec5e507ddcdb546f5483b5a44e`  
		Last Modified: Wed, 17 Nov 2021 13:38:52 GMT  
		Size: 11.5 MB (11525452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4dd56a29db23efb893ab16850832733df3813b7a11f292dee71fd5094fd58a3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73344320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:962d74b000a7400b45ea570dcd0f3351f2de7987db6d7cbd3225992e396a156d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7cb7cefc9fa6132910698c9133093c1f9b92416218f2ee05824d1bd3c04bf7af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71348254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c188c28686d73282c6cc150448e2c28b123c0faf48b12f0c6ba204562bd511d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:12:23 GMT
ADD file:9e3985f5064204cf4c74f2d464977349398f8e0325083d223b22ace99f5dfa3a in / 
# Wed, 17 Nov 2021 02:12:24 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:39:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b79f1dde26df3dbfdaf094cc43f4dc602b492e9dd707f7a7874e1366808028c5`  
		Last Modified: Wed, 17 Nov 2021 02:22:36 GMT  
		Size: 54.4 MB (54365459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c0e1963482abb9ea5592b86c11c6528aebf6fe675fd25fdeb440cd4f999043`  
		Last Modified: Wed, 17 Nov 2021 08:52:05 GMT  
		Size: 5.2 MB (5227764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0761e303fe4f33cd92c7d2d5ce49857285721fb135e5bf569abf4ec59745f3d`  
		Last Modified: Wed, 17 Nov 2021 08:52:07 GMT  
		Size: 11.8 MB (11755031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b66398bb06582e08079239ae0b55efcdaa4a6ce35f62aef40ad59f2066a751a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.1 MB (78127933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4909eb043acba9dfc8f6ced1c81d8f31d080bf218205bcff6428112c4bbfecd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:32:54 GMT
ADD file:33bc17dd3e3b6cd8c5ac37c8382a5d2b8e3ee8384b598b69b0d17b813dcfc767 in / 
# Wed, 17 Nov 2021 03:33:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:08:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:60fa303f933c621481dd7a32f72de0e35b85a3567ff116516725c45089e1cb88`  
		Last Modified: Wed, 17 Nov 2021 04:05:01 GMT  
		Size: 60.0 MB (60045015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a3dd48191daf1a5544d8a3146aececcefc7d4f8fe8e7e64e723022de0e5bae`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 5.5 MB (5531621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c14b8f9e107cd759a99e83c419ee5c8c99e500d16d4bbbfdb94cf6126b724`  
		Last Modified: Wed, 17 Nov 2021 08:31:39 GMT  
		Size: 12.6 MB (12551297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c56a5966672afb0d47c167ad7358e0979cd24aef6efa756a7d6814b137b647df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67743044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2ef8905089a0b83a3817c763b00709bc4c9c53504e843a8e09c10005a148e6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:14:24 GMT
ADD file:9ce8adafd95fc1e31db924edf473abf22a68101cad20cd078c35db5fa719b34b in / 
# Wed, 17 Nov 2021 02:14:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a35675c997377ee8bf94b0a94460a6d2fd72a26b5c7fc6194b13ae99da869125`  
		Last Modified: Wed, 17 Nov 2021 02:30:42 GMT  
		Size: 51.5 MB (51522304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6561ec3264f30875424c0937b41795ce70f58306ddfe766af2fcb7d266b6a6`  
		Last Modified: Wed, 17 Nov 2021 03:35:29 GMT  
		Size: 5.1 MB (5080232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f12be064689662dab642f65c8e821186c7247cf7ea84901a22b9e2584d51ee`  
		Last Modified: Wed, 17 Nov 2021 03:35:32 GMT  
		Size: 11.1 MB (11140508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:40088f08cf065fbc90807be108a7a28a69ba5cf9a42b702be39a8c7e51925ab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70861043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27d0591464195b772d890535dec1c22fe3a85b97d9aff1dbb6f656574b113c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:11:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:12:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634664d8b893813a04761069646d85aea7164717481b8c7e3f500e4260fc39ee`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 5.2 MB (5248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1780c6b7bcc6484f6ae6602c37ffd3bb2c9aad27b1b2587b796a5824e8b6575`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 11.6 MB (11647079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
