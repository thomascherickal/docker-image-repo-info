## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:4af3914903f7c8c135eca2d9364561d3b57c19689e1d7523c6d319c84de9d5c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:826b7f49bc9a72a20279db6c676aaf1f19ff402cc633bbbf904c251b7d4e5b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.1 MB (322078647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b41bb8c2c06896a0a16fc0921b0f55d9b4b0b01ec0d4811dee0afdd37b76e54`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:57 GMT
ADD file:97b8c276224b2b9407a1635d61780b968f86726642a00f3d49298ab19e9ea714 in / 
# Sat, 10 Apr 2021 01:20:57 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:55:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:55:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 01:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9097f35530b77dcae85a27364a3301e3362adb2860367422ed06b99fabe94b8b`  
		Last Modified: Sat, 10 Apr 2021 01:26:23 GMT  
		Size: 54.9 MB (54881626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4657bb2202fe6d13371845dabecbb1843dc3e9ab3d45afba017280a24f40`  
		Last Modified: Sat, 10 Apr 2021 02:03:17 GMT  
		Size: 5.2 MB (5169536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a456d1fa6a4d732964fc57896f119a9e85d6cae028f4deffc62729e23624641c`  
		Last Modified: Sat, 10 Apr 2021 02:03:18 GMT  
		Size: 10.9 MB (10868840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815ce4c9e511158bf858d6ebdb7862400e9c296a85eeccce737045c8e04145ff`  
		Last Modified: Sat, 10 Apr 2021 02:03:38 GMT  
		Size: 54.8 MB (54798810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce986c96c05b40a3246a50f4ed1397b3a8933e666eb453c9829290f006450814`  
		Last Modified: Sat, 10 Apr 2021 02:04:17 GMT  
		Size: 196.4 MB (196359835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:eae6cbaf20141aecfced2e5c51526d7d23846eb386a99f9cd4fcf791cf3be30c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295144721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f5e1196dd3b711e7a01a4f21ac18f304f2ad73daef766bec8e5de21df97183`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:52:44 GMT
ADD file:9bdb85e8b11f9d011901b496376920ceaf2a43e4dd9f7dce303f362c5cd9847b in / 
# Sat, 10 Apr 2021 00:52:52 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 02:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:11:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84ee0e585c798c84e07ba41f87e072c0fb43795cb12e325a126f9026f876059c`  
		Last Modified: Sat, 10 Apr 2021 01:00:27 GMT  
		Size: 52.4 MB (52414024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f91ce0c40daeff87428c76fc2b11803ad6153af50d86ab3e84d37fb8ad8ca7`  
		Last Modified: Sat, 10 Apr 2021 02:20:41 GMT  
		Size: 5.1 MB (5074282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a126b0b2e172136e012642af22312fd73d761d735f0990caf91f35b6f294fb88`  
		Last Modified: Sat, 10 Apr 2021 02:20:39 GMT  
		Size: 10.6 MB (10570471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d442e399c5e6a8d0ac5b10309719b78c3f28f95043726252343efa4387a92288`  
		Last Modified: Sat, 10 Apr 2021 02:21:05 GMT  
		Size: 52.5 MB (52498471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a9d706d7bfb467b998041cdae5a80b507c2059ef13d990f31e13f45f2e876`  
		Last Modified: Sat, 10 Apr 2021 02:21:59 GMT  
		Size: 174.6 MB (174587473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f912292f15f822d363a5637a0671020c2c58c99a05ad874ae929159af91d604b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282583834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88e3f5ed34b6bdd5b62c4e0d768be0bffc8551688fcd1823f565084704401337`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:01:00 GMT
ADD file:b91b8d2ef6efe2bd9fc0625108290b82f4567ba3654aeea20bd4b9e7c9fcacca in / 
# Sat, 10 Apr 2021 01:01:05 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:09:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 06:10:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:11:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e9c76177d1ffa0bc1a85678dee6f5c61b2264a677790342fc5bb17961fb8015`  
		Last Modified: Sat, 10 Apr 2021 01:08:52 GMT  
		Size: 50.1 MB (50083439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26176a706c2fe768e7e54369121192f2b1336a3ac2985c3b017b574b99f4164e`  
		Last Modified: Sat, 10 Apr 2021 06:21:18 GMT  
		Size: 4.9 MB (4935049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ba90a2781c4eed4854a1e54204b119cfe0e948ec34564b9e2235d443f69f1`  
		Last Modified: Sat, 10 Apr 2021 06:21:19 GMT  
		Size: 10.2 MB (10218224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cd0a84cbd21a2be98dbced0d40b752d619473a031122610ee81667f9c56d22`  
		Last Modified: Sat, 10 Apr 2021 06:21:42 GMT  
		Size: 50.5 MB (50514802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2fcb6c699d8fb33a40e65446c562b6072c84b985e54e22a74694da9eed6c80`  
		Last Modified: Sat, 10 Apr 2021 06:22:33 GMT  
		Size: 166.8 MB (166832320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d46ed71c122fff936e5c78a8e146ad724e4d250304ada1a0cb89ae46562050d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.8 MB (313768605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6516cc551c567d1a47efb9687399d22b4bc99767e3fe89c0eac5cfd738e5edfc`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:30 GMT
ADD file:6bd461aca61a6c4468971e152cdd2158ba47c56a30fedd2560ab69bc0d5429d0 in / 
# Sat, 10 Apr 2021 00:42:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:50:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 01:50:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:53:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4d191ad9b976ffe4d9719cf4d8241d751e0870f7abf4ded747f4258cce757b2`  
		Last Modified: Sat, 10 Apr 2021 00:48:46 GMT  
		Size: 53.6 MB (53568143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5779dd445520bcb3f8ff73ed0cfdf91d218d8c0272557c8e2959626d83c1e6cb`  
		Last Modified: Sat, 10 Apr 2021 02:02:23 GMT  
		Size: 5.2 MB (5157782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c386828fc4d261064c2034ef6ea283e4de5534b6dc52e8f7dd4d4cb671677`  
		Last Modified: Sat, 10 Apr 2021 02:02:24 GMT  
		Size: 10.9 MB (10868647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51a5dcfdd30750f476f52ea0e183b37054c17682ecbd66f52636582ad051c41`  
		Last Modified: Sat, 10 Apr 2021 02:02:46 GMT  
		Size: 54.9 MB (54920818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c48769838a9abb7c058dca4fa32400e26d68739d5fd7e303e2ec2f8b8a37ec`  
		Last Modified: Sat, 10 Apr 2021 02:03:35 GMT  
		Size: 189.3 MB (189253215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a8cbfa210ba2e8de2f182de92340f795f5c18f4371a9982daa795025471a1209
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327952168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd00c168aac32d9b00131e73e21c97da9795097309e8a43ca709fde35659ac8b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:40:23 GMT
ADD file:e8f1dc678a4622b7caa83d305ed03d778d1fd4b248d1217382e32f2b6e88b87f in / 
# Sat, 10 Apr 2021 00:40:24 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:19:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:20:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 03:20:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:21:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b3e9fd2b852472b6f69da429722bff4b757f5da21d5bbda36f776b73d788c39`  
		Last Modified: Sat, 10 Apr 2021 00:47:25 GMT  
		Size: 55.9 MB (55891041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db588734c7a8e3da8896097246345eb23edcb4069f24b1a38de4542876f761`  
		Last Modified: Sat, 10 Apr 2021 03:32:16 GMT  
		Size: 5.3 MB (5298882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb805f0843d55104ade8cf43636ecbace50cec91d8361219a4ccd38dc91cb756`  
		Last Modified: Sat, 10 Apr 2021 03:32:17 GMT  
		Size: 11.2 MB (11249056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f792ccb623310e77399e5071c2d61f3ac84305d1244893192549e89400ebdafb`  
		Last Modified: Sat, 10 Apr 2021 03:32:49 GMT  
		Size: 56.2 MB (56195089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a748536a60ffdf4fd51f59f353f1c6a584ef72ea76dbb5c6361a359fa8447`  
		Last Modified: Sat, 10 Apr 2021 03:33:45 GMT  
		Size: 199.3 MB (199318100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ff73022f677b789c980c2de3e155df99d85e4fe026becf5c7a69a13fb055e3de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301563351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a393ff6b5c68205031539b18f4cadca564d3b5a46cb657f358123dc7b5440fe2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:10:06 GMT
ADD file:a0cb4c0af6dee6c99c3739fc2b27a4d60df79591342d18fd79bb4e38a25d28d5 in / 
# Sat, 10 Apr 2021 01:10:07 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:11:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 02:12:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:14:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6eda60e328d687e0091fed92ed18129ac8eeed03d72dd92f7941c847f05a6dfa`  
		Last Modified: Sat, 10 Apr 2021 01:17:00 GMT  
		Size: 53.1 MB (53138256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b35bc44f5e1748a146c217ae7f8eeb19f129f8171afdfb72f50c2e672425aa`  
		Last Modified: Sat, 10 Apr 2021 02:22:09 GMT  
		Size: 5.1 MB (5128904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9290332c458e552d3d40e8db4b52e91c80f460edf5da9ee4bd9e86668fe97738`  
		Last Modified: Sat, 10 Apr 2021 02:22:12 GMT  
		Size: 10.9 MB (10870902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0c1430cb8920e76053cbffc8ab83c10ecb5c076f046396b396d747c42e2d2b`  
		Last Modified: Sat, 10 Apr 2021 02:23:01 GMT  
		Size: 53.6 MB (53589224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c25459c6df1e5ba51d6ed513c9d939e2a6ed612bfa8375a6e6a419db8a35e37`  
		Last Modified: Sat, 10 Apr 2021 02:25:09 GMT  
		Size: 178.8 MB (178836065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d8ba29379864e2e1098d77199f3c8d9854a8e59b95108e3933b9b0d65aaf228c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.6 MB (330627533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96a51a742f5b007303cb3342189c8c9f609209bc3f391ea3eb6be5144756d103`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:27:11 GMT
ADD file:a41b62f9bc6147a0ab13a91e4ce5169739d220f716dc3752d7c872c9bf22748b in / 
# Sat, 10 Apr 2021 01:27:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:47:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:48:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 02:50:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:00:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:907e6a464bad63c32df38aaa0e848e3e09634237527afb1f8728bda2038576ed`  
		Last Modified: Sat, 10 Apr 2021 01:34:23 GMT  
		Size: 58.8 MB (58777775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d1d0df065cb2c84ba66e763425b139d7dc18eb050bf8cc5cb8dca7e25ac80b`  
		Last Modified: Sat, 10 Apr 2021 03:06:05 GMT  
		Size: 5.4 MB (5420160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebdfc94479ccc35bbc35f2da43ced87239a8ca75ef23ce43d8dd981eab17c3a`  
		Last Modified: Sat, 10 Apr 2021 03:06:05 GMT  
		Size: 11.6 MB (11621184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06204118184dc1ec0a05e69ba94ad3152a6c5fa8e3733a6d1313099c5e2d273d`  
		Last Modified: Sat, 10 Apr 2021 03:06:28 GMT  
		Size: 59.1 MB (59138557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b97ca8796491eb99ef9274a70264dbc885bdf756788698b902aebcff5c121`  
		Last Modified: Sat, 10 Apr 2021 03:07:21 GMT  
		Size: 195.7 MB (195669857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:88959a2e39a2e87711e39a570e5232c172a0720e4e39fa4ee1f0cd4f2fc33e32
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.7 MB (295694757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e91000c7cfe8ecfeddb072a9511e59705f18031653402ae7dc3f909821c979`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:33 GMT
ADD file:95fd1353430dde759ab86e64384180601d2eec1359d5a81ebeb58e17b8998353 in / 
# Sat, 10 Apr 2021 00:42:36 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 01:30:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:30:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1b22aeeaee0a7589a5b67e1a3571ce4d1a0942461ff2075b104514fa1967711d`  
		Last Modified: Sat, 10 Apr 2021 00:46:02 GMT  
		Size: 53.2 MB (53155408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9ca0514c5f0614720863667ddd96ff334dce5555e8ae2112bed88bfa4c6711`  
		Last Modified: Sat, 10 Apr 2021 01:34:29 GMT  
		Size: 5.2 MB (5151136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe0daca911ede51529950150d6623adb8cf7f5d56b37a6dcb3e07ee55232054`  
		Last Modified: Sat, 10 Apr 2021 01:34:29 GMT  
		Size: 10.8 MB (10758740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f202156cce94de4434decbe56b2df6c30d6939cd5413272e421aa0edb064219e`  
		Last Modified: Sat, 10 Apr 2021 01:34:42 GMT  
		Size: 54.3 MB (54256990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afd2e43891e8d13519a0b8b4f80950dcb9584a442fce2f7f44e0333c603e212`  
		Last Modified: Sat, 10 Apr 2021 01:35:08 GMT  
		Size: 172.4 MB (172372483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
