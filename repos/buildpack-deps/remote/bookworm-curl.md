## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:51d9de5b60517f7dbbcdee6096bdae6da3767862fed8ab6a5fe21be2117e4a3e
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

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7f672cb94a21b691b5622eceee7146ff9d63c09cf9b9a615468cda4982bce031
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73586402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52a3576a74b27fbdc9ee30a6d3bcd8a47de0d620783f4f3237a349f712bf5f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:34 GMT
ADD file:e413c7d61ecdc96ab067e1f8bff6ce03c792c94b9d1f54e80cf633052c5d975a in / 
# Tue, 12 Jul 2022 01:19:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:46:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:46:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7c7a32fcf1e30b18b7a9a032acf892763291bef7159859a35297bf81217bbee4`  
		Last Modified: Tue, 12 Jul 2022 01:23:29 GMT  
		Size: 53.0 MB (53022393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00146b6ba9670f0b5362fb1ea6716d934ae0d1545d85efb6e7d9871f449ed7f`  
		Last Modified: Tue, 12 Jul 2022 02:53:57 GMT  
		Size: 9.3 MB (9292245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed5201b04ed0ec80bf5f970e6e10f4e241d58bfbeff69ec15faa4c6a34f01b6`  
		Last Modified: Tue, 12 Jul 2022 02:53:57 GMT  
		Size: 11.3 MB (11271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e102c8175db9e940a2f314c870c4ad9721d38bcb78562236ec5b0f46f690f0d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70487955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5990cd30edcf6798ed6dad6deccd86ce57b88a9316da67967ce35a05272fbf76`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:48:59 GMT
ADD file:211648cfc211d73b6facf8b4f6762e1b45f5894d43880d7bf0a7822be746ad58 in / 
# Tue, 12 Jul 2022 00:49:00 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:33:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:34:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e06063f979dbe8242191c248c95f1840e27b65404e59a60f54bfc1575fabed87`  
		Last Modified: Tue, 12 Jul 2022 01:00:53 GMT  
		Size: 50.8 MB (50821602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc41e44fbad79261bf0a50b7500c64ccd7e7f8b3209de9bb0165c595e95914f3`  
		Last Modified: Tue, 12 Jul 2022 01:54:32 GMT  
		Size: 8.7 MB (8725587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac530a424b46c790de63a633c7ffebf87465fa20a427e8389d6bcaf6ae81028a`  
		Last Modified: Tue, 12 Jul 2022 01:54:33 GMT  
		Size: 10.9 MB (10940766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:118cafd918a67b200ccd76ad2e1e398bcf62cd852f37b0da5a931bb157cd5640
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67554066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f06c5e8eeb995e91091f27855327aa695c5a175ce712579ee3ad2d10c8f44de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:58:11 GMT
ADD file:5e1c66e0b3334d725bfb0c7f0d2772c9781b78f01d54756b1924de7abe4abea1 in / 
# Tue, 12 Jul 2022 00:58:12 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:24:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:eb8579179b8f8463b05b790bf1566472700d70b08d50d0c6cbc776da788afbb7`  
		Last Modified: Tue, 12 Jul 2022 01:10:35 GMT  
		Size: 48.6 MB (48562934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5ec0a68470d880c05a2e75012ae47d36f57e8e96f491c963000d36a5bd0125`  
		Last Modified: Tue, 12 Jul 2022 03:47:36 GMT  
		Size: 8.4 MB (8405468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b47847e9c4da9d8e5006ac7d60da76d9bf81a4a5b77c355988cbc11285cdbff`  
		Last Modified: Tue, 12 Jul 2022 03:47:35 GMT  
		Size: 10.6 MB (10585664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:76765d24e1a88b8ea01779c253df01b952c3eb7da98866bd3d3be38685b56b0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72319163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e101ec5fbde3de51bfdb7fcc486ce8cae1ffe0f7f97054c5a852a43c11c83d3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:53 GMT
ADD file:56a82a6c91d29741aef57453822e5502a13bd7841a1b3c8936a6f7b5c0b80bb6 in / 
# Tue, 12 Jul 2022 00:39:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:31:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:31:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:73d3feb17dc47282a9451cf8832ac9c5a707630877cc6c832d9f5cf4d3e2d202`  
		Last Modified: Tue, 12 Jul 2022 00:45:00 GMT  
		Size: 52.1 MB (52128620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3f77295745c94527eef3df84e5f089d7404a40e8f243f00fb8ede9cd04cda4`  
		Last Modified: Tue, 12 Jul 2022 02:41:22 GMT  
		Size: 9.1 MB (9132573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22eb759abcb3de672cf64ccea22ebac1e035560b83ba8bbbd82b3c274ccbbf9e`  
		Last Modified: Tue, 12 Jul 2022 02:41:22 GMT  
		Size: 11.1 MB (11057970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6970bdc1ab100b6801de5c99f4eee88a0b4085665fdbd3e8fbf7777c3e6931b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74939557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5674817a9f71a508f198e6d2f1e0cb5bf9e859e47a78bea7595430d239db2402`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:38:44 GMT
ADD file:80ec0e35d6a4c162afe79f40617b47f846a2eb2065f245a230447609d1e7c001 in / 
# Tue, 12 Jul 2022 00:38:45 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:24:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:24:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ec7f9e3ed305349e742c012dcd142cce637ef3525759fea18f30c5987bf0e2fe`  
		Last Modified: Tue, 12 Jul 2022 00:44:03 GMT  
		Size: 54.0 MB (54004076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4070b35288ac278d35017570259c20c0599ff1459ee03a4492a44fedae6c68f2`  
		Last Modified: Tue, 12 Jul 2022 04:34:48 GMT  
		Size: 9.5 MB (9465776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001cac3991e538096035178065ed3abbfbbd6211f5e8284e24b2095d4e30a6a8`  
		Last Modified: Tue, 12 Jul 2022 04:34:48 GMT  
		Size: 11.5 MB (11469705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2be0993a0496e36806a4e7bf59363cfc6dacfb5c75bc8486937ad4ff0b1adcf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71839292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a166fee9b8076060744a2572524576fb2ec6b80006c078d83b56c39a45652e3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:39:09 GMT
ADD file:a4c1c80b05ba336cf2c87e4c90f5bd31ad9a6952b41985b49461741377bdf82f in / 
# Tue, 12 Jul 2022 04:39:13 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:59:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 06:00:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d42ff6e50c127c0849c96192832cf954071e1fe597bc69ae0894999838a3d95b`  
		Last Modified: Tue, 12 Jul 2022 04:49:46 GMT  
		Size: 52.1 MB (52148304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6761aa7c460392eac1c72e9e3d658302ae105a69f107d6b7fb8bce7f988b5b`  
		Last Modified: Tue, 12 Jul 2022 06:37:09 GMT  
		Size: 8.7 MB (8657917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6e4ee7231527a7e9598fb19bb5b34e13789124eaff6a2955f130d363356fb1`  
		Last Modified: Tue, 12 Jul 2022 06:37:09 GMT  
		Size: 11.0 MB (11033071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e6f20ff891bd42d4e3bda4d761fdfd188f7006bb154a6b6ac5fe7801a7ce7e2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79223335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0180dc35d74cfa8015f2768034c9fbda6385836b3d638745beeab0b8563a25a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:24:07 GMT
ADD file:ae1b00e1c53ca0bbd56262f1d2cd742362c7a02eed6214e944b4b4762dda64ff in / 
# Tue, 12 Jul 2022 01:24:11 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:27:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:28:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8000c6ba1eb02ffb5f03a6b7e7d8f71a864844286f05cb8516ff71014b1cb870`  
		Last Modified: Tue, 12 Jul 2022 01:33:34 GMT  
		Size: 57.2 MB (57237580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40aa4d5388d97e0872477cb7660fbd3c341738064717f187dcfc90f0b64e8e89`  
		Last Modified: Tue, 26 Jul 2022 23:45:55 GMT  
		Size: 9.9 MB (9902776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05727228be0751bdf9f161f49f4edda690903161ccbf1593b8a4a16062ad8ce7`  
		Last Modified: Tue, 26 Jul 2022 23:45:54 GMT  
		Size: 12.1 MB (12082979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:23d7545e6602fe8443607b9d32a9b3a9decc2f89a0af1239732d5fd1ed391b71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71655983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9359b5dead00a52de8c2035125d1623990f3c10c2b0cff55e4da228ab68b7c49`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:42:21 GMT
ADD file:affba659885c7b0f365e0fe6df963322452d3a11e8c5d1f1d1908cadb57c33eb in / 
# Tue, 12 Jul 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:35:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:35:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4819cb6cd77746b912d22ae402922254d55d38be97967a6c3851624256c8a8cb`  
		Last Modified: Tue, 12 Jul 2022 00:52:08 GMT  
		Size: 51.6 MB (51554170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167df8c8442dcbc38170fd2782ed9a5c4e450b990c5d3f5bc8f1e960393fe12b`  
		Last Modified: Tue, 12 Jul 2022 02:52:43 GMT  
		Size: 8.9 MB (8939224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca0453a18e7c0e72daadbe03c9a6c56fb34dc6db87af258b576918425f6bbef`  
		Last Modified: Tue, 12 Jul 2022 02:52:44 GMT  
		Size: 11.2 MB (11162589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
