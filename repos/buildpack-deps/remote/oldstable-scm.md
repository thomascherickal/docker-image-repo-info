## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:cc1b35e2898687ddc8d8a1647a6ab5bddf97e5353bd295afde64c83334f0b54c
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
$ docker pull buildpack-deps@sha256:b986a009ed679b7298fba7680918f736072a6af74a70a66f9d70530e7f50e291
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110585066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8503a8dd08a66466cf03c165dc61eff01374b5b7d3411efb35780432af49445d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 04:00:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 04:00:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 04:00:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953fe5c215cb5f929e0e42e5a1011f33edce9278a650faf10655e855a670f79f`  
		Last Modified: Tue, 12 Jan 2021 04:08:01 GMT  
		Size: 10.8 MB (10753468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3f270c7deffd353181076af3b5746c8dbeac5abf454169a75e7822587bdab`  
		Last Modified: Tue, 12 Jan 2021 04:07:59 GMT  
		Size: 4.3 MB (4340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed36dafe30e3d9c4fde74478dae686f851d7e93b719dc3165d8eb7e8be9305d9`  
		Last Modified: Tue, 12 Jan 2021 04:08:23 GMT  
		Size: 50.1 MB (50110938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b37f382bdcc9addf9c484ad69862f57bc16ea7500c07b88f1f218b8747fb1e20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.4 MB (106381551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92d9b135dfa9f58b11ac073d7bf187cbccc43064e3b3bed13d6e5a02a011ff8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:55:15 GMT
ADD file:3047f832191e46ed288c3efd5d017316fc7b7d8fbd282800d02da8ca0f799430 in / 
# Tue, 12 Jan 2021 00:55:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:36:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:37:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:37:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c99253078aee5285b1d9437ad45736eccc40de8b1007a23b3de45924452cfb0d`  
		Last Modified: Tue, 12 Jan 2021 01:04:44 GMT  
		Size: 44.1 MB (44091438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8cd662e395616851748f77d200cebcd23c0ff3e1416b086bba54350bdacea9`  
		Last Modified: Tue, 12 Jan 2021 01:47:15 GMT  
		Size: 9.8 MB (9827084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae70193a410fd3620313dc1177f88c9edcea3db4659c8d9da8294f29939e21`  
		Last Modified: Tue, 12 Jan 2021 01:47:14 GMT  
		Size: 4.2 MB (4160279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b82525c1b286ca16c60a4769d1d318c6e2555de48b58e90c951421088d3627`  
		Last Modified: Tue, 12 Jan 2021 01:47:45 GMT  
		Size: 48.3 MB (48302750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1d1a3960456783bafab1d51197bc6a47d2bec67820264c731de04f999f4981ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101899357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02e2f265baa94edc78144aaeaa96b79ea9051eb2c7d0b37962dae7da24977ac6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:05:19 GMT
ADD file:9c744a203d36aa8c515bbc11873a4a479cdf3fe9f020ca1ef207b53e6b3a251e in / 
# Tue, 12 Jan 2021 00:05:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:21:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:22:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f5de2649c1cd9091872f81b8ceb6a67890124f113d9fce9c52bf60d5a6e19f43`  
		Last Modified: Tue, 12 Jan 2021 00:15:23 GMT  
		Size: 42.1 MB (42119951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cae60aac6e598935e2b14216dc4265434ba03d17c82f622b18abb712577d2c`  
		Last Modified: Tue, 12 Jan 2021 01:34:01 GMT  
		Size: 9.4 MB (9446203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9694e28a75917ff08caeaee5ed8729a2f12d2110bf203781d578006a0ef2f7`  
		Last Modified: Tue, 12 Jan 2021 01:33:59 GMT  
		Size: 3.9 MB (3919958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49da7baaa533b2272938593647e65b46d3fd7a5df2211e746229f18c95ea81fb`  
		Last Modified: Tue, 12 Jan 2021 01:34:27 GMT  
		Size: 46.4 MB (46413245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eaad05de54581d05b7d6fbf0eadf3eb554691bf79507b72fcf1faab4d70a0981
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105020674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e0aabaa0dc1841b1bafcc9bb5638ecd8a24b7a2b218e973f2ca38eb853b3f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:18 GMT
ADD file:bc4af94773a01defa7a79adb22199dde2229843dae224d13d3385c522cb71652 in / 
# Tue, 12 Jan 2021 00:45:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:30:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:31:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec4f0a0f30ab1b4fc2e412a926b8608502de98203ca1994c7916de2017136729`  
		Last Modified: Tue, 12 Jan 2021 00:54:45 GMT  
		Size: 43.2 MB (43177964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d21e1234248b5afd95bc41f061ec505353daeca6d4d5312a0167507857e72`  
		Last Modified: Tue, 12 Jan 2021 01:41:51 GMT  
		Size: 9.7 MB (9703645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e47f4b9ead7d5e8caca5072922207d5aa928f0144af32c78cf5a7e165f1898b`  
		Last Modified: Tue, 12 Jan 2021 01:41:48 GMT  
		Size: 4.1 MB (4095462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12669d76f10697ce6f8db3816f905c864edac1edb9ff9264a5c77c52e93e970`  
		Last Modified: Tue, 12 Jan 2021 01:42:16 GMT  
		Size: 48.0 MB (48043603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:fad8f503817ef848b433108bb05c0ab0f4b402839ea6bb2db71c62f6927586eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113064613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9da3fda447754d53e2ae30dea916a0aeeaf73d12486941e178a8e1540791ea6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:00 GMT
ADD file:0da7fb4b520f7df6963291eabeab1e021ecc9f8fa5507ea307b64cd109898702 in / 
# Tue, 12 Jan 2021 00:42:00 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:23:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:23:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:24:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9200bc3dda820226401b71a8464b0ea725d889387e461c9cf3d8155012f09f94`  
		Last Modified: Tue, 12 Jan 2021 00:50:31 GMT  
		Size: 46.1 MB (46097646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3342e22b1246cb06a9a56c2d434f5a71bacf828347b0960a4757743ce537e59b`  
		Last Modified: Tue, 12 Jan 2021 03:33:38 GMT  
		Size: 10.8 MB (10775953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb274352ab417de2d06e1b8086789a02423e1d5aaf7fd8263786b0afa39aedd`  
		Last Modified: Tue, 12 Jan 2021 03:33:37 GMT  
		Size: 4.6 MB (4563315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ee6a11a71c0f8e1468772536af0c036df220c5546bbb5c7526af611074a0a5`  
		Last Modified: Tue, 12 Jan 2021 03:34:02 GMT  
		Size: 51.6 MB (51627699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
