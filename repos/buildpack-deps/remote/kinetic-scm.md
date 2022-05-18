## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:d54db216e4367cf979e4c9249cd1d71899301cf7d1fb67644f9410bf2e28870c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:426c1ba2dbf2def856a8201f5a2c9ebc880c465f744034548ec3072697d866ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79748239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38704d064123d7c2db797f2b82c528392df4745147dd5ec7609ceac9cc08ea52`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:23 GMT
ADD file:ebe265aac135a4affe0b35a5e79cd43480dc94796fba7b04095ff6dd92c42359 in / 
# Fri, 29 Apr 2022 23:21:24 GMT
CMD ["bash"]
# Wed, 18 May 2022 18:20:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:20:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 May 2022 18:21:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0ca6c954284ce98aea2c55589ebabd347d2caf3ba94387f53b5339c1f35ab8b7`  
		Last Modified: Fri, 29 Apr 2022 23:23:13 GMT  
		Size: 30.4 MB (30420973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34593d6d3712c4ad4ebef4d6f4a535e446351dec50e06ad8b998f5cb4a2abe4`  
		Last Modified: Wed, 18 May 2022 18:26:30 GMT  
		Size: 6.4 MB (6412971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec417ef712f9b3010f5c94843eff9d8b75a32b9ed38b90b0de2bf829e6f8f27`  
		Last Modified: Wed, 18 May 2022 18:26:29 GMT  
		Size: 3.6 MB (3567056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9a866b92531b3d55f0b37fda7eaffd3fff55f9d6283874a280273f18d8dddb`  
		Last Modified: Wed, 18 May 2022 18:26:45 GMT  
		Size: 39.3 MB (39347239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:232cc0cafe51764f6762ab8115226cc4684969652b8e6901bc1b8dd6f14b00fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78253883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54ee827e863d3b20a6f6520a24005348ea51a441bbd744ea88a5b6b93e4ad41f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:55 GMT
ADD file:063f432f8adfa6ad56a7bb07ff90f71f00c47c30a03bd892e04ddd744042a0d3 in / 
# Fri, 29 Apr 2022 22:59:56 GMT
CMD ["bash"]
# Wed, 18 May 2022 18:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:03:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 May 2022 18:03:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1fc430d8f49d4d10815388bc3cb533e89d8123bcc10ffd2a333c16216f2e4303`  
		Last Modified: Fri, 29 Apr 2022 23:04:36 GMT  
		Size: 27.0 MB (27015929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89783a5b9c1d5f0a22dbcdf255a84e8909a4e61a4eac70b41381b61121e2a38`  
		Last Modified: Wed, 18 May 2022 18:12:46 GMT  
		Size: 5.6 MB (5625692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253307b1acbd5f7f7e968c3da0fb29b31baa5f85c808566b01a3db407d77e1bf`  
		Last Modified: Wed, 18 May 2022 18:12:44 GMT  
		Size: 3.7 MB (3715955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d88d2a61ec5acd97d4faf8d5a7b2d44ae9bd535a9de00e899f87884d2c063d7`  
		Last Modified: Wed, 18 May 2022 18:13:27 GMT  
		Size: 41.9 MB (41896307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c555b73f2636b1a079202af885994a533477162a965a260d4dc52a752f0c72c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77146233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15315555386fd2237e3e79ab9af269af0ae24e0440623541371fd669c4407877`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:02 GMT
ADD file:1dcfa00d31cec211ba91522ed6fcf6f72e3f1f4ad30c4f7ca398add7eba377c0 in / 
# Fri, 29 Apr 2022 22:50:03 GMT
CMD ["bash"]
# Wed, 18 May 2022 18:41:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:41:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 May 2022 18:42:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:957fa4daed10cc16359daab2a50b5ffbbc1d762035c4eba567b3d4205e7afbde`  
		Last Modified: Fri, 29 Apr 2022 22:52:30 GMT  
		Size: 28.4 MB (28376165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecf88994911b3123256118b9bd96f3264984301fdeab08165451ae9e6a702ef`  
		Last Modified: Wed, 18 May 2022 18:46:03 GMT  
		Size: 6.2 MB (6200595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d271b6a5485276e4f0ae87970e4f3c9559a1dd51586b0c37d3a98260fae490b3`  
		Last Modified: Wed, 18 May 2022 18:46:03 GMT  
		Size: 3.3 MB (3326759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9d6cf5bae98dba51fa83bfb0f6271fa75c7bd5b07e76434b1612cd7004ba2a`  
		Last Modified: Wed, 18 May 2022 18:46:21 GMT  
		Size: 39.2 MB (39242714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:b663a1c68b8211673476ee8c13311adc9c4aaeb4850994d647cba9edebcb36fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79294591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42b3d6295990e26a25dfa28fc96258a1001de0751df77e482662bb65271842a3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:28 GMT
ADD file:88e52fba8a3ffc283333df24e0d115ab58328ac1d5f6cf585d17422676e146d3 in / 
# Fri, 29 Apr 2022 23:21:30 GMT
CMD ["bash"]
# Wed, 18 May 2022 18:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:33:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 May 2022 18:37:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e53595b65ef34f5f4d764d94e324a0b884612b1b49f768cdd94321c4f22fefd`  
		Last Modified: Fri, 29 Apr 2022 23:44:55 GMT  
		Size: 27.7 MB (27745108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71e2b3e035fbf74038baa262139105344a466094a8b69c84a3e3808b2d77a1e`  
		Last Modified: Wed, 18 May 2022 19:13:17 GMT  
		Size: 5.7 MB (5664247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2de7c23d6a5c7c3e733b1cbad086084a34c74a8d01aaa7df95a4245c3f5e875`  
		Last Modified: Wed, 18 May 2022 19:13:14 GMT  
		Size: 3.8 MB (3782735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fccda12cae526874d6fbdb368003a21309c6a0f4c332aac35b3b8d73dec90d9`  
		Last Modified: Wed, 18 May 2022 19:15:25 GMT  
		Size: 42.1 MB (42102501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f4db526ee67588d32d188eb0f3c1eea004544899531e45f66faaf3875b96065c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77496735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac33875f3dd47f7b2ce8d5723069c35f255c0517e66f5dfa14a5fc3717273df`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:44 GMT
ADD file:55affb702d0be7976581cacdb7c77f2c1b0d6921d2cd689a427471c2fd9d4daf in / 
# Fri, 29 Apr 2022 22:50:46 GMT
CMD ["bash"]
# Wed, 18 May 2022 18:44:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:44:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 May 2022 18:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c551bbcabccfb0977b8a9e2ba72099b05f9ba8b7c7106d8a29073b45bc73a9a4`  
		Last Modified: Fri, 29 Apr 2022 22:52:38 GMT  
		Size: 28.6 MB (28637139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc99034c1c5069115fde088e65757003cf7565698429334337590bf0a86bda5`  
		Last Modified: Wed, 18 May 2022 18:50:09 GMT  
		Size: 6.1 MB (6084504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690461f48e9ac677dc791f777d46ec994250897ad6d015fc260a2de96eaa82ae`  
		Last Modified: Wed, 18 May 2022 18:50:09 GMT  
		Size: 3.5 MB (3479076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37fda6c39e0ad2735d675f8a329621f3311eb325813ab3252ef68ce119bae80`  
		Last Modified: Wed, 18 May 2022 18:50:22 GMT  
		Size: 39.3 MB (39296016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
