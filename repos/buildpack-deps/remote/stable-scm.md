## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:663243bb7eca71a92623eed866eb8809900033c80ccc58a0bee88cec1dcfdf6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:stable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5f78634045e9ac71575c660cd2b6d2d6302156e6107280bede466f495ee1c465
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120104805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:249b31b759d78ac17066cdaa7a0e4ccd60c4eb710bec491eb15a6c5bab17872f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d943ee54c1fa196b54ab9a6673174c66eea04cfa1a4ac5b0328b74f066a4d9`  
		Last Modified: Wed, 12 May 2021 02:05:07 GMT  
		Size: 51.8 MB (51841468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:90394a67a091f9429735fed2308a099635fe630fdf1992c53b73739f021a755d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114789736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9da08e3fad951e330e87ed53d42c01177d59b24c46a946cb4d7106d3084d918`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:54:57 GMT
ADD file:443be99157e29a4ccb29f5d0ffc9994ce41fb51c512815f76fec9e1fb4d5d8ba in / 
# Wed, 12 May 2021 00:55:00 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:28:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:28:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 02:29:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db69af0c9ce605b61ac30d118d6c6ab4f8579b8c80e5469335f2108afa5d2c66`  
		Last Modified: Wed, 12 May 2021 01:09:52 GMT  
		Size: 48.2 MB (48150747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47203fcc2d787900c2b29557537f54bfb4736cf95aeb1da72a4eb38afe48002`  
		Last Modified: Wed, 12 May 2021 02:46:08 GMT  
		Size: 7.4 MB (7376669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8503ed6a21cfbc9d6bdac105da9df47ae10adf0aca8c5a0156725d84e6802879`  
		Last Modified: Wed, 12 May 2021 02:46:08 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2744fe63b86d7edc936ed85b2f71f37b3cee4d397d3310cb8189317b6b365da9`  
		Last Modified: Wed, 12 May 2021 02:46:35 GMT  
		Size: 49.6 MB (49574780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bf7c9aad80681044ee4e4f4f8ca4e2d967adceb2d4e0d7571cd32d6f0fbe7dfb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109741295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de082dfef0a27f616c5bf0ab1c4aff09528688457c90f470f2884366d86df51`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:02:10 GMT
ADD file:51a0472692adf18117444dc1f35d6eb3b4d6d672f28a7f6631f9d5d269b0b85d in / 
# Wed, 12 May 2021 01:02:15 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:40:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 00:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89475607b1df9fc7eec7efe2fa845738a16cee3e92c1bb864c1f5a93b8303bc6`  
		Last Modified: Wed, 12 May 2021 01:18:49 GMT  
		Size: 45.9 MB (45916922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88447de5eb3eca4a1d96b6980b44d82ac19d121f6b77b826989f8d611fd001b0`  
		Last Modified: Thu, 27 May 2021 01:03:02 GMT  
		Size: 7.1 MB (7124249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25b14665fd0185f2f3b90a8d1825fc8ef9f330e1aea452f60fd70cdcfe99bf4`  
		Last Modified: Thu, 27 May 2021 01:03:02 GMT  
		Size: 9.3 MB (9343721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba65a331625e51ba8f0e1af07dcb97c0583204dda094b5da79672fdf554129c4`  
		Last Modified: Thu, 27 May 2021 01:03:40 GMT  
		Size: 47.4 MB (47356403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:00a68b1a4dd545b9b9e64435583071ec3c1d0196d77f9304863970c9b6708518
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119073182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56611d1184aad42d38e0690ec2b3b52465dd93d774f670a02f4c6b662867a239`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:50:48 GMT
ADD file:ff9983cd659b3fc32ddfbbdeda76a971afd7d399e6d8b98faea3a9ead0e598f6 in / 
# Wed, 12 May 2021 00:50:52 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:34:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:35:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c54d9402d498e45ed396b5b6fe836f55e4ccadbad745decda3e9f83d880bc677`  
		Last Modified: Wed, 12 May 2021 01:01:40 GMT  
		Size: 49.2 MB (49225351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91bbb3592d6685d1c683c8c20e60901274c636605800608685274c194d43d25`  
		Last Modified: Wed, 12 May 2021 01:48:24 GMT  
		Size: 7.7 MB (7695057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d8c28b9129321858810cff4cd78385949579ed18d991f98c77f912c7a754f8`  
		Last Modified: Wed, 12 May 2021 01:48:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b3803033bfb8e0c8ab31f286ca427ccb8a47b7c63ca8e6d05d23ff7231733`  
		Last Modified: Wed, 12 May 2021 01:48:46 GMT  
		Size: 52.2 MB (52168431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6ca745145db70f9e429061f2a9eba3c1c202b43d363b22f4045a2a50decd90b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122976612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e242712fcd64ab04f5bfd1dafdf1a105828ff6844e9e9ae95ab7f9655f0b3710`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:39:33 GMT
ADD file:f823eb487fd44688b29f866d2c837da27f508db7fc1f19e4dc01dde9ea7c72c4 in / 
# Wed, 12 May 2021 00:39:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:09:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:09:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:09:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07a4b6b1756691e1f8a89eb64afc18fb9b4a0712eb810679a4b89b1b351f8e9b`  
		Last Modified: Wed, 12 May 2021 00:46:03 GMT  
		Size: 51.2 MB (51200034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2395b55871bdaf1f7143048f77c63000ab6412664b1ce49fe9a8602e496d1`  
		Last Modified: Wed, 12 May 2021 01:17:52 GMT  
		Size: 8.0 MB (7998534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106083f164cc6c516cf3c838e5ba0c6870172a26217bd766dac43b0ecc89ca3b`  
		Last Modified: Wed, 12 May 2021 01:17:53 GMT  
		Size: 10.3 MB (10339817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfd96379aaff5d0e0fbcadade17bc6dd9c9fce6e229d06bbcf028b432ef82d0`  
		Last Modified: Wed, 12 May 2021 01:18:19 GMT  
		Size: 53.4 MB (53438227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:dd1358affe8a5d0ae4909382e78efdc12c23388dc2d6c1f52cb3dfcf83cf24ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117196042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c565c44ce956b44f47142f4604e5c99cab1c2e4bcfd86adf060bcea4c5eb59`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:09:17 GMT
ADD file:2e2c1e52b19e85e4299309ed75f088e727e316902a0dd39be198c41ced817b01 in / 
# Wed, 12 May 2021 01:09:18 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:58:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:58:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:59:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e18ab78f0b7ce048045ffb547791aaa698db3869d1da87f71e538a7fd19f965`  
		Last Modified: Wed, 12 May 2021 01:15:53 GMT  
		Size: 49.1 MB (49081826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03651915a251d4aae832ea26b7e72a8d93c3b7bde9b9b309c4069e8de71798fe`  
		Last Modified: Wed, 12 May 2021 02:09:54 GMT  
		Size: 7.3 MB (7252462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc21a03fe417b31a222d86e092660202cc0fae5556a43581e06b7d6a7ae1849`  
		Last Modified: Wed, 12 May 2021 02:09:54 GMT  
		Size: 10.0 MB (10016363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0e8057c7976180c1276687f493d7ba1a8ef256364c51e7c518c539f03b9386`  
		Last Modified: Wed, 12 May 2021 02:10:45 GMT  
		Size: 50.8 MB (50845391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6d2705d2c090f05c0c67f96c4d1b0d5d664c1ecd38708f242b7cd74e1cbf9896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130636742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c86fe0f1b611a98dbf6e8d6d9daba41d458365c9e62502c681b7d5774f6ea5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:34:15 GMT
ADD file:b714397b44737108500b0256abc9750626cfa28cc0bb52623b9a14bb0e2345fc in / 
# Wed, 12 May 2021 01:34:24 GMT
CMD ["bash"]
# Wed, 12 May 2021 03:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 03:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 03:42:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd4ac1330adf594df6c60d33ec5060c79833a8455e6cdb9f5ef2be33cb843845`  
		Last Modified: Wed, 12 May 2021 01:43:19 GMT  
		Size: 54.2 MB (54180124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb8ec8ba72b4c906c6a3b88324130a605cfda687a94ed75e901c7cd141492fb`  
		Last Modified: Wed, 12 May 2021 04:19:32 GMT  
		Size: 8.3 MB (8271865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46415d7d07194b30fe4845342dd9c5927deb73698c2cfe9a55c6417b98ed3855`  
		Last Modified: Wed, 12 May 2021 04:19:32 GMT  
		Size: 10.7 MB (10727703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443c274997562dde0054a5cc26e8bbee59190c34ea8b862e917569cfbee85b63`  
		Last Modified: Wed, 12 May 2021 04:20:12 GMT  
		Size: 57.5 MB (57457050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a4244013a9f7d4fb1f761bf673ebf22907cf0718dc8228bef6d96500defcd26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117665179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88823dd162ad3c648aefafc0121ce17b2a55b3460f6fe16a82fdfe3e91300772`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:43:13 GMT
ADD file:ffd730820ba7e4874e61b094cd8b1b19e272722efa2f96b6c2c0518882aa8010 in / 
# Wed, 12 May 2021 00:43:21 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:24:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 02:25:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03edb521c4b9db23cdd0bda14609ccca13d11f4c37cd9ca16173028e6d3647df`  
		Last Modified: Wed, 12 May 2021 00:47:45 GMT  
		Size: 49.0 MB (49000941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34f82527bf298856cf45773644d350eef4edbbc31c0abda7c268dfbe472c46e`  
		Last Modified: Wed, 12 May 2021 02:34:40 GMT  
		Size: 7.4 MB (7400573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7314687ab69ade4e94423968ff75eb3a6f047e5e53aae12aef126aab10da1d3c`  
		Last Modified: Wed, 12 May 2021 02:34:40 GMT  
		Size: 9.9 MB (9883275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a664f010e5f184251905b6213d5a3762e3d48b827a06000350e3463ea6a1cf53`  
		Last Modified: Wed, 12 May 2021 02:34:56 GMT  
		Size: 51.4 MB (51380390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
