## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:abf630adcd1a7b66b008cb9a2b2bf1d57e97450b6937aecf61c18e27060dc04a
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

### `buildpack-deps:bullseye-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:49252a72ee7f580fb65beebc0cf02c40ad522a3d63c24632775028b307978246
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123988381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c94910fce9b566b875b840fe5c9675ae253658da46254f02b0ca92654698775`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:3f67740cbc1b7fefda4dc75bd2c0f0e76df9ae6b845f37b33cf8eea958403b6c in / 
# Sat, 28 Dec 2019 04:20:39 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:45:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:45:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:45:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f64e5c246a10532414f3b69dcf620cbf27337d8900089f4139ab3215186e02f`  
		Last Modified: Sat, 28 Dec 2019 04:25:14 GMT  
		Size: 51.4 MB (51358861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a40087c7676442e3d13e8a213aa17fb44a1cbab4d952197f09edac463f58edf`  
		Last Modified: Sat, 28 Dec 2019 05:00:44 GMT  
		Size: 7.9 MB (7919349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce8ee259aabe18e11221885897dc3fc3f8081c56a276bef858633277e6384ce`  
		Last Modified: Sat, 28 Dec 2019 05:00:44 GMT  
		Size: 10.2 MB (10182884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2980bfd4fdb4de40a047bf0530bc098ffcad6342b5a5b8ff22be79ed73e190a`  
		Last Modified: Sat, 28 Dec 2019 05:01:00 GMT  
		Size: 54.5 MB (54527287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ba952191b842e5d5c8c3676a63fc89856c723b86b6a576015fa77eb42690b0c4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118813413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:343ef0993a9dc46085b6204a84284858da3ea85c2488f19b081e95d544d25a72`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 12:12:27 GMT
ADD file:2baa1f0574c2834ad17d2f76e28f77e533c06686ddf3e7cd093dcb4c72ae9942 in / 
# Fri, 22 Nov 2019 12:12:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 17:17:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 17:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 17:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c41680389ba4d76f3e046357090c3c237888674b176f2ed957bbb159706f221`  
		Last Modified: Fri, 22 Nov 2019 12:21:10 GMT  
		Size: 49.3 MB (49268003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc981530e6b8edef7874ba6212f5b9cce279a30e51b2c53295a4e4d2571adb1`  
		Last Modified: Fri, 22 Nov 2019 17:44:40 GMT  
		Size: 7.5 MB (7509588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3cb96c42f91b6aa679e1b44ac84fbecb2cd38d5efc5a37efe1ccd33f65c7cd`  
		Last Modified: Fri, 22 Nov 2019 17:44:40 GMT  
		Size: 9.9 MB (9877224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca1175690ee1994c038277ea737404281fdc2e7d51a3cd1007f12c2485aee5`  
		Last Modified: Fri, 22 Nov 2019 17:45:06 GMT  
		Size: 52.2 MB (52158598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:136cdce6bd211740a9c3b86d3bac7e777cba14742e73f030d5b3a5a6815a2bfd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.8 MB (113824980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029a209d3952cfe7d8c0a086d9db6dac7e01d4cd782a6be779e762583c82137f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:21:14 GMT
ADD file:c9fbe61f7ded389c614d7a2dc7a73db387e5c89419aab9b0acdf46d39fb6cb04 in / 
# Fri, 22 Nov 2019 13:21:15 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:05:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:05:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 23:06:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7829ca4b083805aed02c7dff13add2b8d98f2f2acc202324179e6b3fd2e8e8b7`  
		Last Modified: Fri, 22 Nov 2019 13:32:22 GMT  
		Size: 47.0 MB (47004823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa54e745c00d42991e0ffcf809df32fdde29efb873febfbb04d106b5f13c385`  
		Last Modified: Fri, 22 Nov 2019 23:29:08 GMT  
		Size: 7.2 MB (7248647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73cb25af478f5d8f5f1eb45a63aa43bb357348836787fe1383a004dbaf87a28`  
		Last Modified: Fri, 22 Nov 2019 23:29:08 GMT  
		Size: 9.5 MB (9529025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbb19ec19469dd4cf6f428559d20702690371622e81bc5959a9e4d53d37b374`  
		Last Modified: Fri, 22 Nov 2019 23:29:29 GMT  
		Size: 50.0 MB (50042485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3758c901bccaee9b17bbc93b91cb3fcdd67ebebb30ac8f78ad551ccaa369df13
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122993959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98cc5c7f82413052dee768c24b452faa69e4bac6f4fc443e3a676566f6ba62e3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:40:29 GMT
ADD file:9facbcd1b6cfe39d1286c4322f52b4a0fffc19c418e69808a91a18d24389ceb4 in / 
# Fri, 22 Nov 2019 13:40:34 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:08:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:08:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:09:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c9323f8b378204c8971fa964b7dea92c5c3506d0fc91bcaed5414c36962d408a`  
		Last Modified: Fri, 22 Nov 2019 13:48:52 GMT  
		Size: 50.3 MB (50254093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79451582277fef4301136fd87a74ac924308c99b67753cd6c706bcd80c4d6345`  
		Last Modified: Fri, 22 Nov 2019 20:26:20 GMT  
		Size: 7.8 MB (7814071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c280be30668695ab64918c37e490a5e9c8f57f6e700f9dd71a928bcbe0397ee`  
		Last Modified: Fri, 22 Nov 2019 20:26:20 GMT  
		Size: 10.2 MB (10190737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6213a386cd1bf3ae8b8fe88af2040a58cea0e519ef25d4938c883cd1c3bc396`  
		Last Modified: Fri, 22 Nov 2019 20:26:44 GMT  
		Size: 54.7 MB (54735058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0a056c014eca4f30af598c61bd7095b2645b2f868c0dae97a02b9d7d150bb0c9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127416784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8343e48f84d100bc5a0197ce251ba801c941a8842e4364808918510564bfe1da`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:38:52 GMT
ADD file:de81f6da93dbb580dd4c6a23ebd6cef637ab58e6f566e5ff7a217d4def3ed529 in / 
# Sat, 28 Dec 2019 04:38:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:18:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:19:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e3ee43b8971d572beb3640b791c4bba0d66137db2252115ebd9b2bb3ab7704d1`  
		Last Modified: Sat, 28 Dec 2019 04:43:38 GMT  
		Size: 52.5 MB (52480376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372a64d1cd36c22d0befce3fc6f8cba8fa5023d7bd33fc658de98186e128919f`  
		Last Modified: Sat, 28 Dec 2019 05:41:00 GMT  
		Size: 8.1 MB (8091626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac8412cc2ead4ec139c961dbfca9f633b422edecc1798b4b7057866f1cac71`  
		Last Modified: Sat, 28 Dec 2019 05:41:00 GMT  
		Size: 10.5 MB (10533850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce9c776c7ea7ab8df81aec52dbda475b2976bb40c49fae2accf334b1755c319`  
		Last Modified: Sat, 28 Dec 2019 05:41:33 GMT  
		Size: 56.3 MB (56310932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:78192f49bcc98a85bfd28b5775b6633eba08d35045e48f2ad8422730391226d5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134223685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e2286ca3b00b2d56ac5562a8e4971720fbab610177677b7c5110fa8f19448f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:53:47 GMT
ADD file:b12b950fad43a45b27069cc60b807b788017c0b7afbda941432314ed9baedce9 in / 
# Fri, 22 Nov 2019 14:53:51 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:49:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 23:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d9030213e9ca0dda517374420b70437d57b213737e4313d3d3b7da588c75a611`  
		Last Modified: Fri, 22 Nov 2019 15:02:18 GMT  
		Size: 55.1 MB (55119200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16d2f968598a1b0dd8a6598974e5227877e498cc41ef594f8083c7abdf1a4ce`  
		Last Modified: Sat, 23 Nov 2019 00:24:36 GMT  
		Size: 8.4 MB (8369585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ba3989924e2be4d02a61b9b821e3f11edd034ec4268e32478ae75a2ee96016`  
		Last Modified: Sat, 23 Nov 2019 00:24:37 GMT  
		Size: 10.9 MB (10947217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b497f921d9442fabccd826d57ba044b65292f9f20feffb112058ff057c075c10`  
		Last Modified: Sat, 23 Nov 2019 00:25:09 GMT  
		Size: 59.8 MB (59787683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b7b8f0ca9eb76c060f9b329fc146cc7e14f375159edaf9ee0390302a62457343
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121409461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eda7070f05f7a039a7679010a17143e0f786e7165a0deee9ab35fd5fc647907`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 10:39:53 GMT
ADD file:dfdf0ec49bef8a55fa525692bafadf9503d769f6fe23f0ccdd904236be48169f in / 
# Fri, 22 Nov 2019 10:39:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 11:24:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 11:24:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 11:24:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5236d095abf6f42c79c788819ad11be11514c8a8774db88619e96d7f50894887`  
		Last Modified: Fri, 22 Nov 2019 10:43:47 GMT  
		Size: 49.9 MB (49940120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de0148a2b53b8c484e691bc4e736d5e54e5a5226d9a2584acfdde9b61f5ad94`  
		Last Modified: Fri, 22 Nov 2019 11:35:52 GMT  
		Size: 7.6 MB (7607980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f5e6e78499e671d55a0eea16bedc319ce1a849b8bb130123ea84e3a36200c`  
		Last Modified: Fri, 22 Nov 2019 11:35:52 GMT  
		Size: 10.1 MB (10068046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8b7feccc17881afd1b2cd965d593673d29e34b4976317fe8172011e0824d3a`  
		Last Modified: Fri, 22 Nov 2019 11:36:06 GMT  
		Size: 53.8 MB (53793315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
