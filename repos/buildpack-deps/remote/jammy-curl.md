## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:62cbd856d5cd76dfdb9a87befa2905e454b04bd0d7e2ff41f8eec078e0191809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c9333807db1513b0154449a0d36bab76873b485432e013e734419211a1054dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37807749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:900513d4f9365fb0c9c53639f83dff22f9a369275dc0b8a7c1e4e91cc80c5133`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:05:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aee672653a887d233e46702a755dc9d0bccd131595737ee8d74630d576aba9f`  
		Last Modified: Tue, 02 Aug 2022 02:24:14 GMT  
		Size: 3.8 MB (3821068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956655cf581c3ab1ff5e6a995a7f429fa35118f6afc2d93ade8082cf0d0196fd`  
		Last Modified: Tue, 02 Aug 2022 02:24:14 GMT  
		Size: 3.6 MB (3560545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dd3bd02cb06b00a6b0e05290d62dfc04f462a233d96b82fec29f39be0585b5cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0783d26fd063b045a6a6d1ad7484a25a49f96420d15956b66d9c6a1fdd8f06a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:56 GMT
ADD file:1bec4ea562c9a42add30f5e3626edc93bdfc0271cbd208a4447842fa31b5c114 in / 
# Tue, 02 Aug 2022 01:40:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:58:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f1a5cf9a21e485b0a676c22ced0e80a140055b3ef0d7573caf5be408a10ddb04`  
		Last Modified: Tue, 02 Aug 2022 01:43:32 GMT  
		Size: 27.0 MB (27017015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7f5e1bf5a769b4cdcff0e4f7232bd3bf5f7d07c3f23ff030f74cf0abd24053`  
		Last Modified: Tue, 02 Aug 2022 02:16:37 GMT  
		Size: 3.6 MB (3572129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fd3be308fda95edf60931006bd4d3432d41d1a26e5942a75d3f6e89282df28`  
		Last Modified: Tue, 02 Aug 2022 02:16:36 GMT  
		Size: 3.7 MB (3713550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:46fc6e142336fbe53686a9b32ce2588ef1d88236df5f1d28f8a010c9a37af054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35495544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0b8f89e44d753f137abf471fdef52e03ea28cb68bf54efeb4813576f3fe06fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:35:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6de042cb869a25eebdf68de514b4450f82c38b9cec853a790e0bc12272588d`  
		Last Modified: Tue, 02 Aug 2022 01:50:49 GMT  
		Size: 3.8 MB (3793545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efd2a11a62cb05975c115b200176aa1783cf879e07bb4ee462cf161275ec087`  
		Last Modified: Tue, 02 Aug 2022 01:50:49 GMT  
		Size: 3.3 MB (3320844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f90616501e56c0a29c314b116b5b9ce5f53aa9e7a0d42ae9b5c753c919d3e39c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44241852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1635ae01ceaf220af350d6734387396e2064e26580b565afcc09d0e6bfcc5659`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:53:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc064b2f92ee9486c5aff9b01b6c4e03b1dabb079057e9522378da6a679d656f`  
		Last Modified: Tue, 02 Aug 2022 03:23:01 GMT  
		Size: 4.3 MB (4290202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85366274834fa0723d3cae9a97e7aa88f9e031aa2c26e64e8d90d3650c2e978f`  
		Last Modified: Tue, 02 Aug 2022 03:23:01 GMT  
		Size: 4.2 MB (4233646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c6ad1add8cb3fa694c527514c6e4afdb648c3d33e315b5071a3e8ed08818625a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35137886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f125b7ccaef6f830a208658480ad1517b9649846f985e6cc3b2d580518f72f01`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:12:34 GMT
ADD file:79d1b21ac7f3117a8618b05cf302417041f08d563c40c792234fc75f5fafa46d in / 
# Tue, 02 Aug 2022 01:12:36 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:31:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:71a79c3e49d550d7ae02dc0996ef9523f40c8b7e588399426ab3347a34debd75`  
		Last Modified: Tue, 02 Aug 2022 01:30:03 GMT  
		Size: 27.7 MB (27743985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c93a051f5891403eacd9235411422b7cc7f9c234e0bb239b42ed226d36df82`  
		Last Modified: Tue, 02 Aug 2022 03:27:30 GMT  
		Size: 3.6 MB (3615912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e645e9ec95a1ceb6899427992b9198e35739b358c01fec10abcdcaa731490c`  
		Last Modified: Tue, 02 Aug 2022 03:27:28 GMT  
		Size: 3.8 MB (3777989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b85663e126adfe687ce37f1afab4d1665f7942d4d0775b95aed12ba73ee945bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35937997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:963ef58fce755092c7abad54c13bf5addd8bc0834c12138f917672e66da5ea1e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3f1b5666f8b3207bb75caab1dd328b04374a37a1d6568a5a870f2e893cd488`  
		Last Modified: Tue, 02 Aug 2022 01:39:39 GMT  
		Size: 3.8 MB (3823523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d904f2efab931c8317caa6af484cf95df9e6cc7e721574cc2a67fa999822e39a`  
		Last Modified: Tue, 02 Aug 2022 01:39:39 GMT  
		Size: 3.5 MB (3471689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
