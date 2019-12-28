## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:36d577a86ba52fe6a1ba40679855a3df9764a616fb4d8f6142374d0e480a6114
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
$ docker pull buildpack-deps@sha256:1721528bb36897a77e5039566e8b91af81168cf831f8cfe6ed700192ab158412
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118840756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ad9ebde0a55fcfc339eac1ce9eb39cf327a1ea86b115e7f372834876d3b8e7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:48:50 GMT
ADD file:730d57bac91e32701978679d8ccfd9d70521397f6008ad321414c8d7ccefd937 in / 
# Sat, 28 Dec 2019 04:48:52 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:17:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:18:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:19:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a3c7b9678a433c6c2e10ed1e6dc96f81cfce99fe5f71bc8091965c137d50306d`  
		Last Modified: Sat, 28 Dec 2019 04:55:31 GMT  
		Size: 49.3 MB (49328079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775f3daa9663989f7914a385f5db11a26a307dab5f2cd76d08edc09eda570a44`  
		Last Modified: Sat, 28 Dec 2019 05:48:51 GMT  
		Size: 7.5 MB (7490102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebeaaf463e9882767863e9735347274863750c30cf65c8b1a8c8032c9e7b221`  
		Last Modified: Sat, 28 Dec 2019 05:48:52 GMT  
		Size: 9.9 MB (9877186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c828bf3de027e23d3ec285037b09ce1cd8652c1389dcdd865fb7522c5eeb0d`  
		Last Modified: Sat, 28 Dec 2019 05:49:16 GMT  
		Size: 52.1 MB (52145389 bytes)  
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
$ docker pull buildpack-deps@sha256:648bcdcbc5c099c496688f4b83f7956f0035fe1a4e658a80e35785be2816e686
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123012049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13619a66d0c681a286754308843cba12b0159cb8fe986858474992775d72f458`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:59 GMT
ADD file:d8dee71c9b462c830ef0fea7e4ea281b8c8ee4f3a1e9e3252fae2401bc715637 in / 
# Sat, 28 Dec 2019 04:40:01 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:58:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:58:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:59:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ddc6b7ca7922f46e5d77becb1dd9bdbfabf5d66b99008799facc91235201022`  
		Last Modified: Sat, 28 Dec 2019 04:46:03 GMT  
		Size: 50.3 MB (50319316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f147f3a8b319f949fb21cc8ef219b5e607881821f497aad9dea6fe7a9a88977e`  
		Last Modified: Sat, 28 Dec 2019 06:19:47 GMT  
		Size: 7.8 MB (7793115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15fd445a2b52a4806ef65aaa42f0fe599f857e4b40277d4740433c4c0e2380f`  
		Last Modified: Sat, 28 Dec 2019 06:19:47 GMT  
		Size: 10.2 MB (10191212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aedd3ed7054c5c8146cd072344a2a3541373199331f8fff581744540645125`  
		Last Modified: Sat, 28 Dec 2019 06:20:10 GMT  
		Size: 54.7 MB (54708406 bytes)  
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
$ docker pull buildpack-deps@sha256:d4efd8f642ca901997f36c78eda44ed1ae1bbcaf5d321663369fbeced4c0d60e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121446309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c42a29541a54a65a95732adae6108d161f61c11baf037171dddbb6df083838b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:30 GMT
ADD file:ef81707ff6f9411444d40f7819b6103572f1c71599afd4c687f5262af6d30f7d in / 
# Sat, 28 Dec 2019 04:41:30 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:42:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:42:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:42:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6967537f6d685c8e7bce246638525934908340998b95e5baed55bd5e9805611f`  
		Last Modified: Sat, 28 Dec 2019 04:44:31 GMT  
		Size: 50.0 MB (50017657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5626baeec9661579acdaed4ea6587cae4c16df097bc274ac329b6422d405ed9d`  
		Last Modified: Sat, 28 Dec 2019 05:52:41 GMT  
		Size: 7.6 MB (7590139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc69b710fc3f7e4f96daf59aa3255a7f810b677a869eedde6dc313330d76855e`  
		Last Modified: Sat, 28 Dec 2019 05:52:41 GMT  
		Size: 10.1 MB (10068811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb0c2c2d0d3cba15da991cde49579c040bc860db52909b9eb568b8bd8326b59`  
		Last Modified: Sat, 28 Dec 2019 05:52:54 GMT  
		Size: 53.8 MB (53769702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
