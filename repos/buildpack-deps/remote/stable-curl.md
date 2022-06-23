## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:ec54895ea1b329fb19adf11900cc352a847287cfc17ec033c0fd5e05293c88e2
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

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b1f53efae2fc2c06d8cc76e1c6b14a3783ad25bd0caff4eb358b05d779c3bec6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (71040934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6844d768ac9d1b8f3ab72cb8e439b809f062b812e094ca561b258c99912f8405`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:16 GMT
ADD file:798015650079cb88614ff181a30f9c3d3fde8361c49ae2dec2058d5a3e61f5df in / 
# Thu, 23 Jun 2022 00:20:16 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:50:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1339eaac5b67d16d6d9f41fb7a7b96f7cebf3ba4beab36cbb60935aa772af583`  
		Last Modified: Thu, 23 Jun 2022 00:24:48 GMT  
		Size: 55.0 MB (55009886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c78fa1b97999d08408734a61040475ade5bd7e33e91c0d5170dba2c7c7a92fd`  
		Last Modified: Thu, 23 Jun 2022 00:58:38 GMT  
		Size: 5.2 MB (5155961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f0d2bd524377dc42d072443c0e5e7cafa14f5df609d39bb1f717f43817a2cd`  
		Last Modified: Thu, 23 Jun 2022 00:58:38 GMT  
		Size: 10.9 MB (10875087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2fc7e68f6526491ff28922bbae0df251f2218adf2bcec65c70c73b699e3fef17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68179605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9a29bd7cee7b7953bbd00d6efcd4151d1090dbbe955154a0fefee6fbb6e26f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:04 GMT
ADD file:a9a29412ef2a46df9ac08c0263e1fd3872777bcafdf6f172dae904af96ff7585 in / 
# Thu, 23 Jun 2022 00:50:04 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:37:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e4031f48ff7c3b7223afff91721ded4a4de5f7c666f84c58a5d8298dd0fe028`  
		Last Modified: Thu, 23 Jun 2022 01:04:50 GMT  
		Size: 52.5 MB (52541138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81d328795b20b164711abd9d265ebf98fa864c36cc2ac7b79fcde10ea683a47`  
		Last Modified: Thu, 23 Jun 2022 02:01:21 GMT  
		Size: 5.1 MB (5065402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df15bbc2ab79e81b31649e3d85b8e92141abf53487afd2e2dac38a9889b4d3`  
		Last Modified: Thu, 23 Jun 2022 02:01:23 GMT  
		Size: 10.6 MB (10573065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f1426c0e5ee7ac79454e6ad0000e0bc85e04176b15c5da1963a3a5f247452120
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65342414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96020d90ee0e3f6fe0427ce7ef73e0ef2848f919c6672deeb6546c66f03b840c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:08 GMT
ADD file:59a6186285c4849971ea2d4801e6ebc1e4310f5e3dc0f87389f39d1fa8a63c58 in / 
# Thu, 23 Jun 2022 00:59:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:46:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:46:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2147df557f50051066d8920b460727b890c1da5cb2c15b055c99ed8216b5528f`  
		Last Modified: Thu, 23 Jun 2022 01:14:34 GMT  
		Size: 50.2 MB (50199604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b28303e18c4d3b1788071e1a67ed51ad28c9574bf30371176fc152638acdbe`  
		Last Modified: Thu, 23 Jun 2022 02:13:15 GMT  
		Size: 4.9 MB (4924846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536c76bf1b84e75e4834c8b50a6f3697460303c4b2021434891103b94ca78fac`  
		Last Modified: Thu, 23 Jun 2022 02:13:17 GMT  
		Size: 10.2 MB (10217964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6c02bf8a8f9584356dc60af379136e028a31d12e47de415a13139d266a5d378e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69292545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849803a2868f0e5e7695d05b765972029faaaa49d0f6f08c3e2e3b2a4bd8c544`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:28 GMT
ADD file:64c455af1bb18ff2c202a244e058b6e5ac147b89410ed36edc5e29f4b6f02c5d in / 
# Thu, 23 Jun 2022 00:40:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:11:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:11:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f873dfbc59b181817d5bc2b9fc31d90d8f9139c8cabb2fa7264f9bd7b418b8d2`  
		Last Modified: Thu, 23 Jun 2022 00:46:51 GMT  
		Size: 53.7 MB (53696815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7b65e0e9cdc28c8cedaabbc5cbae4652c9b107c47684de49f01a77741a5ded`  
		Last Modified: Thu, 23 Jun 2022 01:21:51 GMT  
		Size: 4.9 MB (4938760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43836e7983cba8b758620a218a0ee622daf5513308b6a9e8316f94c271ecafd`  
		Last Modified: Thu, 23 Jun 2022 01:21:51 GMT  
		Size: 10.7 MB (10656970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f9fd3319661a28c9f5cfb55f025aac1154a804d4a9806cc0d31a9dc5a32202a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72121708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56261466c6beebb3aa7a4ea7bd99f25eedce2a64257b7e485c876f92d4b7cac7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:17 GMT
ADD file:38ad8e7562f238cf436c2a32b21b397a0ad3dd5c8f68f29bc724458cad18a47e in / 
# Thu, 23 Jun 2022 00:39:18 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:11:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:11:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8bfd9a7ec075cef3ff84a270710c704347f9a866aeb50e5a286491696168d5f5`  
		Last Modified: Thu, 23 Jun 2022 00:46:04 GMT  
		Size: 56.0 MB (56007522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45f3c7c07e8e6bb9d2c30f8b932d9db0300b97850bfbf921a5b56ebefa99769`  
		Last Modified: Thu, 23 Jun 2022 01:22:14 GMT  
		Size: 5.1 MB (5080447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f01d925e37f51b5dbeac306dc641b52957d383e5fd3d61dc8822590b97d171`  
		Last Modified: Thu, 23 Jun 2022 01:22:15 GMT  
		Size: 11.0 MB (11033739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:298b9ce5e35c81a30caabd8df541d3a948bfb94c8938ad63637b7d8e4f08e8a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68845892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf833385ab93c45bffaff4137667bdc626821e2da87892f07557ccd8027250e2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:09:48 GMT
ADD file:b4c1f4f21cc3a6a3ebc27c9c15cfab9e67c385c2df87110392754663c02722f8 in / 
# Thu, 23 Jun 2022 01:09:53 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:52:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:53:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5a63618d87cd80f12f8640fecf6d13ece7ce3ac6260be88adcebe60f4da899b8`  
		Last Modified: Thu, 23 Jun 2022 01:19:34 GMT  
		Size: 53.3 MB (53273237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac43be31041e2631cd8bdabfb3934fb423e7237e142c5b86e532e192e4fe36`  
		Last Modified: Thu, 23 Jun 2022 02:19:58 GMT  
		Size: 4.9 MB (4912505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfda9893d218bf2decc23f236eb8276f1b5512b4d2647fbab36c43e9bbf96d3`  
		Last Modified: Thu, 23 Jun 2022 02:20:00 GMT  
		Size: 10.7 MB (10660150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f90fe89270e1bcaa6ff7b8554b3ebb1ac7a33c846940906a2563e4c28ad08605
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75935836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f4b2687ef815638d930c08a6e2f666b1936dd4f40633d6a6d9d01e54ad03970`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 02:01:53 GMT
ADD file:8e4c382536553538abd5a62333996023e484596173131dab18020775b0731238 in / 
# Thu, 23 Jun 2022 02:01:58 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:03691a2d4065f9ca4fafadaa8229407224c6aac10796fc0884981e6c81a43b8d`  
		Last Modified: Thu, 23 Jun 2022 02:14:21 GMT  
		Size: 58.9 MB (58903151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a26b659a43f0973605ce681b0a27a9563e32a560c64518a32cbf9284ffbe8bf`  
		Last Modified: Thu, 23 Jun 2022 04:56:06 GMT  
		Size: 5.4 MB (5405243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d46f40a862767538cfa58e9d25dca4b07caa0e31992187e566a6c24b0e11f0`  
		Last Modified: Thu, 23 Jun 2022 04:56:07 GMT  
		Size: 11.6 MB (11627442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a133548c83df64d7888265843c7044c96fe44eabb17be906b9ef9e74c2747651
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69183192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c8e45e6d232703bd7d915270bceade47ab7e6caa4c4e483ddcf2098d6f7f31`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:40 GMT
ADD file:80a08f446549ae1b71aaab0aada00625b804fd959e2a21a9c0747fb3cdb0afc0 in / 
# Thu, 23 Jun 2022 00:42:48 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:16:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:16:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e92226c94dce8ebeb505bbbebdc70207295a4a602fc736044e4e69866dc05e58`  
		Last Modified: Thu, 23 Jun 2022 00:51:36 GMT  
		Size: 53.3 MB (53276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d640cc8936c5cb6e3d305ec831be1b35a79839e07490358519cd2f48759274a`  
		Last Modified: Thu, 23 Jun 2022 01:35:00 GMT  
		Size: 5.1 MB (5140923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356e72745d061d1b1515a417d346c741fdcf0e3c58b6aa88cc86eee96ec3daac`  
		Last Modified: Thu, 23 Jun 2022 01:35:01 GMT  
		Size: 10.8 MB (10765497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
