## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:5d0ebb760a40d211805bb357e2076b120a0853198a0ee42fa8a2287e35c959d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d9d32abca878552d8cbeac9cef4ebe13dbd79b2e5a7e870fe6cb4e328623f8cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39959110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bf8c658980fbac31c918b62f1d143c54ec282d324829b8227e5ea0343502ab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:28:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbaa066a683dc28989e3eb0b728605c7c70bc4b52271fb9ab54afd86adf9340`  
		Last Modified: Tue, 13 Jul 2021 23:45:33 GMT  
		Size: 7.8 MB (7769217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c738dcee3895426d22a9e75e8be4ec85f891c23ae879ba1a365d61d34e833fc1`  
		Last Modified: Tue, 13 Jul 2021 23:45:33 GMT  
		Size: 3.6 MB (3624030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:65e3e8f41aea17b28b66fe645cb822b7c05ed26e5d8bf00c4cee5a4f97d42075
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33932322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38fd0b858d8b4467b21125237f86803bb7c4e6242beacda56cd30d4bf52837c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:51:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:52:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed249db5e4f1496516d6a4c10ff289843df3f21648df9e24e36bc1b645798f03`  
		Last Modified: Wed, 14 Jul 2021 02:16:21 GMT  
		Size: 6.8 MB (6766542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dddfbc3ef9239dd2d30749243dfe662b1fc9701fc338d7cedaac8f75b0cb14`  
		Last Modified: Wed, 14 Jul 2021 02:16:17 GMT  
		Size: 3.1 MB (3103714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:04ed0d57d89d0b57cdf8127fb32120855c20684b46db96e9779df2df08ff8510
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38403841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c69300956d4e725bbf0814aeeca1b8b4f941f39052c8e21bb61e2b9b65d538`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:51:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8068365a70c08261d3e893e294ef06766f03eb4b328fbd9f9ee02518d306b62`  
		Last Modified: Wed, 14 Jul 2021 00:01:44 GMT  
		Size: 7.6 MB (7634354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c649808bb14a85a70355b7ca704a3d0ef2d42b5ce714fb3688dcc2e9a0d82df`  
		Last Modified: Wed, 14 Jul 2021 00:01:43 GMT  
		Size: 3.6 MB (3600406 bytes)  
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

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0b28e66df7dff1e931769a60735ad3d8203464018a12427e67fb82ece8bd1d4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38120620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8530c4ebc32fb0d5482412c266f06aefb1b7801502e0eebeff37958d6e95f4e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:53:34 GMT
ADD file:ae5354f89d91eedd0614e3e97ee59fd6e23254923062c288d775e19b137dfd1c in / 
# Tue, 13 Jul 2021 22:53:36 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:42:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:761fa758059faa0c80b0b90fcbcc192fc7f573da055460d5b3f019e0faceeb7a`  
		Last Modified: Tue, 13 Jul 2021 22:55:47 GMT  
		Size: 27.1 MB (27149318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d8c0bf47a6fdda1f1d498f8231bc1989fe2e8c2070b8dd2385d7ead1e5ab2c`  
		Last Modified: Tue, 13 Jul 2021 23:51:27 GMT  
		Size: 7.4 MB (7429091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e713df0bbfb7887fb64228cab5e6895b5303bc72ac1618bcdeb9fbdf3bbc13ce`  
		Last Modified: Tue, 13 Jul 2021 23:51:26 GMT  
		Size: 3.5 MB (3542211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
