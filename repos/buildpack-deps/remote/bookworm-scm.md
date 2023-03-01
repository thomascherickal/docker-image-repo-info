## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:6010adfdd68330d5cc75103f4204b81cbd0975c60b82d835e0bf7660febf6864
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

### `buildpack-deps:bookworm-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7672703ae082615e986385b91c9fa35429dde626233955b38d57cd672e8220e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133786861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da1325778cc479069b68fd4bbf41083893a5ce9810f4735b36ddb24809bbcdcd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:21 GMT
ADD file:74b4e0fbcb9cb38344c32a0512a72d8179f885de4b7bb127215f8d96a6262664 in / 
# Wed, 01 Mar 2023 04:09:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:40:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d915a4248d2913bb8451eba978ac348a983990eca9186543367f5f44900e0fb`  
		Last Modified: Wed, 01 Mar 2023 04:13:25 GMT  
		Size: 49.2 MB (49237273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012774ea2ca6d41295cf7bc05a82ac4aa9183dd2ce4f4c0584b549d922ef6b2e`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 9.0 MB (9049510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871c0f2b6b6518e6675004eb4ccd8a8d77105f4f1d83d8f0d0168b16f544ffbe`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 11.4 MB (11405791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df7f0c3bf5351a2fa63ae6776d5565929b9afb539c689cadd1e415b1751f478`  
		Last Modified: Wed, 01 Mar 2023 04:49:31 GMT  
		Size: 64.1 MB (64094287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e368a980ce07d0d05c407f5f83fd7eaa214a94ab89a68fd65bcc72113d126c75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129141721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f1ccaedc02174ef64b93a8f0f326ec4ffec1458f1c54768a5da3d2e53c616d2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:24 GMT
ADD file:1685939a153ab7a7aa03035565c60e99663abd3a416ef0d00bddaf24e0ae6f08 in / 
# Wed, 01 Mar 2023 01:48:25 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:15:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7516928cdf57280d137bb31220dd9f0b6ca54e290189b42a68ab64d0d2065b7`  
		Last Modified: Wed, 01 Mar 2023 01:51:43 GMT  
		Size: 48.1 MB (48072838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402a03a1c745fc42a93ed0082abf13d52e0c961da496b7b2d7d9a60a1d8031f`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 8.5 MB (8496389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1f01cbcb26c4e22bf2c443b3515e57d9267d84661daeb7ae809ff62ff82`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 11.1 MB (11051495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db38c030ddb0562da5b6a4ed2e4333299c295c785959c19faae6aecfee04f841`  
		Last Modified: Wed, 01 Mar 2023 02:24:07 GMT  
		Size: 61.5 MB (61520999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9363999a5ced7319bb4e8233919bcf696a5ff06ce055f6ff25cddc125630fe82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123900581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14baa6809f04057f886b38600982f1e5bbe9c414e11e8a016f729d70ff9ded84`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:26 GMT
ADD file:9f8ce83cf3e75c63cb351ec688378ffe29d7105ff8e8892b3cef95aeacbf6779 in / 
# Wed, 01 Mar 2023 01:57:27 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:28:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:29:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c5d14f15cd67359c9f8d5dbc636ce6ffee972aa4acbeb663e40e865b0dd7dee`  
		Last Modified: Wed, 01 Mar 2023 02:01:54 GMT  
		Size: 45.8 MB (45843301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925df4d36e5e8049cacb403582ac8832aed842417020be560ab0398e08c8fb67`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 8.1 MB (8140837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5921afe59294ea6e26c9a0c8c143bce276da4ba83ef2f7194b96d034a2b463d`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 10.7 MB (10687660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daffa30bd41618c0f8d8bc932ac6b2e541af6a12c3462963570690c046fb0eb`  
		Last Modified: Wed, 01 Mar 2023 03:08:25 GMT  
		Size: 59.2 MB (59228783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:707d81e8f30e61d9f2aaa457f83a07eae8b2a592a62b58d3d7e9d83da5975f8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133469946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f6c7e35dd573abe7c4284cb4996d045b058236c5962edd7424453357d4c3c5a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:13 GMT
ADD file:5b81699b80066f9e3bc967bdf130a67f54ebe15cd80df6c952262d6132b1cabf in / 
# Wed, 01 Mar 2023 02:20:14 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:46:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:47:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf639a903cc04a00c81ac77b3b9f9a79644c51b7f515895fd60403c20ff34a80`  
		Last Modified: Wed, 01 Mar 2023 02:23:22 GMT  
		Size: 49.3 MB (49273990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42632d5ac93ac504d393018f5e0f56f02bedd9cd2df6e1d91da9fc0ef4806d9b`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 8.9 MB (8882130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c0a0685e10806d6ca5aac08337a76d9fd6a47f16f665f5d3a2e692eabfeb3f`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 11.4 MB (11371530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1ccc2a9c1e986768a01b08e1009a75262c8bac308f9c9d414685034ce162c1`  
		Last Modified: Wed, 01 Mar 2023 02:55:40 GMT  
		Size: 63.9 MB (63942296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ae8e961a9e40fd1cc67a16b2eeb562541342ae4bdaa1e6a49ac66fb1484f8e96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137251175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c2068c6e1d78739e77ceabcc05f5cb988caed03f0c045bd5c99279abfe372a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:38:40 GMT
ADD file:0ccdbb7b1f104c23abcf77c506eed771d5759d210c2284a95f85e558405a5390 in / 
# Wed, 01 Mar 2023 01:38:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:05:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:05:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b5ba6d7d02dd42cc6291ae5b4e129956756f664662a78db71f320107a1b6d189`  
		Last Modified: Wed, 01 Mar 2023 01:43:30 GMT  
		Size: 50.3 MB (50273396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f35c12f0528f81569a1c99e040f4d3527ee4391aa4079d740a4c6638bcece0`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 9.2 MB (9230996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f35836381f914f3bbf4d55b955e9cf90a83165b64e829c72b52051b5e5c5`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 11.8 MB (11808790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a8ff813204e629160f019ffdb45960b87b39f586133418d3fd5f36323e5f03`  
		Last Modified: Wed, 01 Mar 2023 02:22:30 GMT  
		Size: 65.9 MB (65937993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:58f7776ae5802beb5ff95c124b893ff3a2ce121f93e98d305337e9feeeb340d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131875223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dde5105ffa4ba49e36c8a2afa67c343d1f83bde2ad9dde91a2a56b5056c6d4f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:09 GMT
ADD file:bff5ae942e6561f2afffbbd0267d57706f7fdd71ebe43c64b369b20940d55f00 in / 
# Thu, 09 Feb 2023 02:43:14 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:32:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:33:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aa6addfe979ac43879ea9517851622f7a6c1516568fbd6a0c101c3b86cc1163`  
		Last Modified: Thu, 09 Feb 2023 02:51:51 GMT  
		Size: 49.1 MB (49063446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6db93799880bf6f9525fc696324e0d450fd37ebbb37d356955a9057236da38`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 8.4 MB (8399010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b19fed47eb69b023968097b12ef67cad0d7e15a03675cc16e3efc9b67a44e4`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 11.1 MB (11105521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7152f2a237e2d177c5dc02d27a4b1e0433902b36280eb92369c2a9e5620678e`  
		Last Modified: Thu, 09 Feb 2023 07:57:24 GMT  
		Size: 63.3 MB (63307246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ebef91cd94f5561186fb0b696247790d031846171cfc5662c9592c36adce5858
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144588786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524c9ee0845a8c69cf6771af7edf1490f94ce4d0dda21968e413a26752e9b320`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:46:00 GMT
ADD file:311d9174b941eeaaa2babe3a94b035ab7c3880d5908d630bdec420f42eff6a06 in / 
# Wed, 01 Mar 2023 04:46:05 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:18:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6b61b4a96c9a944bd44d67cc885cdb2ef5f9aa35a0a94dba6ea2b6372ad27e48`  
		Last Modified: Wed, 01 Mar 2023 04:52:26 GMT  
		Size: 53.3 MB (53250230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a057e1f93c20f3bf648ce49e3455619f0854aef331a7d297c7425e435adfcb8`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 9.6 MB (9631581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb4683b31216d30e252186c2c0cb6f06f69d737321cb3d95c8f1036adca0bea`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 12.2 MB (12168325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18e9322efa86ed752abe3ce6c6627d95fb158f9e6fc57b15a1dd5c4eeac07ae`  
		Last Modified: Wed, 01 Mar 2023 05:38:09 GMT  
		Size: 69.5 MB (69538650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:70d660b84d8823209adb0b68ba88f2b2bec7a47b14c638270edbc9242cb64841
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130649917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e1f38dc04be68c2fbe7138cf87bcdf1c061ef8a1f11fb0e2353575347e48b18`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:49:37 GMT
ADD file:55baf50ca3524103dfcb38a8784744d482a5cdb19f66a7baa92d44dc18483a58 in / 
# Wed, 01 Mar 2023 02:49:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:12:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e95e47ef2a5cde1145fe4af2db22dbfe40c09cf83dbb9ff00d400d23e6dd5331`  
		Last Modified: Wed, 01 Mar 2023 02:53:58 GMT  
		Size: 47.6 MB (47608102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf204e7b8be3c288518bf65a248e94d7d77b56c235d30b3eb93058f663337226`  
		Last Modified: Wed, 01 Mar 2023 03:21:19 GMT  
		Size: 8.7 MB (8684339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca66d3959e328f7d96d65cb0b1a3f79c9c7f949a2fefecdadb692344f6e8a5b`  
		Last Modified: Wed, 01 Mar 2023 03:21:18 GMT  
		Size: 11.3 MB (11268858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb5857b88499838945e97d7c6a6c6ebe9e8cedf2f9e53fd3969022b50bafb3c`  
		Last Modified: Wed, 01 Mar 2023 03:21:34 GMT  
		Size: 63.1 MB (63088618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
