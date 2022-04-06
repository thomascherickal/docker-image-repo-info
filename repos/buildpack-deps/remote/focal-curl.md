## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:99e813d82e61852857469fec483ecb440adf9ff1b9f27f91e04255a1bb9f7e9a
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
$ docker pull buildpack-deps@sha256:5bb3fb019d3127b971f95c47eedb2a90788787aa303393fff210a7a65e9ab5f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39957754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e8930a3ae6298664cf9ccdab269960d91a072139b288ad04514bb22af668c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 22:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:43:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63b9ea7f1faf2713b5c34cb3b777030b1aac36fdece5d6feb67104b3fb21471`  
		Last Modified: Tue, 05 Apr 2022 22:58:02 GMT  
		Size: 7.8 MB (7767403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8a48b746676433dc96aa2823b32c793393bcddbe79e001a99ac7fe19413df5`  
		Last Modified: Tue, 05 Apr 2022 22:58:02 GMT  
		Size: 3.6 MB (3624059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0a9e74f562566bbae813e390f524a29e49328fc9f736e88a0b8488e4c74d9349
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06ad2b3ca1b9500cfbafdf9a436de5ab50ad5e562f7d08d090033e4dad652b32`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:10:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:11:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568f7ebc955bbe4fae43748e4f7fc4f51dd5504de80f991c91780474f0807e8a`  
		Last Modified: Sat, 19 Mar 2022 03:43:05 GMT  
		Size: 6.8 MB (6762829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeebca37cabefaf4478ce7fa176a92849e8bf759754f1b2d7d08f09d3e3af8f`  
		Last Modified: Sat, 19 Mar 2022 03:43:02 GMT  
		Size: 3.1 MB (3103654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7137ca1f38f14966d9054358aaaad6dce6ecc7abd28d454a4ca44797cb98f769
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38189121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b950ea464cff10be1f1fe1a651d059ac8c8d1d1121f0dff9ce669b2da843d8b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:59 GMT
ADD file:113ba5e7bc74d50e8d35449f8a62712359e2f00146e03eee822c28c8c6f59368 in / 
# Tue, 05 Apr 2022 22:41:00 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:07:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:07:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d134b018f7f6073865eadeb6a35b1340bc689c734729c6a12a1e961e4fd95a1`  
		Last Modified: Tue, 05 Apr 2022 23:15:45 GMT  
		Size: 7.6 MB (7633565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7e92a0840764f8503d62db3c049dd856a3ce3291a628086c0d0be51f0e8a94`  
		Last Modified: Tue, 05 Apr 2022 23:15:44 GMT  
		Size: 3.4 MB (3386163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6f05d1fa157574a7123f33d43166734adbdb742a34fb8f0a4f510192d567ce86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46469499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c09816b6e83290706d3b1671cfd37f801491640591981b54694bcafbc7fedfa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:37 GMT
ADD file:c1af9c0e405f7eecbc87225c13709becfd46d66f87a4c5b8e30a1b82de7337e5 in / 
# Wed, 06 Apr 2022 03:35:41 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:83a2da48a82b52067676278a5eb4359bd7a79e7b57cabd370d77e11a9204121c`  
		Last Modified: Tue, 05 Apr 2022 13:16:22 GMT  
		Size: 33.3 MB (33291809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7036ffae6ea84710d34cff8b1ce6086d026dc91f309346b4893ed539b71cba3`  
		Last Modified: Wed, 06 Apr 2022 04:49:54 GMT  
		Size: 8.7 MB (8721734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845f237e4363d8e08836ac01b5dfda9138d75c2ef96b0a13177539dd798998c5`  
		Last Modified: Wed, 06 Apr 2022 04:49:53 GMT  
		Size: 4.5 MB (4455956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:d2716fdb6189f296bc88912b1b319600e0a86ae3b4c48ad695e79fddd2a1d955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34119408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f199d426b40edfad24c50d27099c6d6ffbed8f6b6b4ee642d6315c8f8f2f5a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 23:14:14 GMT
ADD file:2d2954ed28ad8bc069404a9d5f6d36f5ae810295e2973d6b5315e26ae191a7e7 in / 
# Tue, 05 Apr 2022 23:14:16 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:06:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:07:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9938df50ba0ad14890322376a86691bfa55a1921714e56aac56e9f297d6c0006`  
		Last Modified: Tue, 05 Apr 2022 13:17:06 GMT  
		Size: 24.2 MB (24228262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00db2becdffa3da2489f68925fed54da4d140e05554040353b7c4a112cbff3c6`  
		Last Modified: Wed, 06 Apr 2022 00:49:43 GMT  
		Size: 6.7 MB (6746426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720daeb98ebde10f93c0e7ff5a73190bf4a1ad493e82e952231a539f3a1e5bb8`  
		Last Modified: Wed, 06 Apr 2022 00:49:38 GMT  
		Size: 3.1 MB (3144720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d964d3d424ed0c654f891ad21cdbb0fc3b79a43ffab0d7047ff5cab44d361020
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38049247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8708d0937fdf5acc976bc5801633fef766b76e465007b3221fd6e8789314949`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:42:05 GMT
ADD file:44b5cfe67740a0d7e33d6aa2c83d9918fdb30a0649aa3471e2f668dec1ba7f3a in / 
# Tue, 05 Apr 2022 22:42:07 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:19:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:19:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:502c7975d4ed549ab7d6e63b9ea10b0d24c1c3c12a33540d91d6739a0218faec`  
		Last Modified: Tue, 05 Apr 2022 13:17:47 GMT  
		Size: 27.1 MB (27084913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77d5aa69c8b3c477d84d7f54eeb115c573bc2748cf9e73ecfdb20126141dc08`  
		Last Modified: Tue, 05 Apr 2022 23:27:40 GMT  
		Size: 7.4 MB (7422161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cbf31e9bcccbb04fe148a59c5fcb86a9ad6d51df836210815257590ccb0f78`  
		Last Modified: Tue, 05 Apr 2022 23:27:40 GMT  
		Size: 3.5 MB (3542173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
