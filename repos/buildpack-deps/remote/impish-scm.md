## `buildpack-deps:impish-scm`

```console
$ docker pull buildpack-deps@sha256:52a74c14a7d4f66ed85fae2e0e77f2d1cc06d3f3facc40617137c9b2fb914448
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `buildpack-deps:impish-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7319832896e926184815c22defe7031ecdc4e2a64a35fc30e61e4dffc5fd3e6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.7 MB (78742622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:948855c3898acffc9373d4d4a43be0300cc8eb82948ba6447f467fc4b9f4572b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:51 GMT
ADD file:d46db76c3e6118cdd3e7517ae171c3b5f2d8fb27f0a0469fc171f4a68a7cd058 in / 
# Thu, 17 Jun 2021 23:31:52 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 21:49:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 21:49:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 21:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba6f9ad033a8ec51e800f4c8157a07034acecee60eb6a809353f4a0411de697c`  
		Last Modified: Thu, 17 Jun 2021 23:33:52 GMT  
		Size: 31.8 MB (31762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6186c8faaedb0c6583e16b34c24317d8de3e75aa17c9c4ab4d3a0f31af2cf24`  
		Last Modified: Fri, 25 Jun 2021 21:54:40 GMT  
		Size: 5.4 MB (5445270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4885d7393d4d2b1d917d8b062bc2ec2c28b9668817c5219bf7ebe7d386c084a`  
		Last Modified: Fri, 25 Jun 2021 21:54:39 GMT  
		Size: 3.7 MB (3658326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4724ed0deff0cb3007f5a64add146c0365716b8f25cf45c86592b014b205b7e8`  
		Last Modified: Fri, 25 Jun 2021 21:54:57 GMT  
		Size: 37.9 MB (37876901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:91056fbfba72e72a0edca9b83b3258191a15ef3577fd732e6c9f4049234d872b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74937813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c49cfa25f964b20373e81d3f813af284d831fbc1d8ba8102a5207b1cf70a704b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:42 GMT
ADD file:fa5d0f84f67854e01718ffd2b64fc816b3c41ac044ab600cc24faa10d1727b08 in / 
# Thu, 17 Jun 2021 23:32:42 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 21:43:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 21:43:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 21:44:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d03567d42541920e4a880cc689ddaf0880486fcb60beb940f50ff08bdf05a812`  
		Last Modified: Thu, 17 Jun 2021 23:36:11 GMT  
		Size: 26.9 MB (26871009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2651b8ad64a7be0a28b5db143766f0453101bfdebf5ba07d071012e6eed0f33c`  
		Last Modified: Fri, 25 Jun 2021 21:54:12 GMT  
		Size: 4.9 MB (4870552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adff242982597f117700262ba88b6e5f5d40b47c76dccfa9e5b6db338d09d7ed`  
		Last Modified: Fri, 25 Jun 2021 21:54:10 GMT  
		Size: 3.1 MB (3140009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e7ae7886ce4b5ba39f548492ae13778d625a8364617ea839be9cb7003f23e`  
		Last Modified: Fri, 25 Jun 2021 21:54:54 GMT  
		Size: 40.1 MB (40056243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b6dddd2d255394ea75006ee774add7224b4797664935fd7b7f3728ea6302043c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77110178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f148d9e26b5036eaabd41ee20947a6958fa4266007259f75c72ea54534bde21`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:24 GMT
ADD file:8ac53c1ed01a99cb2109d1635ccd3777f060dc9fb3daacd9f1162e184c8d2af6 in / 
# Thu, 17 Jun 2021 23:54:25 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 21:56:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 21:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 21:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:007f70680acb7b29b5067e2140245788893cb101a0ba9167f7075492ee7d3345`  
		Last Modified: Thu, 17 Jun 2021 23:57:08 GMT  
		Size: 30.2 MB (30190470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043f54485c70a1ec6bc6d93ce2eb52a6b042d1d3a961ed6e3bd06543191f8376`  
		Last Modified: Fri, 25 Jun 2021 22:02:05 GMT  
		Size: 5.4 MB (5413697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8770895b2bd15458ac266140143b5bd14ca3f5c76d10037417e0705b33e106`  
		Last Modified: Fri, 25 Jun 2021 22:02:04 GMT  
		Size: 3.6 MB (3636150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2767d4151d5892e4d979d4c4956377a58713490523a5e1dfdb2d34bc4b9d3933`  
		Last Modified: Fri, 25 Jun 2021 22:02:24 GMT  
		Size: 37.9 MB (37869861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
