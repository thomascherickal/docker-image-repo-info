## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:7dc276e74f025b3af240b3a8fff199627289228cffc79efe80a0e3cff4bd627d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e7b8d9943c94fc6333a924bcc9de7ff4ff1d34e10f640887d16876101d5cdc33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40401000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c36b01b6848b7fd0fdceba8ad6a65fce3ac3d71c8c8ad1d00942caa652de1ee`
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

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f320613ba1d7b2771097baa1d8e99aa968101c2feb155c988d1a20fc1148b4eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36357576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:918e66aba4663b918d2522684025a797f83ce509165f90cc93d5cdb326e1111c`
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

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eec4fbde5aa9e285993e14bf40a5397efb7981a7cac82e3487e7d7c854f627f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37903519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c94e0002a6bf3647e151a39f159ad764fceda8aaa09ec82f5c29126dd496da7`
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

### `buildpack-deps:kinetic-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:cd57c861daa5ed632626b780bae8178cd23d049f9406fdb9671b3c47f531b888
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37192090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e72178111e81a32c8cf91a756f37762dda8f9e995cf213a9d2f879ad7681e6b`
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

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:507f03aa1361659990ee30202616c9304dfea3c84ef8edfe2fe20bda7e36a6a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38200719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b619eaef60c9149414ebe593e29e26f1f10f900103d7b68c86f16e9c1603f81d`
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
