## `buildpack-deps:hirsute-scm`

```console
$ docker pull buildpack-deps@sha256:540342c46d76db22368d7efc404214fac6390ffd4fd3971b2be2b498a251e3bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:hirsute-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e4b34d9ecd5c159571e7c4aa5a92e5f59021eae78e6b03e1619fad1216f46a17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.3 MB (84338648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a3cb2eb560e049b85cb7c014a687b3aae9ce86dadd0640b986879a2d7f70cf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:12:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:12:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e61e03c60557bda70bf3cc9a2dd5562bdd9f66442dd9a5b33f393f7f610ca9`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 5.4 MB (5429421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1701598239c3ba301af98cdbdc4c053cff70425e0102d03a0a0a660b68520b35`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 3.7 MB (3662530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bdc834e59f4ded456cfe6c6f10cc62573219101f62812b9e6aa4fcb1724d6d`  
		Last Modified: Fri, 01 Oct 2021 03:20:11 GMT  
		Size: 43.5 MB (43542401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9804a4fd9b159a2bf14e2e9fecfafd454b98c57b208e9f1cd046c5367321421e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74810383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa57e9ca19a6490459f1d1b27fc9522ba5af6d70e5bf5de22e6d43365e578599`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:24:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:25:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8944eff0f4815cf5a70868ad5afaed083de9f7ead5a73bc97fa5dc147a04f9`  
		Last Modified: Sat, 02 Oct 2021 22:40:51 GMT  
		Size: 4.9 MB (4858463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bed8cb9d9d7259532d0d30040f4f46ba30d3dedae6e7d37d51c4bf9f60bc54a`  
		Last Modified: Sat, 02 Oct 2021 22:40:50 GMT  
		Size: 3.1 MB (3139002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8efec2f84a292f59a270ac67ccb130692e15a90a3105f135600dd1ee32bed4`  
		Last Modified: Sat, 02 Oct 2021 22:41:32 GMT  
		Size: 40.0 MB (39953431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d9446fb751659cac97fe4602a547a07c488b2e551c439846879acfe1d17fd7f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82739629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c6cb7af054be1655c285f42e5dc616e5c700b2145d26cfab1540f6fcf5034dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:18:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:18:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:19:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22e5e9de7272c5e4544f153bf2aeeb8c118ac5a3ccdea10a7d6a6c996c3575c`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 5.4 MB (5400844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c320e18b5848a613875caa1714ab609c4840c23b41f7eb20a8d3dc34193f53d`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 3.6 MB (3638468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47cb72d2d39bf513d49bbb200478599434e3db9569aef12f56685039732f370`  
		Last Modified: Fri, 01 Oct 2021 03:26:46 GMT  
		Size: 43.5 MB (43526154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:08c18882a70aad8af2599f0170a98f8c20db30a91fcc5a77d3b043e5bfc7614c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.3 MB (97332366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5211c4bfed288ada093bfbb9e2f58c5f291103d5c360755d5ac8be047e188f50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:57:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615e5e41d59fe32c6e6c5284994935d713f08ed29bdc3f9841683f0793cf8394`  
		Last Modified: Tue, 31 Aug 2021 05:20:33 GMT  
		Size: 6.2 MB (6155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99aa8209221f270d9ffc050088f6998d6ceefa228f2ca68f9eb5bc410b24fadc`  
		Last Modified: Tue, 31 Aug 2021 05:19:57 GMT  
		Size: 4.5 MB (4523763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e43d357f3322abb3a717de7eaf87420b14cbcae1a2c006e9267578aa7c7881`  
		Last Modified: Tue, 31 Aug 2021 05:22:13 GMT  
		Size: 49.5 MB (49467214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:f65fa8029821604824f633737c48c72f705393e217b105f05b5b0666541fe3d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75593792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b647358b6ce20b1f16ee3cba013956f23773270e2ad5c14a3acf32d1f3d7f1b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:10:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:11:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747535e5ca63ea5be385acb70aaca4311fe2b78f1e44463cbfce298800f9f33b`  
		Last Modified: Fri, 01 Oct 2021 02:50:40 GMT  
		Size: 4.9 MB (4944581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0facf6815c035133c1d22c89659eabcd14838fa24ff638d7a2f822c2d42d795a`  
		Last Modified: Fri, 01 Oct 2021 02:50:37 GMT  
		Size: 3.2 MB (3177915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f4c1d69caf6add02d4549d216e9e00fdaae087f4d280cea93bbd3f8b3ec48a`  
		Last Modified: Fri, 01 Oct 2021 02:52:36 GMT  
		Size: 40.3 MB (40329415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d25b90928f781d816d02bea7d8f54221a35b29730fd84d0a00243b3b8bdb3e73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89892323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f73f0b59e7117c44cb5c0f23df871f926492ee7502ad7028f57ca74fe86c8cae`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:36:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:36:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a99a5951692580021e948472804dab0a010b074b1163b603e4f5cfda6382bf4`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 5.8 MB (5801664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fa544ba88c98b23feadb6ad914d8da1debe080907cb082ad2b8d8046e6c5da`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 4.2 MB (4185318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f556cc2020b283f43fb541b48641c7dd9e20e8d7d40de1a098420d28dbe5b70d`  
		Last Modified: Fri, 01 Oct 2021 02:43:07 GMT  
		Size: 47.4 MB (47399802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
