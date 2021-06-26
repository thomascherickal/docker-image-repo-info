## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:d0f3be2edb2053be5d03cf74d5b40a88950cebdb232231730357bcd742981194
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `buildpack-deps:impish-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:152fd955ae787f1e073d39d8f8a748d0ce78fed3bdd5da844ae2600313faedda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40865721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b42b2f541e72e6c32b56d57c287e2f3361bcc18ea478dcdbdc3d733cf44569`
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

### `buildpack-deps:impish-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:333dd92402cf72a97af135cca0311596f682ea09d9188cfa6f9fc76868819bd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34881570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dd7613de9e66cfb0e1960a54af1efa6939be9c8aef5254edc6e0814bd7196ed`
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

### `buildpack-deps:impish-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f2fe4f5fc41fbb312732dd310eab2560c3946309f1195f0d410e2d1398dd0807
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39240317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96cb8260e5cd9d34847dbc8374da2852e4f293efca698527ca3a8ddd02da072a`
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
