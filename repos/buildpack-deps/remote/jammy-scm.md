## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:5fb13331b0ff8cec9ac41088dea866f962c4cea57746f9a6786b951973f6a8cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:52a7124440aeb68cd12e2cf204d86fbfecb0da0f4c7e3cea170ba3e02918fa82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77151035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d42f20418a32e6749f9981f745dacdc558edd5fe6925bc07a06a6dd7a6989a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:16:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:16:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 02:17:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bca3245ce06c5f92cf1528db00b152cdde37af4bf05c5d3976141dc4a704c5`  
		Last Modified: Tue, 07 Jun 2022 02:27:12 GMT  
		Size: 3.8 MB (3819557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7cdee01903ed192b91b97760507cc18ed88be4ff61e33e87bfe6f1944605c9`  
		Last Modified: Tue, 07 Jun 2022 02:27:11 GMT  
		Size: 3.6 MB (3559751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e140559ac12daaa563a0869b223a27cca33ef57ed3eac04f09c6c1f88d1da866`  
		Last Modified: Tue, 07 Jun 2022 02:27:28 GMT  
		Size: 39.3 MB (39348012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b7e1fbbfbf5e1bf5c8db230aaf94aec1d34933d23ba16c8fcb803b2a5cc64cf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76194989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5444563afcca99567b8ec3ce461196208eee4f3942adbe6cccf61ee8959b9f1c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:30 GMT
ADD file:78ae02cb00d8cc788584388eeb9fdc5ca6b45f502d33acd7f6efe7fc2a325683 in / 
# Fri, 29 Apr 2022 22:59:31 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:35:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:35:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:36:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a3411c136d8a6da4e9d7d3abcbfc94f59ecb2935fd02cad49be6a79c899fcaa`  
		Last Modified: Fri, 29 Apr 2022 23:03:59 GMT  
		Size: 27.0 MB (27015834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0fc400254e500236c1a1555f53101f3d136a6466afc02b601d41b663424039`  
		Last Modified: Fri, 29 Apr 2022 23:53:01 GMT  
		Size: 3.6 MB (3569862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff75e9c518264298a148cc4e8d868ef1588d3fbb3eb5a8f37dbc41d393fb89`  
		Last Modified: Fri, 29 Apr 2022 23:52:59 GMT  
		Size: 3.7 MB (3712399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac2f30de9b874657871112606d8d66e7b11892765a38c6fb72a160749dd932f`  
		Last Modified: Fri, 29 Apr 2022 23:53:42 GMT  
		Size: 41.9 MB (41896894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3a8fda18a50b93e11d586f6ba0c82513f2536ab7d24276e4d69229cc57da25de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74730994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93958bfd003d3f740e9dd75498f8820daa987d67b6b54272473add427e616d3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:32 GMT
ADD file:20805b983efd5443e34ebdfb7795010e5684eb1ca1ffea30a3e61e0089c0eee8 in / 
# Tue, 07 Jun 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:48:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:48:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 04:48:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed02c6ade914c2962413c1ad2ccc86ed8d1512098f2c87fe7bafa8e1b5293185`  
		Last Modified: Thu, 02 Jun 2022 08:38:25 GMT  
		Size: 28.4 MB (28378212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6155c325759d93f782b168bbc88964ddfe411faa203824e0d07cd6457fe5a6`  
		Last Modified: Tue, 07 Jun 2022 04:57:25 GMT  
		Size: 3.8 MB (3792707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408b3de6df6b01e21cd63f4825cd89fc1054971d120e93b8bba543d30f9ba68d`  
		Last Modified: Tue, 07 Jun 2022 04:57:25 GMT  
		Size: 3.3 MB (3319790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb57b0af2c6611fe078fe838912b55b6a8d86e9be30f71bc5fe11077d47ca3d`  
		Last Modified: Tue, 07 Jun 2022 04:57:42 GMT  
		Size: 39.2 MB (39240285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:eb73e93ae933bba13bc3d493271626cf5c510a2d2a2a25a02460581c0629fa47
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77229577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db9acb80252960587fbab9540365e07b254af741cab169a74ecccce7d3602e9`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 18:18:50 GMT
ADD file:d19287898059e2e99fffa362a449097aaffb132af21a1d1e72c5b898ff785df6 in / 
# Mon, 06 Jun 2022 18:18:51 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 19:31:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 19:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 06 Jun 2022 19:36:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1edfbf9ed16b67ab57bd93f6b8aa57ec157383c958bd3e39e94cdac02ca1db32`  
		Last Modified: Mon, 06 Jun 2022 18:41:31 GMT  
		Size: 27.7 MB (27745919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0b2b247adbcda207142d115c60814f361a65d9e79b584f05cf2c7ae16de140`  
		Last Modified: Mon, 06 Jun 2022 20:28:14 GMT  
		Size: 3.6 MB (3614448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e32164a9b5dee9bb43c693f8c7c833ebe435e4b86660f7a14ce30decd26898`  
		Last Modified: Mon, 06 Jun 2022 20:28:12 GMT  
		Size: 3.8 MB (3776968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26beb173e0f45f69bbe4fe18a33e9aac6ddee5f7c6e5cf78b1a639f7dcc4b1f8`  
		Last Modified: Mon, 06 Jun 2022 20:30:26 GMT  
		Size: 42.1 MB (42092242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f36c02b2846a404c52f3c3f696313b35cfdea715623c03961573f6d28758805c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75203852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63b1696a347707fb9dd7272486eb84ed615075c40f8dcb89c2123db639c10242`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:41 GMT
ADD file:5412b0d16961079a78b96411ca23f1838ac09c2fae839829476380b5389e49f8 in / 
# Tue, 07 Jun 2022 04:05:45 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:57:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:57:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 05:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6fa1296f44090f6150dfb96d6ae217a58b9d66c56d7a986c35657df6bd1a89f0`  
		Last Modified: Tue, 07 Jun 2022 04:08:13 GMT  
		Size: 28.6 MB (28638482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c21ee3fc0eae5db8aa29b016cfeb4872fbed236a180eb98f9c578ecb1d24f1`  
		Last Modified: Tue, 07 Jun 2022 06:09:06 GMT  
		Size: 3.8 MB (3821587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869606af1d12204312dc361122a3664437ee80f9a31ca39e0f6fc7c7b9ec5e7f`  
		Last Modified: Tue, 07 Jun 2022 06:09:06 GMT  
		Size: 3.5 MB (3471029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b22c031773ee8c006c6f8ba28c5b47a56d9db4e2893420c8cb9b167662d97b`  
		Last Modified: Tue, 07 Jun 2022 06:09:19 GMT  
		Size: 39.3 MB (39272754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
