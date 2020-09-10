## `buildpack-deps:stretch`

```console
$ docker pull buildpack-deps@sha256:ca02fbfbde080c2b05acbf920142f467d364d200c77e3a11200c37a8d9fda52f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4acd894d4b272f8325be3fdb3a1c168f1a74ce7010e321c79c53ed7d19efb59c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.8 MB (324822076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3592a5919baa4b40e62c9bd109c6cc71d62857ec79f9b0a479822cabec226baa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:11:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:11:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:11:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:12:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b49aa113642e1d83773ca83de882e12c4981ed565d47b4c7da998855ad182e1`  
		Last Modified: Thu, 10 Sep 2020 01:19:16 GMT  
		Size: 10.8 MB (10750802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159512f4cc2a5f8c64890a32b7766e2662b61241ef585cc28daf194bccaf1c1`  
		Last Modified: Thu, 10 Sep 2020 01:19:14 GMT  
		Size: 4.3 MB (4340512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8439168fd8dcb35b71c06211b4c23c02bd846e1d37f72cfe5638ada30c196556`  
		Last Modified: Thu, 10 Sep 2020 01:19:35 GMT  
		Size: 50.1 MB (50109858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abbc6cc15820e59f3f9effd6987da17f809be3666d5db2c7ccb5795f8b35ed`  
		Last Modified: Thu, 10 Sep 2020 01:20:31 GMT  
		Size: 214.3 MB (214254178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2581c3073f6994bbb53071c2fe01e1f3e3f7151f2f62a3eab0d3362355cbe8ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.8 MB (308799310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b05b9cb8ee46a1e24af180ab61c8bf9cef8cc8f835e11d5ff0f72aef2355e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:58:16 GMT
ADD file:39312a9e824bd7c6ad3eca3ada9e922d8f7219c51e10047672e9ccab3dadb248 in / 
# Wed, 09 Sep 2020 23:58:18 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:46:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:47:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:48:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:51:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:301ffd407a7ebea8722c85a0474f1c621b0785275eef7a32a1ab7b5106a8e762`  
		Last Modified: Thu, 10 Sep 2020 00:06:45 GMT  
		Size: 44.1 MB (44081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7b013af3cd7da74fdf184d75df567c3ba56ee21fa571230b433477d588a2`  
		Last Modified: Thu, 10 Sep 2020 00:58:19 GMT  
		Size: 9.8 MB (9824691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f78c2d8a2a251c2677baf2550b75f26e68595aaeefd369b10dbeb6c4a8a76e8`  
		Last Modified: Thu, 10 Sep 2020 00:58:17 GMT  
		Size: 4.2 MB (4160081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaf49af0025cf63295d41c39b9a75e9e4adb695cfe41f26eb93f8801ee772b2`  
		Last Modified: Thu, 10 Sep 2020 00:58:44 GMT  
		Size: 48.3 MB (48303402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf51849333ce3877a155c777af22bd80cf80ef93df727a4e41be228d0cfff6c`  
		Last Modified: Thu, 10 Sep 2020 00:59:50 GMT  
		Size: 202.4 MB (202429839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:83ae2f04b731eb19211b7fa221148743e841ccbf593be55b2ffc104dd7b726a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297351493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eda56eeb3d5cec26a5835f3426080074902008964d37fc7855e540c5011d5b7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:04 GMT
ADD file:0ba6f3203fb10e66124d03088d234e92fc908c572ec7eed268e866623a383a7d in / 
# Tue, 04 Aug 2020 05:01:07 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:16:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:18:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:29:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:323178d00ec2c5eb5ffb9cb696a52eaf8683dcf2eb605c742da2953556f06e37`  
		Last Modified: Tue, 04 Aug 2020 05:08:40 GMT  
		Size: 42.1 MB (42111382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b4e15a79453f6ae10815d79c8f4590aef2f1ac2979c192ff7f1ed0fbf04e60`  
		Last Modified: Tue, 04 Aug 2020 08:30:43 GMT  
		Size: 9.4 MB (9443881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9cb1ef704caf3af8a2ed43dc12884b4f74ac867ce95f60bd8996f51fde770`  
		Last Modified: Tue, 04 Aug 2020 08:30:41 GMT  
		Size: 3.9 MB (3918490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ae4cf51f1ae7af0566bc381b7fdc344ae6a916df2554156029039b4925d30c`  
		Last Modified: Tue, 04 Aug 2020 08:31:09 GMT  
		Size: 46.4 MB (46415465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dd65b90e26540484b3e0609a821c0d6fcdf223f03988f82d4e6dcda308eead`  
		Last Modified: Tue, 01 Sep 2020 00:37:20 GMT  
		Size: 195.5 MB (195462275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:16fc8ae2599d4111afbcfccbe907395b5298f90369d32ea50f3e53675bfb488c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.6 MB (306635545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54b96c7cd53c3cd45c00a46065b25cf4be4a280cec56a34006aca5c20b1f6771`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:23 GMT
ADD file:f74bb8d38ef70a022988428f254630d1f424ed9a3b957687b0cd0f85b9d49e29 in / 
# Wed, 09 Sep 2020 23:54:25 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:35:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:36:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:38:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b396f138ad78ffceac749b105c676dce568fa15a7b9f2273c2ee13ba023cea1`  
		Last Modified: Thu, 10 Sep 2020 00:01:33 GMT  
		Size: 43.2 MB (43171697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5db606bd1ccd8d11ca18492ee5d5122fdae2e7172ceb0df9cd15dc4d9f3c259`  
		Last Modified: Thu, 10 Sep 2020 00:45:55 GMT  
		Size: 9.7 MB (9700841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd3b5402f1859618a8e455e6bf04a916c8460da1c5f115568ba530c96f6ba3`  
		Last Modified: Thu, 10 Sep 2020 00:45:52 GMT  
		Size: 4.1 MB (4095176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb81e51c7d923c71bc53fedd00e3247cbe38545e27848eb452110320aedf641`  
		Last Modified: Thu, 10 Sep 2020 00:46:19 GMT  
		Size: 48.0 MB (48044000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6077cb8785bbbed8f14fef78ee07d648b12216bfc6551532fd1029138ffce0d9`  
		Last Modified: Thu, 10 Sep 2020 00:47:20 GMT  
		Size: 201.6 MB (201623831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; 386

```console
$ docker pull buildpack-deps@sha256:fa919635f8792cdd52ae686e1d5e52965fe47f15910c154fb06b6f68beb3297f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.1 MB (333052484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:243900ea89f4fe31ab7b140ecd0b4c2e2053d7c848dccf37e6adbe6d47e3274f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:39:59 GMT
ADD file:af30f23f89d9bbdd6ad60199f3d978a5e426835c6138e0c76a3453680945a121 in / 
# Tue, 04 Aug 2020 03:39:59 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:21:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:21:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:47:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36eaaca1a8d1677d2d2aa93f595d838e71ccbe4254f548ff566f97e8d555df1c`  
		Last Modified: Tue, 04 Aug 2020 03:45:28 GMT  
		Size: 46.1 MB (46086777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312e98903306441f0b9bd43306e20722d14f9f02f55de10e037f31f8e9887d06`  
		Last Modified: Tue, 04 Aug 2020 08:30:08 GMT  
		Size: 10.8 MB (10773882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fa371da331bdfaab943357b965c1839c24c25c15a78aaa7180325db8fb59ca`  
		Last Modified: Tue, 04 Aug 2020 08:30:06 GMT  
		Size: 4.6 MB (4561115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b121224d37089d29e88079f00cc9ed94ee5cf4bc763184a9c90231f28a0291`  
		Last Modified: Tue, 04 Aug 2020 08:30:39 GMT  
		Size: 51.6 MB (51619972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0634421f8324e02f1a930803af89dacac42b4a7b85354c9e881491e55c1dcd4f`  
		Last Modified: Mon, 31 Aug 2020 23:52:19 GMT  
		Size: 220.0 MB (220010738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
