## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:e23404f8cbe41fd6bb2218612db23f4601dcd32869e4e934d281929647f60765
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
$ docker pull buildpack-deps@sha256:8ad7989339bd5853dee1b4694129b35e8f3da4f9bd367566525e02f4bc25430c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39961907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c7b26ba20fb907bc6e40ebdec0384394f1a12802265f68c178e8f2919a646a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:45:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844d0dd6bf6aa5959f603bad64a331fca5cda171d344450ca89c77e67410ac3`  
		Last Modified: Mon, 26 Jul 2021 22:11:07 GMT  
		Size: 7.8 MB (7769926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e2a2dd7363ebee0e3b7e3d44204409298c305ea2a5f38345f68c7b769033b`  
		Last Modified: Mon, 26 Jul 2021 22:11:06 GMT  
		Size: 3.6 MB (3624037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4d6589f264d3d82306ab179d8ff852a670346027a7b62190c0babd4b8d34a958
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33935044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02443af7132a39831ae2d9b9d585c88205154e162e5bbf922e0c3084d7be59d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:18:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0761e0b1ad0205162c66dfa83bf91ca0344921eca2bdd1d64b0970a5c75f0c`  
		Last Modified: Tue, 27 Jul 2021 01:42:27 GMT  
		Size: 6.8 MB (6767075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c226da21dd821a4b4f19689b2131f6e34d29095f42b4046f2eb48cf954e0076`  
		Last Modified: Tue, 27 Jul 2021 01:42:24 GMT  
		Size: 3.1 MB (3103731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:21951dca961bd55892f50418da8d401ceed45758d655dc4824ef3fd148427526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38404978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f04a573f3594b717d52f143bee6767d2e0c6fa4ea8a2c8a309c84a6a1104ec74`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:29:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0bcd6c59f771794bb0723fe6b8c1c0e51e9c469cdb93041dcdc9f49d27d7be`  
		Last Modified: Mon, 26 Jul 2021 22:40:18 GMT  
		Size: 7.6 MB (7634457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1740c38141581c96965e8f1d5d11782dd201bcd16881ecdfae0fa9b6054f6639`  
		Last Modified: Mon, 26 Jul 2021 22:40:18 GMT  
		Size: 3.6 MB (3600266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3343815e10509d9648012c05f2e752a78831d17deb67a5fe6254365c7e3f1318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46466428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06961955e80c37898130cd6fc301e88e67a0eb63504745d38e5c747da68756a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:22:24 GMT
ADD file:cdca4c00902f291c6bc305420b891f5149b6833b5f9892232ea690d38adfff3f in / 
# Tue, 13 Jul 2021 23:22:32 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:157ef43c951ca9b65226089aef70b09df64b81636884260390a329c24a3c614b`  
		Last Modified: Tue, 13 Jul 2021 23:27:34 GMT  
		Size: 33.3 MB (33287846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa601d6a2e5b36d987c4fdb079f47adcb54e845f31bdf1e5e9ee48ab4ba4990`  
		Last Modified: Wed, 14 Jul 2021 03:19:13 GMT  
		Size: 8.7 MB (8721735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60512369c33b9f7b7eafd481b6703a8a71a0fd9d9e71aea740ea72bdb8f45529`  
		Last Modified: Wed, 14 Jul 2021 03:19:03 GMT  
		Size: 4.5 MB (4456847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:5a800205d481ebe6cf41d9ee845aaf4cafa356fbe7f7a39a307227a455ac5384
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34119810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523a013d50d70e6e8c523060e1592fa9fc10356c500613a9aa1e1edc7b173e97`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:20:57 GMT
ADD file:d370c95489db85c7c58c7970cc48bc628ce77c17f20cb1e4528de52872dea8d4 in / 
# Mon, 26 Jul 2021 23:20:58 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:57:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:57:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c5d79ba950300edac11d7183946840d5d8c25cc00f5806730a2215d957c7e372`  
		Last Modified: Mon, 26 Jul 2021 23:39:44 GMT  
		Size: 24.2 MB (24227867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b262e67f3091f6263b382a9172da3c574e3bcec0e43f4e3253e1cd06825dc81b`  
		Last Modified: Tue, 27 Jul 2021 00:59:59 GMT  
		Size: 6.7 MB (6747598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373cb1f270a6b4c0bf67e88c81fec3cb58e1d6b1dbe3f8aaebe21802b0f59bc3`  
		Last Modified: Tue, 27 Jul 2021 00:59:54 GMT  
		Size: 3.1 MB (3144345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b500f583083410bb3795832f191e4ac67ed611f99cc09f5722d34193e8fffbe1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38121214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8bd4713594e6350bb021b0877a086198d7e2ce48a24d0cc6496a927d80ade7`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 20:55:12 GMT
ADD file:b8731edfdacfade2ec96757342f216962f3971b24077a9144da3f80003e6893e in / 
# Mon, 26 Jul 2021 20:55:14 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:40:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:40:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:38800a0044dea146ca3c3a08bc2c9c956396ad3241a3c343010775650298c379`  
		Last Modified: Mon, 26 Jul 2021 20:57:03 GMT  
		Size: 27.1 MB (27149898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2888a21c9447e296644db94b75a0ebcedbffbfe4771d5361146fa064756319`  
		Last Modified: Mon, 26 Jul 2021 21:48:28 GMT  
		Size: 7.4 MB (7429218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fec118c5a61478d525b2e93c72b9c0d221eba35013d951988beb556e65179e`  
		Last Modified: Mon, 26 Jul 2021 21:48:27 GMT  
		Size: 3.5 MB (3542098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
