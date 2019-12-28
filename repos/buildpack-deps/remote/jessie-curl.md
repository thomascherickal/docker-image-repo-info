## `buildpack-deps:jessie-curl`

```console
$ docker pull buildpack-deps@sha256:644ea6791bec09db43cebfd9e804c75dae2f43a34feb9e0129aad2f351fb49a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:jessie-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:48c1eb6cb8769434c89c194c34266140d5225d78e8d45833eb001bcc635f431e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71935125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89dd2448f7dae10d9cb32766ae016f3b2714d8070b98ad4afdd241c951d4929e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:35 GMT
ADD file:6bea7fdf1d11cd3f2dfa923395205f70d42d388f597b21e289e7f516a2c687f1 in / 
# Sat, 28 Dec 2019 04:21:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:51:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:51:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a4888a2f4fb02c1971555f590f5c9ef6369e7fa4599e586fb70cdfe80330370b`  
		Last Modified: Sat, 28 Dec 2019 04:26:07 GMT  
		Size: 54.4 MB (54389662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fe6cef1db298eb80da7e99c0df1d8cf44011585831905df6373b5dbb32e0a8`  
		Last Modified: Sat, 28 Dec 2019 05:02:45 GMT  
		Size: 17.5 MB (17545463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b3a093758699a05f34d6354ead4f98e34f313bc886b22273fff31a180ace37b6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69616119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad2fd4ee65d1add1616a0d363ac308d6d6b423671d419d6741c047a5793fdff0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:50:07 GMT
ADD file:d4edce93ba93edcd37d608a9b631879fc39506074ab425c75b3c55c68ce0f349 in / 
# Sat, 28 Dec 2019 04:50:10 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:31:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5fdba72d0442ed279b2949203d28c37c7388a87145a31eff8a5dbd1ec4d3f8dd`  
		Last Modified: Sat, 28 Dec 2019 04:56:54 GMT  
		Size: 52.6 MB (52579512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185dfc772e20f53d92109142b40655cb4ad05fd0c5a9d98fbc8588dbd41be3cc`  
		Last Modified: Sat, 28 Dec 2019 05:52:05 GMT  
		Size: 17.0 MB (17036607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9893a10311c667392b8c568abf1b743712d166c84a16aecb89dcfb62de03b2e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67025867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1733e4b1a7e48e3c8495e367f8cec2c3b29c3ecbc49d3ffc98287edf304d45e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:23:14 GMT
ADD file:110bc0c1b675b285bcc5c961ecc9df9a3d68e240c3f87ba3d1e446d7b01817d2 in / 
# Fri, 22 Nov 2019 13:23:16 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:15:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:15:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c944918a63c296a1200f56386f2e6568cc9dd22dd8828e6b7595124662826f5a`  
		Last Modified: Fri, 22 Nov 2019 13:33:48 GMT  
		Size: 50.3 MB (50303247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e57de99ba7bfe3e75eebfc97015acc829fc080fa57138dc099c33d4b1283da3`  
		Last Modified: Fri, 22 Nov 2019 23:31:56 GMT  
		Size: 16.7 MB (16722620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:015bbdbae59ed546f1aa6e68acff0ec0c9e51663232aeafb9d3b08f578d99c3b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74462643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2964477894db721768ab1126c854af2c6d9e59f03c208d22f66e799929c93bdb`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:48 GMT
ADD file:e0837cf024229091926211f978dabf672673212fd887227ecbb668eaa07b64eb in / 
# Sat, 28 Dec 2019 04:39:49 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:27:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:27:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ede3dbff736b8a8510fdbb387e58c82d2efd65021b945e042efe623a81b3e961`  
		Last Modified: Sat, 28 Dec 2019 04:44:42 GMT  
		Size: 54.6 MB (54607465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b718c467bf649514ec1a976027e559e28c2abb8ac429739f94341d0ac1c5142c`  
		Last Modified: Sat, 28 Dec 2019 05:44:24 GMT  
		Size: 19.9 MB (19855178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
