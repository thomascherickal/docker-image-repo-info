## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:1522c1db2aae4e9414d5b7bec256e9eab0b1f31f77b82f87ac32e5f7dafe4a2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6c1872f4ea21628b7c323305593b94d6ecc5125852b4a03827c6d38b473835d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125631181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e73278505bb143c007d79f686483ae493b77ad2ad4f7cadc67deeb86f4dd38e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:48:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ad072f9cd16fc8eb93b182b20e758e11acc0ef60babef0bf1043c08de1901a`  
		Last Modified: Tue, 23 Aug 2022 00:55:57 GMT  
		Size: 54.6 MB (54584135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f544bf2e62950527f9e904a056de2ffc7f7d57a0051cc0a83f53029d715f2847
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120512626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254098229367b0e03446fdc4d0858c497972184186719e50d9853daf38a33bb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:51 GMT
ADD file:132abd62c4fa546798c96d5b1f6f409de9ee27242caf6c479d65309b764c3ece in / 
# Tue, 23 Aug 2022 01:16:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:19:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1918e2afd901ca723b3483d8d521789daac45ddbaae2bf9fd813933e826f39b4`  
		Last Modified: Tue, 23 Aug 2022 01:22:10 GMT  
		Size: 52.5 MB (52547848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a58d3f469ed5c6be23bbc74a836bceb306e58e8cd5e58e4464c2b23519543a`  
		Last Modified: Tue, 23 Aug 2022 06:26:58 GMT  
		Size: 5.1 MB (5070690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61379bcded34629fad0582d1d42f2cba36b5f418591509e15301773304e7c7c0`  
		Last Modified: Tue, 23 Aug 2022 06:26:59 GMT  
		Size: 10.6 MB (10573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c872e375903a379cc5ab82220655ab6973d82f8b48ab51b42d197a4ab189b6b`  
		Last Modified: Tue, 23 Aug 2022 06:27:30 GMT  
		Size: 52.3 MB (52320330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:495a7139ac1f0b677a9476288d454f9dfd4763312ef4dc4d467ce3f29c36caed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115696134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e362c69b51c9b48c55b381399fc2b7a49ec81e115a633a60638b43084b817c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cbc350f4a21916bb6fe70920c962a4889a5059aee86258e4d8263f0c7afbef`  
		Last Modified: Tue, 23 Aug 2022 13:12:28 GMT  
		Size: 50.3 MB (50342476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5156f3bb278fb0dda42cdf0b406331f8809ab19a049e6ea5506665811c002475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123973338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf31c8a1856f38bfa1a001f3b72d3e9678c5aadee3ec10352d90f571361e1fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db608c3c3ce3568556faf63acbc2069811afe242faf8992ccf0ab1986ee38e4f`  
		Last Modified: Tue, 23 Aug 2022 02:37:07 GMT  
		Size: 54.7 MB (54680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1afc200fb3ee2b4b85c5c984fbbc088ff53286077a843588bc04c935cd6b7416
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128053909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bceeed6ce487fd59052390091c5f4300ff05ada27c1650c1dbf83f91a4d9788b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:24 GMT
ADD file:4012c41187a03bdb3d37bec80f6255a1d46582e3ed145b4f313e42196529e524 in / 
# Tue, 23 Aug 2022 01:02:25 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:32:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f683b9c66ef80b527ee5e4cb11969c6e0c1400ab69a4f1279af90f5766d70c7`  
		Last Modified: Tue, 23 Aug 2022 01:07:53 GMT  
		Size: 56.0 MB (56012624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f506948c8aa6d2e0693b583a388ce5e10b4393763bd2ea2529af3bfaa07f0c92`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 5.1 MB (5085725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915cb3138c0c978b1806934d3f979cff24ecaed321fe7e13caa292cf9ca73dcc`  
		Last Modified: Tue, 23 Aug 2022 01:40:01 GMT  
		Size: 11.0 MB (11032841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc001487b6a15d61b32ac2dbd4b06bdede894077b8fcd3fa2f3969f98052bc3`  
		Last Modified: Tue, 23 Aug 2022 01:40:24 GMT  
		Size: 55.9 MB (55922719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:f77a6a7b17a830e7b62d5efe2289fb42f472a239f233bb3ae4c8fe4c471696f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122351812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4232923e1b46610a8a651c7103d3827310fd9f9924b997a6024c31adf7b888ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:09:59 GMT
ADD file:d4bcd76354f6ce92e52e206333ebbe2399c24e2ee5b19ae5f758b25dbda35efa in / 
# Tue, 02 Aug 2022 01:10:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:53:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:54:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:55:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b6232334ba5947043903a2c95b6b7c6e6b613d66b10b9cad82702032585b0d8`  
		Last Modified: Tue, 02 Aug 2022 01:20:18 GMT  
		Size: 53.3 MB (53263487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77db3f931ef8e6c6e59d3af4773381ee1557b70b35c21e01543324bf664e132`  
		Last Modified: Tue, 02 Aug 2022 02:24:11 GMT  
		Size: 5.1 MB (5123478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cd018f526c1a738a2f7b90dbeb1439a31059e66e9d09c98807c316b6c72e1a`  
		Last Modified: Tue, 02 Aug 2022 02:24:13 GMT  
		Size: 10.7 MB (10660940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35e4a84a02a342bcbd6764be5e369e4b07630db2011302157f21d32c41a72ef`  
		Last Modified: Tue, 02 Aug 2022 02:25:04 GMT  
		Size: 53.3 MB (53303907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cb31310b3598fc3d3ad9daa40df9a133a6e2e360aee409d29191203c4686d095
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134816917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30881ed3045278b91be936aafc665ff71cd8bc93d39d8b69650de485729b3d02`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:30 GMT
ADD file:c498f58d8dc50a2a20679642be8f6f43de8b79455438a1c237ef4c94a9ffe34c in / 
# Tue, 23 Aug 2022 01:24:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:58:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62d01a7bda469557451a05bab1d4de7f53dd936e8032b36635019fd54cd927e4`  
		Last Modified: Tue, 23 Aug 2022 01:29:57 GMT  
		Size: 58.9 MB (58909173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b002340b938f821f3b0978eb9bfc47d2b8fe91b33c50508bd618c3c4b0ffe0`  
		Last Modified: Tue, 23 Aug 2022 02:10:43 GMT  
		Size: 5.4 MB (5412576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c65f43f4fd248e0fd18c35535f21fcafa740bdde05c5c367f32926f478e55f`  
		Last Modified: Tue, 23 Aug 2022 02:10:44 GMT  
		Size: 11.6 MB (11628949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e7f52d8f52b4e830cdd20f538730eebe893f6c1f11aac1d0457ae132da2e8`  
		Last Modified: Tue, 23 Aug 2022 02:11:16 GMT  
		Size: 58.9 MB (58866219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fe781f689e6f87bbf043328a5546a3c8810e4bb71bf4aace341aa84bc8e2aab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123246645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd05daa086ec2eb9eb0d8724cfebe627e1a621d31c39e41c49c480e60b4413fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:53:42 GMT
ADD file:799d2eac4bf12dcb56eca0b771da879e8873a2a81b4d74520db7d6665d448ff6 in / 
# Tue, 23 Aug 2022 00:53:45 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:51:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:51:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e8428caa8cb9dd5cd48266f588e1d935181b0d75e5f4680a9d4d03700d44289`  
		Last Modified: Tue, 23 Aug 2022 01:01:15 GMT  
		Size: 53.3 MB (53279185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b41fe9abb9a7707d3bfd9881e997384ad70ba3f811c4152a16e11585318bd5`  
		Last Modified: Tue, 23 Aug 2022 09:59:58 GMT  
		Size: 5.1 MB (5146782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215c1024f20ea76e1b536fcf226d87a639e72806443621a0bf52a719c0218fd`  
		Last Modified: Tue, 23 Aug 2022 09:59:59 GMT  
		Size: 10.8 MB (10765873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeff4b644e5176d180f566f9889b6ed12e443f2fb955b119865cc113d26c3b1`  
		Last Modified: Tue, 23 Aug 2022 10:00:19 GMT  
		Size: 54.1 MB (54054805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
