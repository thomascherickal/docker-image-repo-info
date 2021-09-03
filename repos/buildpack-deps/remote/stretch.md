## `buildpack-deps:stretch`

```console
$ docker pull buildpack-deps@sha256:7a134fd5af7789892eee5195491d385175ac371a3c28b343bac3acbb45e20e41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7140662b65e0e50b57644a55d12cde26e955fa8697dc363f06643bfc8df1dfac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.2 MB (325207071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe35bd8b28ed0f3b5c033b305de8ff1f004be0241f69a4687617ce4d5fb5f03`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:56 GMT
ADD file:0d0aa1ebd07b0f301aaf1077d1e9f2e9be1859510dd8535e143571b347a2a379 in / 
# Tue, 17 Aug 2021 01:25:56 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:24:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:25:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:26:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eb18d230e067c240479c6a3f842e7f9d4ff1088e3072d0a3245829c4e356623f`  
		Last Modified: Tue, 17 Aug 2021 01:33:03 GMT  
		Size: 45.4 MB (45379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83600c1b4583abb5830c6d4a039cbab9a102ac1a7b3b779854638a371bb7128f`  
		Last Modified: Tue, 17 Aug 2021 09:33:12 GMT  
		Size: 11.3 MB (11295906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae15c65bfa0fdc9053dcb734e6c034f5394ea0481dee3277f6e3e9fa07702d0`  
		Last Modified: Tue, 17 Aug 2021 09:33:11 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19c058edda50f20bd5b06380342e9d99f7138770d79e0b031565dd0c7707fce`  
		Last Modified: Tue, 17 Aug 2021 09:33:34 GMT  
		Size: 49.8 MB (49761551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cdaa0fd103b33659feffaac5fd7cc202fbf1d8061ae2bf6da5a4540db9aced`  
		Last Modified: Tue, 17 Aug 2021 09:34:21 GMT  
		Size: 214.4 MB (214427261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:08f426f38c8106dd8aa8568b793a5ba5b250531b281b1678595f813202229256
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309140896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24a89e103857742245f4811bd7db46b7f04cc78607cda0ca817a9a998b3da22c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:55:20 GMT
ADD file:838b3017c5e14c9c2cb8e2beed881284e402b04a3fa00d6660af0164a62e9aac in / 
# Fri, 03 Sep 2021 00:55:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:44:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:44:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:45:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:48:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:990f81d6b076b231549a6d1c9525983e601a394687d6f34de260e0319bf53ccd`  
		Last Modified: Fri, 03 Sep 2021 01:13:22 GMT  
		Size: 44.1 MB (44091687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddec37b68b0e6232e73d38bbe052e6804a945ec22ed1da8856b3a94ae6967d5d`  
		Last Modified: Fri, 03 Sep 2021 03:00:36 GMT  
		Size: 10.4 MB (10350740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad7b012ed89a45c8d41452eee67434c831c33349535d3edc940d38f72a814a6`  
		Last Modified: Fri, 03 Sep 2021 03:00:33 GMT  
		Size: 4.2 MB (4161371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523728c66871b711f3e47439ee3a65721b15132ee3a78cd31ba598a14ef8e4db`  
		Last Modified: Fri, 03 Sep 2021 03:01:25 GMT  
		Size: 48.0 MB (47984014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87df525559bdf36ecfd5e039f89ff4e8e54fa5e20199594e65d429ff15b85e5`  
		Last Modified: Fri, 03 Sep 2021 03:03:38 GMT  
		Size: 202.6 MB (202553084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:30cd3cac17d470467a8cf74ba547e77ae65e7847e9ec0284700fb9a126c80b04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.2 MB (297167238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b5fcb78438be37f80b23f414e4affc7f611ab6e4feae62206ecfe362719378`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:19:00 GMT
ADD file:5e5e5a4e13ae8e36740009c29111838a32d9901b28809b485c841d25d550698b in / 
# Tue, 17 Aug 2021 02:19:01 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:28:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:29:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:31:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30d3c67f4f95a7d99559389477234b45c05024484d59cec2d66264610a623fe9`  
		Last Modified: Tue, 17 Aug 2021 02:36:17 GMT  
		Size: 42.1 MB (42119745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e002433047948d255f28ba7ee556c302875d03d4d84f4b30b34ed9aeb481ef27`  
		Last Modified: Tue, 17 Aug 2021 15:46:54 GMT  
		Size: 10.0 MB (9951645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a501430415711f6cdd553e589abddd926f28b6f57669a8fafbbc06811a06d`  
		Last Modified: Tue, 17 Aug 2021 15:46:51 GMT  
		Size: 3.9 MB (3921237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a964d42e4129b0cb2f1ef7515a1c3e7c3da3e87809647c943d2b93ed050c085`  
		Last Modified: Tue, 17 Aug 2021 15:47:41 GMT  
		Size: 46.1 MB (46126157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66df9821cbd775d34186e903acf3618eeebbdd0a82d10831f032ebbec47998cf`  
		Last Modified: Tue, 17 Aug 2021 15:49:44 GMT  
		Size: 195.0 MB (195048454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ae83af90d691f92f963003f326247d07f0c63572c001d5180e68382aab10d6e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (306982017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7fc2be127f7f58a889012cda6a9554a463eb77fec3a18ca69c952ed841b0872`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:17 GMT
ADD file:79e0d0ec943ec405612e2310514d8f0c72cf83483eea6d5f1a7c28b36fa21cf8 in / 
# Tue, 17 Aug 2021 01:48:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:57:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a410f7a7fb8af899e64ef008ec59cc8062766e91abbf21ba5cee65faac7ba3fa`  
		Last Modified: Tue, 17 Aug 2021 01:57:32 GMT  
		Size: 43.2 MB (43177652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e420ab67f91937cc8165f5fb2e94bdab905576eadca5515be250bc6212fe50`  
		Last Modified: Tue, 17 Aug 2021 08:04:49 GMT  
		Size: 10.2 MB (10215748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce4bbd3804fd1154090db6722050023d8242e910e02ed7d2c09b9795a9d5ac`  
		Last Modified: Tue, 17 Aug 2021 08:04:48 GMT  
		Size: 4.1 MB (4096582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef28464eb814f6aec9fd29bb296de85a00b19fbb82a37d054836d456c6c89e5`  
		Last Modified: Tue, 17 Aug 2021 08:05:09 GMT  
		Size: 47.7 MB (47737246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718fbc9c6e759c3ca24d0ddaf5a8ffef316cd17ec7a99f5d6d594acbc059b130`  
		Last Modified: Tue, 17 Aug 2021 08:05:49 GMT  
		Size: 201.8 MB (201754789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5260fc02445d2b84a9104ea735633337a14510f9f6f419680364f555d4c8db5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332746112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eee6c39829a2ce415ec6595cd1ed8c78d12cecc7cfb834593c2701a61555b7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:30 GMT
ADD file:46f32d47386428deefe487caf3a07dcbb3fe2f2e89abd3b63cbe7e9d31444ec6 in / 
# Fri, 03 Sep 2021 00:42:30 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:15:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:15:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:16:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:17:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dadb58ce47b39e4093a503cf3b5a3fdb91180e4b16e14c1146b7bb865336d6f5`  
		Last Modified: Fri, 03 Sep 2021 00:52:52 GMT  
		Size: 46.1 MB (46097308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd444f00c798bfd4f9e617154309c372e8d36842dd1b1941d71becd772ddfcc`  
		Last Modified: Fri, 03 Sep 2021 01:23:40 GMT  
		Size: 11.4 MB (11353014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0571d1af33e8ba8e01d8c5f2ff9b4e4a3bd4bd88c459d958bfaa57077a0a3f6a`  
		Last Modified: Fri, 03 Sep 2021 01:23:39 GMT  
		Size: 4.6 MB (4564992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dcaa4b267350835d07fbb9cd12470a43123a18957bf035ad503417f9fe38ef`  
		Last Modified: Fri, 03 Sep 2021 01:24:06 GMT  
		Size: 51.3 MB (51265099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdd9208b418741f0fcf524595f56261907ebd69eebdb908348e350ff0283083`  
		Last Modified: Fri, 03 Sep 2021 01:25:03 GMT  
		Size: 219.5 MB (219465699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
