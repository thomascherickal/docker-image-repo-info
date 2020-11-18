## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:a1f2ee0c029c9ecbb51f2cbabbfc5fd6171b53fa97a44a11e79fdb8ee2e79def
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:edd6ecc5330ceafb541c9071c835b33c6371af3b59b1e7f300717481d0967dc3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110580694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf427cb2ddc57b42bf180e93d5b31a0cd8228284b9ee714c7b5e675bca7abf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:10 GMT
ADD file:373a8875589f170b51fa677a3bf736feeb46ea278c553950a3eb3169a2056c12 in / 
# Tue, 17 Nov 2020 20:24:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:44:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7919f5b7d60254cafc73c0d097b8ccffb72e0b6472957ece4dd5b378c5ca7cc1`  
		Last Modified: Tue, 17 Nov 2020 20:30:26 GMT  
		Size: 45.4 MB (45377037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e107167dcc5392ce7b34cb6af6bcfe1cf99f76f9e632d6c321526666558ab50`  
		Last Modified: Wed, 18 Nov 2020 00:54:39 GMT  
		Size: 10.8 MB (10752152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a456bba435b99e4c17dd5da957e63bef2c43ae5291b055ce82bd26d9153259`  
		Last Modified: Wed, 18 Nov 2020 00:54:37 GMT  
		Size: 4.3 MB (4340590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5435318a0426be8944e8142c90c8501d9f27e23cbd27e1094311e292dcfbc926`  
		Last Modified: Wed, 18 Nov 2020 00:54:56 GMT  
		Size: 50.1 MB (50110915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:5a692085d405822acbd335a915d1986616285f946a20d76ca2367b0a1e130998
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.4 MB (106377386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bfa43afd5c628126e5665336005e431653420714c871c7a1597b149d3144434`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:57 GMT
ADD file:757e33f8832983f079f91ba77cfca5d62b54fe656af623e8566481f0f7a35d8a in / 
# Tue, 17 Nov 2020 20:25:15 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:00:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:00:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:01:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7850b9d990d72513afd82e6c3923a3fa328516bcda19d9e0d7a63ea8f62f0b0c`  
		Last Modified: Tue, 17 Nov 2020 20:34:29 GMT  
		Size: 44.1 MB (44088729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9dbf9463f553cb529257e7f6604f90869dcef003f695feb1938125ff26678a8`  
		Last Modified: Tue, 17 Nov 2020 22:14:16 GMT  
		Size: 9.8 MB (9825627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53613aa57889fa10935262ea57103cd18919ef3bffad006a23c33619258595de`  
		Last Modified: Tue, 17 Nov 2020 22:14:14 GMT  
		Size: 4.2 MB (4160144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b0c978ffc792b386bc74b4233406c058603a28ca3ad52b2838e8e6e6e900d6`  
		Last Modified: Tue, 17 Nov 2020 22:14:40 GMT  
		Size: 48.3 MB (48302886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ea4e3f52e8d8073e3bea484687f3fb8cb66852cd4c00be19a208d4dd206bbc43
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101894810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc8c5abb2bde0dae164ef63e6c53a8f8a82cffe0a7ff54eb22391d8cbef848d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:26:47 GMT
ADD file:58b80132bbfb3cae1eb2a9345e362cce1e39de41055fdcef8e5a8a8a447f69b0 in / 
# Tue, 17 Nov 2020 20:26:50 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:57:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:57:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:58:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfc77fa15d772230821249f78cfbb69a8fc6596f6867601b9dad16aedb424325`  
		Last Modified: Tue, 17 Nov 2020 20:35:24 GMT  
		Size: 42.1 MB (42117734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1d24dbd0f85452f20a934ea14ebc3dadfdd8493317dfe8f7f2aa1772937953`  
		Last Modified: Tue, 17 Nov 2020 22:12:47 GMT  
		Size: 9.4 MB (9444101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90255e5a0a934b36df89ac1c1842d07d8d7ed4b3531898af64fdab8372662e3e`  
		Last Modified: Tue, 17 Nov 2020 22:12:46 GMT  
		Size: 3.9 MB (3919908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d3541348c25cd4a2346df5fa88cd6a4eef94c72fab598b9b2ae20afac1ca4b`  
		Last Modified: Tue, 17 Nov 2020 22:13:13 GMT  
		Size: 46.4 MB (46413067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:90dfbd0c5a0b2823033dc6169e0469ceea450d0a2b330181f9a1afa1bf36bc8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105016862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4550df63acb3990a4195528ed73a3131a0eeb1ec71d4b535427f9957ac7ece1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:33 GMT
ADD file:d2e307c3e54ad69dff47f6bdacca7c8ee0957a09346bb21baec02b9de1a657e1 in / 
# Tue, 17 Nov 2020 20:27:37 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:28:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:29:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f99bf631c0ebddf9e32516b47bf6e198efc42d06c3eb86d6f5f5739757b5839c`  
		Last Modified: Tue, 17 Nov 2020 20:34:17 GMT  
		Size: 43.2 MB (43176009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a9b3adbe4ac4ca73818d8b79e94d2ff2b6ceafc1225d7c036ec4d384f0804a`  
		Last Modified: Tue, 17 Nov 2020 22:40:38 GMT  
		Size: 9.7 MB (9702292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052ba804da6ef34fd9dddf0ca298b1e0551ac8cf3ea14fc371fa1fa51cbd7f7c`  
		Last Modified: Tue, 17 Nov 2020 22:40:36 GMT  
		Size: 4.1 MB (4095219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4839ac53f1fbcca75943ff4ddb761ce018accd0fc19cae8b8776b1619e3d61`  
		Last Modified: Tue, 17 Nov 2020 22:40:58 GMT  
		Size: 48.0 MB (48043342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ccd03fb0dbd7795496b0cd17abec913a86a33deb466a6830cbe965ffd630b76e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113059193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749e3b4a21dd4d03fef49d887ba29eab5fb696d083822cb8f515f46453184aad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:07 GMT
ADD file:7d3a7e4509bddfd0743cfbbcf7420937a48151e0123a0cae600e9485a3f4bfe5 in / 
# Tue, 17 Nov 2020 20:23:07 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:19:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:19:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:19:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:893c5e9df6a4376b9e3596b0e60bdcebb5a49a311ea41ef3742718b00f71656c`  
		Last Modified: Tue, 17 Nov 2020 20:30:04 GMT  
		Size: 46.1 MB (46094887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d862406a72c23fb5aa9d390543194dbeb7bf0b7ca09251c325e1b18777329de`  
		Last Modified: Tue, 17 Nov 2020 21:27:53 GMT  
		Size: 10.8 MB (10774543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb8f70e2c88fe947ee86ac565c88e31c54182935c48a07a9b9821e00bb83553`  
		Last Modified: Tue, 17 Nov 2020 21:27:50 GMT  
		Size: 4.6 MB (4563098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180b91758f0fa1cce7719daee71bebb0e896d9facf7fc1f4f55cef48bbaf3172`  
		Last Modified: Tue, 17 Nov 2020 21:28:14 GMT  
		Size: 51.6 MB (51626665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
