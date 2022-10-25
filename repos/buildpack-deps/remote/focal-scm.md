## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:aa83529c20e9637d81c8bb79ec8042bb08701d8e0aeb6700ce4bceddb07c2155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3fbf9b728805f4855a1e1714abd1122f590819c3c940af6add1e74b6edb1a583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100684328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:556eaf86e2c531f983516419b73441c5850909052e50ab552d75a9d7b29130a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:05:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215646fa628a9c18e31f7ea7321ae4140b44d69995ec4cdf3968cbce9a5c0b4`  
		Last Modified: Wed, 05 Oct 2022 01:23:38 GMT  
		Size: 7.7 MB (7747231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6c7ee6250b02a6cf0a3a3080d082e4ce4f858e2749921bc2623c896c487897`  
		Last Modified: Wed, 05 Oct 2022 01:23:37 GMT  
		Size: 3.6 MB (3624405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ce100b3517cefcb05b92b71a8c91e9881466e25f273c9ce8b59ade42ef3a3`  
		Last Modified: Wed, 05 Oct 2022 01:23:58 GMT  
		Size: 60.7 MB (60738241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ea745c791fe0fd9b6b7bf04130cdc270995b03279f2c411722ff840cd212ead9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89875111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddd42e22b4a80d23d5304ea494d56e753af1132c2869050e028ca61cc3f46c61`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8314cec2c7a441a36532dc89979b531fd7dab365416e8d4f077f16c6322a222`  
		Last Modified: Wed, 05 Oct 2022 00:59:17 GMT  
		Size: 6.7 MB (6740274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b75361ec0073f1728c7bbc9fbf5e55f5ffc978176453aaccd3f3097a710904`  
		Last Modified: Wed, 05 Oct 2022 00:59:16 GMT  
		Size: 3.1 MB (3103607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cd29b8c09506d2393921adb0cded05dba5f57e529ff475ad92160d2b38c475`  
		Last Modified: Wed, 05 Oct 2022 00:59:45 GMT  
		Size: 55.4 MB (55441138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:328e8c05b0f0341747f5871823ad81ae7ac6e958a44be976bcca059cc132912e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99237200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238b304b5e34bc73bb2557c4303d7a9380f67900d30cac408cfa2c46b7c6b625`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:10:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f7d42f1359bed862a992a062b3c7cf025e6bf6625dc1ca56ae2c66d7250fba`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 7.6 MB (7616212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc75acb9c1e02b10ddc3966608ccbac66c6fd9eeb3bff80797f9983f268a9b1a`  
		Last Modified: Tue, 25 Oct 2022 08:34:12 GMT  
		Size: 3.6 MB (3617606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d21db26b13141f20e7cce995a63f8234838277895d2d6d0e2ec4f35e659c78`  
		Last Modified: Tue, 25 Oct 2022 08:34:33 GMT  
		Size: 60.8 MB (60807384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0b5156fdea407f78ae8f5dd5a40c70d5686fd01e7a1316d3896a123aa5f2d1e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116020776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d728b216db5852c775762c0dbeb7021e76038e61147d6565e4df9ebaf321e554`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:29:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa48197ece6cedfce46328b98e2bd3ffa7f116e92dc0cd9aba21390a5edf11f`  
		Last Modified: Tue, 25 Oct 2022 06:54:02 GMT  
		Size: 8.7 MB (8705088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91159ec91712ffe519d3e9624103d9ec7b58e6b1959cad0b77145851e14fc55`  
		Last Modified: Tue, 25 Oct 2022 06:54:01 GMT  
		Size: 4.5 MB (4486836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c68813dea6733b577ebd8f432367b30fab9f0639692bc2e99d633f9347aff6`  
		Last Modified: Tue, 25 Oct 2022 06:54:33 GMT  
		Size: 69.5 MB (69528310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6e1c097aaa5b10d603b3ca7af97305eb87efa8eb846c6b08fea8968c3a45fe4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97967486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01cb9f67e31afed0eb376d14ac80a2758ecbb81e5ccb14b069d1b33c9da0399f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:37:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:38:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7f4256f9365e6546f5def4594e750767ee106712ba11997c58b0e9b15ab10a`  
		Last Modified: Tue, 25 Oct 2022 02:52:05 GMT  
		Size: 7.4 MB (7390068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c49cddcfee6d6315b4a734cc802ff8d05a8ecb16654aeca9cbd0076b7dec22f`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 3.5 MB (3542342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8b09e3088369fc4b7c4afe1c6fa3627b4a08b7f6388e1e455d9bbb75dbe837`  
		Last Modified: Tue, 25 Oct 2022 02:52:20 GMT  
		Size: 60.0 MB (60019048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
