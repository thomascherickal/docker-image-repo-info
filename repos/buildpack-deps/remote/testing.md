## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:b950faeb40fa9cd7152f8272ccd087e7b98c5f7407dedb32f079bf9a453007c2
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

### `buildpack-deps:testing` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d02593a621ee4f4e7e1fcf39298988b2d0ed222e1d591c59c1d473821d34b6f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344906770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0c0cbc5ed6d6e7cc27ef5c4f8b20fdb7085d85320252f8db1c8f63fc75f111`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:52:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:52:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:52:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:54:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e064222ce493e48ae4ceac8f18316e08d2afb963ad57bd63b8630a0ae009f8`  
		Last Modified: Wed, 05 Oct 2022 01:18:07 GMT  
		Size: 9.3 MB (9298646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab229472e3a483409ce2bbc4d461fc6512c03c687daf6546b52705bc7f18961`  
		Last Modified: Wed, 05 Oct 2022 01:18:08 GMT  
		Size: 11.4 MB (11381655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a5a87ebbd4472db252972521c82b5789bcc45b6bf1ff4d5e59ab129a4847a`  
		Last Modified: Wed, 05 Oct 2022 01:18:25 GMT  
		Size: 57.2 MB (57201277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685ee8ce50d5fd303a9b0b6cb4cdf889b35afe78677a8c5006983f396b8fca18`  
		Last Modified: Wed, 05 Oct 2022 01:19:02 GMT  
		Size: 214.1 MB (214062777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:bffb582eea88f603b6d41c7ef23daad00bb2fedee97c28181f7fe609f4b8eb2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312440441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c474715e9214bf3e8018135a814e87399cc0e126d54b51bd68270a348d072679`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:48:31 GMT
ADD file:2f3df348b6a9200fcbcfe13a10334cef72dca5f19d7ed73055f7a03ff08122f7 in / 
# Tue, 04 Oct 2022 23:48:31 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:12:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:12:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:16:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2843f1fd91937d710e0d158046e9c23fe034f11c8c934a478f443b561be758dc`  
		Last Modified: Tue, 04 Oct 2022 23:52:36 GMT  
		Size: 51.8 MB (51838659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cbaeabf686852f0109b0402554bbb882e0b7f95b9befb62dcb2c9cf5334b69`  
		Last Modified: Wed, 05 Oct 2022 00:22:23 GMT  
		Size: 8.7 MB (8744107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b61654d50a40ae8ba57e261eb049904e5e6879f2e9421bb37a8653997b3e6`  
		Last Modified: Wed, 05 Oct 2022 00:22:23 GMT  
		Size: 11.0 MB (11029995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53865dde9c538a03f148e1ba35bf9cb11545d6cc64b982f47d173fc76948ae`  
		Last Modified: Wed, 05 Oct 2022 00:22:46 GMT  
		Size: 54.9 MB (54925579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f85847cb13db9404a8575edd2177010fed6281224d36c5619b9d604f3102372`  
		Last Modified: Wed, 05 Oct 2022 00:23:26 GMT  
		Size: 185.9 MB (185902101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f8a1f3a13a8adaaea5da7e387c0c6867d981753b39f1e85cc607bb0e97fa47a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298606196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:922e36dda65d9735b5f1feb9124dfafb756dd2899076bce2617b826416afae3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:29:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b865ef48770b9d41964e18461ec2d393677f4fc653a0953e9f0b9773d47ac`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 8.4 MB (8396889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b8eea02f53006b302a3dbae787275ce520ccf78df670e0dcafbfd1c4e17cd`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 10.7 MB (10661490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540119c620ce1fcebd013dc72077ca8f4751440b9eb633b56bd350f29e749420`  
		Last Modified: Wed, 05 Oct 2022 00:52:26 GMT  
		Size: 53.0 MB (53011353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a5488439a4130d35884d12b04702afc44c003d55109f1c35f807bec217827a`  
		Last Modified: Wed, 05 Oct 2022 00:53:14 GMT  
		Size: 176.8 MB (176843856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2c9d7478dc930122cd273ab910c4e54acd9fda294855bb0f8e83c7994afca09c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (333984748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bac13661039857034620f3623296aa9b007fefa292cbee49f39e1aaf06dc185`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:00 GMT
ADD file:269c8bec4871d84b9133706a2f391209619d53c0bfa56121c740757cf5798fcb in / 
# Tue, 04 Oct 2022 23:44:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:21:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:21:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:22:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2debf9e7f23054c81a936da9b01c5db9f72a55d4810f7bf0e5641bd1748d90b7`  
		Last Modified: Tue, 04 Oct 2022 23:49:11 GMT  
		Size: 53.0 MB (52980389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a790615211c3ee762ced64a5b81859f93d76062f4cf9c83d396fb13c24f7cf`  
		Last Modified: Wed, 05 Oct 2022 00:36:13 GMT  
		Size: 9.1 MB (9128105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70f6dfe035ba217dd9a40e630bb3cae03e8d9cef649641a8a502495edf00c0`  
		Last Modified: Wed, 05 Oct 2022 00:36:13 GMT  
		Size: 11.1 MB (11134219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9ff2029a6f8ea8f4523829a06c0ce632548ee555f4321818634a64fb364c59`  
		Last Modified: Wed, 05 Oct 2022 00:36:33 GMT  
		Size: 57.1 MB (57125848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d33af7178fa987f0bc084f0b049703cbac4eef9ff6b4a6d85686e44a35c67`  
		Last Modified: Wed, 05 Oct 2022 00:37:10 GMT  
		Size: 203.6 MB (203616187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c61bc9ddb07ae12f0fe15074c296f69f98f8df87ddbd85fe591ef91c7103af72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.1 MB (347090383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fdf61bf7da4f98ff50562c5979008a5a6047c598219298c4425f52a45446dd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:38:57 GMT
ADD file:2a0c743e373aeed6462c2f3ae8a138fb0e240e935ad7ca5bf008aa3efd3673a0 in / 
# Tue, 04 Oct 2022 23:38:58 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:06:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:06:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:07:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:08:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68776dad61a299b8e65d1a6a02e376b8ed2e9b241bd753bf6c35d497055ecdf`  
		Last Modified: Tue, 04 Oct 2022 23:44:23 GMT  
		Size: 53.9 MB (53932827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e1a78eaf50f3a9e7fd0eaec3d6abbc176033d6ca5108dafee5df9988d1427f`  
		Last Modified: Wed, 05 Oct 2022 00:20:44 GMT  
		Size: 9.5 MB (9473771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cc3926eab5aa6b28a396ddad5f657d4bd9890ed5be6836db7cb21429b7923c`  
		Last Modified: Wed, 05 Oct 2022 00:20:44 GMT  
		Size: 11.6 MB (11576979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078aef1e51356ae4c36a96958de308109bcf837c427b8419820646e4fcb45528`  
		Last Modified: Wed, 05 Oct 2022 00:21:03 GMT  
		Size: 58.7 MB (58692129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f369df58d33dbf70162bcfe07d395e297e455b239a2ba9b5782025519ba8fb88`  
		Last Modified: Wed, 05 Oct 2022 00:21:40 GMT  
		Size: 213.4 MB (213414677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e96c56d3802f1d03989d4afc1c9e54f75b256e0ab531932a5452aefc857c2b97
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.9 MB (319903659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d117325794165da4de7ce6de9904f16f3847ebfa03ff1dbda099d1546e9c8aba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:02:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:11:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc6e8e3ab563929336c7963595d1f292897822342a96c95dcb7cff4bc403b4`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 8.7 MB (8663556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c7dae3a16e88ec9bace52486f5c77ed5891921868e64784dd35f09d55ab46`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 11.1 MB (11128331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e031ef7803b56989f08a0276998fb1edfcabb65ab13ea4a75513a55ad575bc42`  
		Last Modified: Wed, 05 Oct 2022 01:29:37 GMT  
		Size: 56.0 MB (56034915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc6482afe3cbf6106cb4fac04ae9d8ed471a7830e0984fba53bec6d8616c441`  
		Last Modified: Wed, 05 Oct 2022 01:31:49 GMT  
		Size: 191.1 MB (191109878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:07d09da658d3847837f93e14e29bbc1644f015af1e723c45312b0fdad7a3c757
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.3 MB (356295415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2835f139a6888341f1a48f5ef618719060149cacf634a077780bf069b1af9081`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:16:56 GMT
ADD file:22dddefde9f3e8eff6049751a459a3c4fdade46622016ce6269b630157170962 in / 
# Tue, 04 Oct 2022 23:16:59 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:47:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Oct 2022 23:47:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Oct 2022 23:48:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Oct 2022 23:52:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8fd653dd210d0ff49ceb9b32e662a564ab01445265e165edd4f963c3953f5b33`  
		Last Modified: Tue, 04 Oct 2022 23:22:42 GMT  
		Size: 57.1 MB (57111564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f7f38b022f1a84d71f8e4124fe0133ced1b702ee627bff0eb3e756558fbdd`  
		Last Modified: Wed, 05 Oct 2022 00:02:33 GMT  
		Size: 9.9 MB (9883282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79064b2f900a5a0fc53fac8232b1268f1f2e3496cc5722826e03a2b768366be9`  
		Last Modified: Wed, 05 Oct 2022 00:02:33 GMT  
		Size: 12.1 MB (12143792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e113e7ad373417ab9b8860252dfab9e3cb296c126693a7c0b8ad045607bed6`  
		Last Modified: Wed, 05 Oct 2022 00:03:02 GMT  
		Size: 61.9 MB (61909581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b834427f613a2283606b20a73c866242afc6d2dd8dc2d2fd3c6aea1746a274`  
		Last Modified: Wed, 05 Oct 2022 00:04:04 GMT  
		Size: 215.2 MB (215247196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ca693cee2d4305a9edfe1215177fe7bce3fec775aaf9f12a28262dbb1c9a2667
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312418079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7701a1183713de3a8c1d0a68352ebc3d189b43e8268d017a7adc512ad72d67a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:41:48 GMT
ADD file:75b0ff403984b3c95919c781c632871090a7238d4c22c9c631160406de8309a4 in / 
# Tue, 04 Oct 2022 23:41:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:07:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:08:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:10:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7893043d434a6c00815ae2e7de11adb8c1f06815bbea513110060ae94e8851b`  
		Last Modified: Tue, 04 Oct 2022 23:46:26 GMT  
		Size: 51.3 MB (51280212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ed7a0c18fee7ec61cc5b8d9ae520abe4b09aa014195c8b9481866aa0eff290`  
		Last Modified: Wed, 05 Oct 2022 00:31:29 GMT  
		Size: 8.9 MB (8935386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d523eea662ddeeaa863120a2afe9127a5bb8c4a67ff524928ce23514e9469`  
		Last Modified: Wed, 05 Oct 2022 00:31:29 GMT  
		Size: 11.2 MB (11240632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff33f2f178d309eb3e2d7fb3457599b55e7731e1d8af441d100e4eb4c7e1b8a3`  
		Last Modified: Wed, 05 Oct 2022 00:31:43 GMT  
		Size: 56.5 MB (56475750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1a4e974c1d6e566e23f56c5816a9e132401dc1ed192d0669cf5dea70d01d8`  
		Last Modified: Wed, 05 Oct 2022 00:32:10 GMT  
		Size: 184.5 MB (184486099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
