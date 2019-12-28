## `buildpack-deps:jessie-curl`

```console
$ docker pull buildpack-deps@sha256:2f3ed01d5b0bb262ec471f08949b72530093761e334ee2ffc459cc2647e50fe3
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
$ docker pull buildpack-deps@sha256:bca28470fd467a5cc33faa517c37f4494b05dd57a849cb5e56a84c63ceb9c31e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69615953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2118cced7fe920c22b338b5066270518efee039e48c5bdf284badb24df6664d9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 12:14:15 GMT
ADD file:f77e817d0b96de22b11bcaf1ee01834a9e3a829a522bcedc2428a4dd32cf1c40 in / 
# Fri, 22 Nov 2019 12:14:19 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 17:29:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 17:29:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:12696cdf1c327a22f96256eb49799791558ad0df80803003d1c11a6d4b70658c`  
		Last Modified: Fri, 22 Nov 2019 12:22:44 GMT  
		Size: 52.6 MB (52579704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3b15c37e79cd2c57d8f3d175e9c72e733c75340371466c13f1414e2efb4431`  
		Last Modified: Fri, 22 Nov 2019 17:47:54 GMT  
		Size: 17.0 MB (17036249 bytes)  
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
$ docker pull buildpack-deps@sha256:f4ee8dff7d5937e4d758dabe86b31e3e1c73ba747790b07bd0ad62d826b614d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74462131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe6697f3aed89b130c78e6e4e68f786bbe177edc522ed132e739bf42252bce7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:48 GMT
ADD file:c195c387b23c684878aa122dfdc3eb14e3871253736c4f148cc4fb755cbaf364 in / 
# Fri, 22 Nov 2019 16:50:48 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:45:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:45:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:42aae7d55ebfb2ed8e18750c3710518e735ee2f4e3ace32a45a3d092531c3228`  
		Last Modified: Fri, 22 Nov 2019 16:58:48 GMT  
		Size: 54.6 MB (54607500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0dba4e47624a2824e1261310bb5022978a46adbb279c660c4a8e1f76de0bb5`  
		Last Modified: Sat, 23 Nov 2019 01:03:17 GMT  
		Size: 19.9 MB (19854631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
