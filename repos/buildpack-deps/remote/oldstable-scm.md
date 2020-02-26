## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:3ceb33d325fa62d3b7f349fc2fa733f9a8c55b6677b7be068d7b9e65fdcd8e6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:26172631ee0586a0aba9052a7959e041979434dc44b234c9b49e364bfd50981d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110583620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:971918da90f14872ce018673d9cc1f07699109b010c07f03844a6c77e3a23c5e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:17:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:17:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:17:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66997431d390aecfd02e57222c9b5752d314a4508de82c9b43c66812c3434ed4`  
		Last Modified: Wed, 26 Feb 2020 01:23:37 GMT  
		Size: 10.8 MB (10797283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea865e2909f355d736daef9076ecda63b3075c6267b858d9eaaf2e3966fc0d2`  
		Last Modified: Wed, 26 Feb 2020 01:23:36 GMT  
		Size: 4.3 MB (4340193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bf23912b71bbd038602cb98cf5207cb2183a8b7b49fa4b16fa2018e09f508`  
		Last Modified: Wed, 26 Feb 2020 01:23:52 GMT  
		Size: 50.1 MB (50070212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a979caa660cd9d6af7046930311c9ff6552995ed0f2959288617b472f85e4a8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.4 MB (106374822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc53296cc46bcd0a40f41cf4a1c433dcef27ac033ac1f6419e2741e3149af272`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:53:01 GMT
ADD file:5ed8e2bc0bf117a359d81b052913e99f6139d0b36e5798d75392429effd5afd3 in / 
# Wed, 26 Feb 2020 00:53:06 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:54:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:54:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 03:55:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3294d23573097fea5f2d79377bc86444ebf83e4bed50a8a6c62b7aa8637dd7fe`  
		Last Modified: Wed, 26 Feb 2020 01:03:12 GMT  
		Size: 44.1 MB (44066613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a952c5ec5882944f0e3977bb3d28960e53c97b7c4985863a7fd5b7c33b3a309b`  
		Last Modified: Wed, 26 Feb 2020 04:05:26 GMT  
		Size: 9.9 MB (9866766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b6614c3a732af22df2caaa8ead40737dc17a198f0ee9d057e6e53fee7f9f12`  
		Last Modified: Wed, 26 Feb 2020 04:05:23 GMT  
		Size: 4.2 MB (4159221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e937dfdc173e40ef43eb533cf95b65a5abf2a454023815cd5f3e958f46aa659`  
		Last Modified: Wed, 26 Feb 2020 04:05:50 GMT  
		Size: 48.3 MB (48282222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a6244a41598c2cb6eca87d2ce0349e239628dcaa54511a7e61831f73338cd86d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101909301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c262d0ccf6e9b59dfc08546710d4fc394f448b552af67d32bb87d59e741b055`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:59:40 GMT
ADD file:6497e2f777f4487d9221931005a8b4b81c021442a769b581e223cf30c81ff553 in / 
# Wed, 26 Feb 2020 00:59:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:27:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 02:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2478a2ed882cb5fbb5e4e92c9f580da9ca52f5fc78b8bb439ecbf3ac18023caa`  
		Last Modified: Wed, 26 Feb 2020 01:11:29 GMT  
		Size: 42.1 MB (42100335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c541086e0dffa72464d4077dcc60504a1c08a73ecec554c159269786ba08fed`  
		Last Modified: Wed, 26 Feb 2020 02:37:24 GMT  
		Size: 9.5 MB (9498391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf0f97b070f73118badb36d21af3459f8317d4ac6d45aec680092cc962f1c47`  
		Last Modified: Wed, 26 Feb 2020 02:37:23 GMT  
		Size: 3.9 MB (3918781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620eb05d9fd9184b8f200537b866a27af44aa6d7ef4dd6113bf1b51421d4795`  
		Last Modified: Wed, 26 Feb 2020 02:37:45 GMT  
		Size: 46.4 MB (46391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d3b1605a1695314d8d0723fd89d06fe206e9afe7f542f9f267bcc549656e50e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105025433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8051bc1ef46b266fbfd566c96a0e0c2195f54e441a67fd0210d58f2b6c67af98`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:03 GMT
ADD file:c82c7dc82c2eb3b50218c35e1b848f707b134d2df957f57125408f69aaeb9b96 in / 
# Wed, 26 Feb 2020 00:50:15 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:59:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:59:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 04:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:668c278237ef972312df4979c8fb1a927b38db5da09f094ae4fcc84a061dedf8`  
		Last Modified: Wed, 26 Feb 2020 00:58:30 GMT  
		Size: 43.2 MB (43158146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b41cac09012800692bd13a1238260bfb293c18c7864536c494809f2983ad770`  
		Last Modified: Wed, 26 Feb 2020 04:08:32 GMT  
		Size: 9.7 MB (9748511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094b353938273b0bbc576a8a80a232614ca2d9bfe48769641eee7055f3db6a5e`  
		Last Modified: Wed, 26 Feb 2020 04:08:31 GMT  
		Size: 4.1 MB (4094435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fba2538bf9e06bc84462d53d1effc13ecb38f026a6bc0df91cb9da3ffc0fb1`  
		Last Modified: Wed, 26 Feb 2020 04:08:53 GMT  
		Size: 48.0 MB (48024341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:dca603453ec745d005af586acc89980d68de5d5c06041b129714d2b6ed474942
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113078021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1cc1cf80504e751b9eb1a8181b294312257182c7c165f88070e847b80e4244`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:22 GMT
ADD file:f57292acaae4c3d7e8b3217b28f9efb27faef1c4e08ca95f4a25d1302355fb51 in / 
# Wed, 26 Feb 2020 00:35:23 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:23:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:23:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:24:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ef83ea0a858b11598fe63ce7d80a401ebb47c746763b35564bd712f013cb961f`  
		Last Modified: Wed, 26 Feb 2020 00:41:45 GMT  
		Size: 46.1 MB (46095035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa60bcba0a57a2662cae84d0bd1cc3e9baa383c9a1589cecbb68b4e65d231ce2`  
		Last Modified: Wed, 26 Feb 2020 01:31:18 GMT  
		Size: 10.8 MB (10818060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172f4142e9968e299cb42a03c7124d1456062e69197d3d50c972ca924d0d107`  
		Last Modified: Wed, 26 Feb 2020 01:31:15 GMT  
		Size: 4.6 MB (4561448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d299990640c71bf2446b454c0391fe405a3390c363cf97eab4f8fe9cd57e6`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 51.6 MB (51603478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7c51bb03b5a44b672abf28a3d70b8e48d763f227c8efe5052a22d61c6a65e7c2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110037443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738bf6a680e96eeb09d76dea039fc569771fe017d6f8b5565688521352a19d04`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:12 GMT
ADD file:ebcf4b112436fa7be8efa5ef204cc174c0d1af648c6ab4af968a71aa2ab2cf4a in / 
# Sat, 01 Feb 2020 17:20:16 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:06:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:072f803f12e35b1a40604b6081cb448d46529e3eb1d453ebbf56850c211f5bdb`  
		Last Modified: Sat, 01 Feb 2020 17:30:44 GMT  
		Size: 45.7 MB (45652299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1738f3141f5288b7d088c111ef5c0250cf1779363648e4abd0a2fa786691279a`  
		Last Modified: Sat, 01 Feb 2020 19:25:20 GMT  
		Size: 10.0 MB (10002083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a959eee44d8ac35abe99ef74efe938d0f14c75e8ba029451e3bb2f3c594206`  
		Last Modified: Sat, 01 Feb 2020 19:25:18 GMT  
		Size: 4.3 MB (4296690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c05296e9b4c4e064ac637742557d903aff58a97639760bb778595e90492a8f`  
		Last Modified: Sat, 01 Feb 2020 19:26:08 GMT  
		Size: 50.1 MB (50086371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:80033dd670892b949abfb0ded79a02ffe988eefa0208331622830af0e7237947
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110439429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806531e21f064fb9997ac1421538212affb929a0036b63fcc38098919d38f63e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:43 GMT
ADD file:17af4834ca99365d5ecf14eb938572689bd3c3ad5fd8a88da12c4c3474975771 in / 
# Sat, 01 Feb 2020 16:43:45 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:00:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb54e9d54b34d992a5c6582a6fe3836692cce3589a408748090bbb916a4cc63d`  
		Last Modified: Sat, 01 Feb 2020 16:47:28 GMT  
		Size: 45.2 MB (45241584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d13d85604945e95d31c38d488a822d8e0b84e7548a10db0c89115cca1887aa`  
		Last Modified: Sat, 01 Feb 2020 18:06:29 GMT  
		Size: 10.3 MB (10325358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596b324848b1286794120fbcb3c696328dd955db597ec3e70840b5dc97d794db`  
		Last Modified: Sat, 01 Feb 2020 18:06:33 GMT  
		Size: 4.4 MB (4372596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38645e5b0e6402c091627176f5aed8b9d434ccf323ecc4ca2c66f934acc1a11a`  
		Last Modified: Sat, 01 Feb 2020 18:06:45 GMT  
		Size: 50.5 MB (50499891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
