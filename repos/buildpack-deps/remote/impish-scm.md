## `buildpack-deps:impish-scm`

```console
$ docker pull buildpack-deps@sha256:f967a20e890a52e751021d4621bd604f399c96096267ef2ebfdb9818a91b53a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `buildpack-deps:impish-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7d31e4b601f7ad3f887279f6d1417f30839e10a086290197bb1f91d10efa9b07
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.7 MB (78748191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe3eedca0c58506597351a858efcd76151aea3fd56ffcba23d547e2e7334c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:30:09 GMT
ADD file:fed31f525edbf4773d5c5dd77d89b40e3c4e2b018cd73ecdcfca8294b5daf963 in / 
# Tue, 13 Jul 2021 22:30:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:41:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a11e0c4b985a14790a9d1b7fc1c23c3e4534495df3ab94ab579474c7ed80abbb`  
		Last Modified: Tue, 13 Jul 2021 22:32:17 GMT  
		Size: 31.8 MB (31763760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f85d2616834f3c9c5b9a5170c5afed8468774c80a1d78fb6e64bb4fa2305bb`  
		Last Modified: Tue, 13 Jul 2021 23:48:51 GMT  
		Size: 5.4 MB (5445866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d1e6d35d2422b6ec0f2a5ac71f8d4db4d9d4a7d1d892f5f88d897e1189997`  
		Last Modified: Tue, 13 Jul 2021 23:48:50 GMT  
		Size: 3.7 MB (3658859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18265ccafaff7a6cc5867107ee40777cfb100c9297c0eee1cecf578ba40246df`  
		Last Modified: Tue, 13 Jul 2021 23:49:08 GMT  
		Size: 37.9 MB (37879706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:44daea5c53948d154aa17b37220d3b970793220f7558c687a791177b864c1497
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74943732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17875851baf9ac9bd8d5f22d4403867d9b2c43424aa66cb49c60e85b635059dd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:22:24 GMT
ADD file:2888fa0aa4baaaed5388c590baea27cba3d71017f1a390bf10191b18f123114c in / 
# Tue, 13 Jul 2021 23:22:26 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:02:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:02:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 02:03:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7fbf6def801b74c6b0c1bfed8350c986239cbb5ed41824f04074b3be99d3d8eb`  
		Last Modified: Tue, 13 Jul 2021 23:28:07 GMT  
		Size: 26.9 MB (26874823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b6db0e964dd1265915e27b1381e39e1188b975992aa758f2e7c7835a7bff80`  
		Last Modified: Wed, 14 Jul 2021 02:24:18 GMT  
		Size: 4.9 MB (4870392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea4a6ea0d1955c472c561adbc97899fbad18d1f6693e475a93a56699ead5f4`  
		Last Modified: Wed, 14 Jul 2021 02:24:16 GMT  
		Size: 3.1 MB (3139920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb4d3aa5c1dff9eaabbcb71cc0461969404c24eb3870caee150083d27a1dd67`  
		Last Modified: Wed, 14 Jul 2021 02:25:00 GMT  
		Size: 40.1 MB (40058597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:43a4917e3dc93283c63932c05942e37aa4973bedb2658b0385983e0dcc80eb8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77124649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108c621c8632be12e720dfa803e0b8375fa9370e6e5a81379a29fbdee703bdea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:57 GMT
ADD file:de726c8b286d17c655e46862c0d19a05b6322f245d12a64d4f081f86dbc50d57 in / 
# Tue, 13 Jul 2021 23:01:58 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:56:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:56:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b278a523c5f40181d31e0d016c0eb35135a9f686db2a8ded8ee3956984302028`  
		Last Modified: Tue, 13 Jul 2021 23:04:41 GMT  
		Size: 30.2 MB (30190328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5300c896e9c7b8f095a5807eac2ad200cd231b145d172d136ba627b25e0602b`  
		Last Modified: Wed, 14 Jul 2021 00:05:20 GMT  
		Size: 5.4 MB (5413602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271ae391da3710f15cf10087e7d8cd70179249ea34d9569458eee8836c51d691`  
		Last Modified: Wed, 14 Jul 2021 00:05:19 GMT  
		Size: 3.6 MB (3636126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466acd68fcdcea40806d18723fc63d83fccd5a54c8f0034f0f1d204f390f2f91`  
		Last Modified: Wed, 14 Jul 2021 00:05:40 GMT  
		Size: 37.9 MB (37884593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
