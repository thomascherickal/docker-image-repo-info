## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:ee0d35c92364bd4c1e41b08df07391d829622d27d1c6d3d95e6af0a7a997f49d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:focal-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d29c5bd69a9b105a9d66188a0567111d14c2d5d67a9d3b55f8bfe3f94ce2bbec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39957585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:515719c9cdc2c94aabf96942970ba9a2ebb15d8c1d70a8124838414910a36dd4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:30:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:30:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722543eba393b6f25a2387b7f7fb5f0247f569506480360827733f1c7eacc0e7`  
		Last Modified: Fri, 22 Apr 2022 01:44:40 GMT  
		Size: 7.8 MB (7767495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09dd9938f985bb6f9e7b84a36bf26a8f5b9a6ce8d302df592a4dec2f5cc9a6d2`  
		Last Modified: Fri, 22 Apr 2022 01:44:39 GMT  
		Size: 3.6 MB (3624092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3032a085ba6439cab3cdefc156bbc5144000fb0f1b643f95617f2244e0f1e2c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33940307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a66ffbe99c3d4c0620a2a0e43544b71757a5abb1e104a7292f9fdbb16f0c46c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:37:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:38:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e00f37da1cee1efe8f3ed0a439fe489465bc7513311aa2ca3170bbc560cd4e5`  
		Last Modified: Sat, 23 Apr 2022 01:56:38 GMT  
		Size: 6.8 MB (6762032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64c80b52697a36bb40c76df32329cd361aaa2a3845b3a09ac751be3d3d9f518`  
		Last Modified: Sat, 23 Apr 2022 01:56:36 GMT  
		Size: 3.1 MB (3104206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:51c3756a806ec70f5d1be9120a449c6b9e5d090f4b619b52b3abb238a25798d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38189464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:971dc8266e1730b12c047ba9e7779fd3ac1b5eb395a87b4b6b1e5078f818ef2c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:31:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fe2982ff8180e5b5c372c1f072dc9096e3aed337880012ec8898e140f2dc2`  
		Last Modified: Fri, 22 Apr 2022 04:40:00 GMT  
		Size: 7.6 MB (7633835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a5ae54463f481880df42328a0f1c57de3dd2da4998178d5094bb9227bf907d`  
		Last Modified: Fri, 22 Apr 2022 04:40:00 GMT  
		Size: 3.4 MB (3386488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:02202f4e038a37e76c6125e3bf5244104f3aa9a0d3c249f4a810f89498e13768
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46468215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bff8e6ebea2a2c556cb678b10daa660b532ad3afccb2810640adf9f9c790dfd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:16:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:16:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201e69fef602ecd9c604dbc526e412a7f9f53da3d9073dcf9b13e90174bdc39e`  
		Last Modified: Fri, 22 Apr 2022 09:41:50 GMT  
		Size: 8.7 MB (8721811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2269d321fbb9bc5909b0f64e4bd17d6910613bd979b25648123ea6ada12e8fcc`  
		Last Modified: Fri, 22 Apr 2022 09:41:49 GMT  
		Size: 4.5 MB (4456029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:572f3d04e424d4ad8b57fd84ef81c99826c91e02a9283662820b5fe9d1d07921
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34119219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd1113cb0f69a6e4623e1744d72a498740be45ebdde82870af09f9ee6fc8ff58`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:14:32 GMT
ADD file:da9b6ecab27e35ebae8f492705795f99e0f2cc85731b5df9d5d3219de9931283 in / 
# Thu, 21 Apr 2022 23:14:34 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 00:07:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:07:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b8029d8dece6b7c2484f3de2deabcc27fb90a113378736b4dc2177c2d0f2aaf9`  
		Last Modified: Tue, 19 Apr 2022 13:15:55 GMT  
		Size: 24.2 MB (24228118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b4e672c9f8fe26957fdb418ac8a515a3cadb41d7d287e5b23ef72bd3450440`  
		Last Modified: Fri, 22 Apr 2022 00:50:34 GMT  
		Size: 6.7 MB (6746409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0c9187320e6be3859e97d2c6516161a9bdc3abacc5d6d4f071ee6f14ce535f`  
		Last Modified: Fri, 22 Apr 2022 00:50:30 GMT  
		Size: 3.1 MB (3144692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:894a080bd03aa5cc7b7ac72b5b1a7f4fb5cfd7a371c9c938eb846e15fe93d3d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38050585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c8e2b26c18d3d39f693acca5d34d54a0394c2847b60db618a4649f86975b1d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:34:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7951284cb68b6a00917429e8710567f9cf59ec824346159a9713e70fd897f937`  
		Last Modified: Fri, 22 Apr 2022 01:51:30 GMT  
		Size: 7.4 MB (7422499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908eb104679df5b72b639e9dae6c144a0e2c32ef5438c9f65a897d136539dce8`  
		Last Modified: Fri, 22 Apr 2022 01:51:29 GMT  
		Size: 3.5 MB (3542368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
