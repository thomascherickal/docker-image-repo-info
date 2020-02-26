## `buildpack-deps:jessie-curl`

```console
$ docker pull buildpack-deps@sha256:d351a9d1f02b893e390b41cbec3e310f95310b64fc7c234a70630c79ce762426
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:jessie-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b9b6a5e6511b33362adfa650028bc5629a51a0247dfac7827cd78e2760eb379c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71934528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b6128b4f6af8f8af9a9507251a5419f5955f19a5327a840383a70e61d8739b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:57 GMT
ADD file:607350db53d30cfbdaaa75b7a47bd59de2bfa83fe4a50be9e7cccddcbfa7c61a in / 
# Wed, 26 Feb 2020 00:37:58 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:09:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:09:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:92d14a6520e1a734155afb0c5b456614718259f56397290ed22fab220c2b96f4`  
		Last Modified: Wed, 26 Feb 2020 00:44:41 GMT  
		Size: 54.4 MB (54388885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953765cae32285a96cb8dfceb67d75359de4ed5b8c5ca50bcd1aeeaf19acb19e`  
		Last Modified: Wed, 26 Feb 2020 01:21:34 GMT  
		Size: 17.5 MB (17545643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4476d7e18867de28805a2b20eb88cd3cfe88c0fd06a73b5710926470fe9a66c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69616076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf84bfbaec3d4f45e0e35e9213002a8c7d636ec66d027bfb22ccadbddb9deb1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:54 GMT
ADD file:32b8a625927c1f5bf5f1b4ba44bb1c2af32e6dbd8f0a379d6a0a7612aacb9939 in / 
# Sat, 01 Feb 2020 16:50:55 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7911b8b96f54b072a80e08f30051237d4db6aa19229c178eadfcb7a0448a1504`  
		Last Modified: Sat, 01 Feb 2020 16:57:29 GMT  
		Size: 52.6 MB (52579602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4464e1d3f05f646bcc989c3bd8bbf247c2c65c1787f9b741b44e7b0eee15a2e`  
		Last Modified: Sat, 01 Feb 2020 17:46:53 GMT  
		Size: 17.0 MB (17036474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fe36ac970fcca0e2572717dd50684edfb36f7a66ff020960f416d9c796bef1c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67025676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f97997ca7b9b44c770ee0c5ab700cf61f40ef29ed6c00c24902c5a2cbd4bdbee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:39 GMT
ADD file:a467dd7304add7a1979638d51c2e28f9355aedccfd4727532a90b0db7fb1d9d6 in / 
# Wed, 26 Feb 2020 00:52:45 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:16:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:16:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10fa2b45efadcc8561689d641256044af7890a575a625a567d96dfbbac1c5d05`  
		Last Modified: Wed, 26 Feb 2020 01:07:57 GMT  
		Size: 50.3 MB (50302762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc01a96123ffaa0c4c0e711f6d51ee89062e113913ee9965abdd34e60170cc3`  
		Last Modified: Wed, 26 Feb 2020 02:35:03 GMT  
		Size: 16.7 MB (16722914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9f4f3e5a33237b6e53cb1d378f5a0bd245eab14c28bdda57828018da8bc7e220
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74463001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42abd2a123672c1ff830ee842a29021d9e4fe5d10b2f01c0f7b3823f3078234`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:34 GMT
ADD file:55edca1096804fbcbd260441dec447b0ee75e01826e82a48d2f4743c90ee01be in / 
# Wed, 26 Feb 2020 00:32:35 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:12:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1fe0a93005696879fec845d0ec4f9bfaf8c2e5d43a8bf4dbb1aa7bb31ef50aea`  
		Last Modified: Wed, 26 Feb 2020 00:38:54 GMT  
		Size: 54.6 MB (54607169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127f47054d5ddf851c1c3cbe9918f68fd635af42568819db800aed86dd229c0`  
		Last Modified: Wed, 26 Feb 2020 01:28:46 GMT  
		Size: 19.9 MB (19855832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
