## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:7a78a5f716dd32b0eb89876f8c5cf5e443781a44b7fe12619e897bad9a642e14
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

### `buildpack-deps:bullseye` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ab6dffecec57be69a421462c301496a0ca0b59538ebdc65e7360dd7ecacf15d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.4 MB (322380770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368c349ca3b0f384f4c46f97c604fb259085cb760c73d759aa8e8dd4a6f29a09`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:16 GMT
ADD file:798015650079cb88614ff181a30f9c3d3fde8361c49ae2dec2058d5a3e61f5df in / 
# Thu, 23 Jun 2022 00:20:16 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:50:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 00:50:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:51:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1339eaac5b67d16d6d9f41fb7a7b96f7cebf3ba4beab36cbb60935aa772af583`  
		Last Modified: Thu, 23 Jun 2022 00:24:48 GMT  
		Size: 55.0 MB (55009886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c78fa1b97999d08408734a61040475ade5bd7e33e91c0d5170dba2c7c7a92fd`  
		Last Modified: Thu, 23 Jun 2022 00:58:38 GMT  
		Size: 5.2 MB (5155961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f0d2bd524377dc42d072443c0e5e7cafa14f5df609d39bb1f717f43817a2cd`  
		Last Modified: Thu, 23 Jun 2022 00:58:38 GMT  
		Size: 10.9 MB (10875087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e5964a957d206950c8c0de99f3c491ecec78887ebe4df0ac5ab9ceb536a4d5`  
		Last Modified: Thu, 23 Jun 2022 00:58:59 GMT  
		Size: 54.6 MB (54577874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4bb1a04a94a9015f79b0d36ee942b63bd486da0ef79689d4326398b561fa3a`  
		Last Modified: Thu, 23 Jun 2022 00:59:36 GMT  
		Size: 196.8 MB (196761962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c29f52f6d830d981e447464ddb8f48ce8dd58b0fefcb246ecc2d30be965f8982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295449929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebb5778a402d18e8a7646fc1240b85fbc1b59d9f7b5412a26bd96e98c167af23`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:04 GMT
ADD file:a9a29412ef2a46df9ac08c0263e1fd3872777bcafdf6f172dae904af96ff7585 in / 
# Thu, 23 Jun 2022 00:50:04 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:37:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:40:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4031f48ff7c3b7223afff91721ded4a4de5f7c666f84c58a5d8298dd0fe028`  
		Last Modified: Thu, 23 Jun 2022 01:04:50 GMT  
		Size: 52.5 MB (52541138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81d328795b20b164711abd9d265ebf98fa864c36cc2ac7b79fcde10ea683a47`  
		Last Modified: Thu, 23 Jun 2022 02:01:21 GMT  
		Size: 5.1 MB (5065402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df15bbc2ab79e81b31649e3d85b8e92141abf53487afd2e2dac38a9889b4d3`  
		Last Modified: Thu, 23 Jun 2022 02:01:23 GMT  
		Size: 10.6 MB (10573065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6277f05327b720d120a7609bad575356aea3c0f1ce8901aa52717c2f196ffb56`  
		Last Modified: Thu, 23 Jun 2022 02:02:17 GMT  
		Size: 52.3 MB (52315681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bcb5356225f839cd3d29f5be0f1b7818d19c263fbbb1187e7b9237f0f1c526`  
		Last Modified: Thu, 23 Jun 2022 02:04:18 GMT  
		Size: 175.0 MB (174954643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9254d3229a35f42338ff7933346785a2d268db84b9efe143b5ca270971de62c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282907275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881d9d15dd210ddec3516b51b6771f5e9de611d23d00d6480601a41fd23b68f8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:08 GMT
ADD file:59a6186285c4849971ea2d4801e6ebc1e4310f5e3dc0f87389f39d1fa8a63c58 in / 
# Thu, 23 Jun 2022 00:59:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:46:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:46:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:47:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:49:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2147df557f50051066d8920b460727b890c1da5cb2c15b055c99ed8216b5528f`  
		Last Modified: Thu, 23 Jun 2022 01:14:34 GMT  
		Size: 50.2 MB (50199604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b28303e18c4d3b1788071e1a67ed51ad28c9574bf30371176fc152638acdbe`  
		Last Modified: Thu, 23 Jun 2022 02:13:15 GMT  
		Size: 4.9 MB (4924846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536c76bf1b84e75e4834c8b50a6f3697460303c4b2021434891103b94ca78fac`  
		Last Modified: Thu, 23 Jun 2022 02:13:17 GMT  
		Size: 10.2 MB (10217964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72032391c22caab41b7e492fc3cac93cd17f7c920e05ff5c34031a544a4a833e`  
		Last Modified: Thu, 23 Jun 2022 02:14:07 GMT  
		Size: 50.3 MB (50329194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce902e7596eca4913ba3977a3f359a5df0ee13c148538d24d880f6687ee8ff1`  
		Last Modified: Thu, 23 Jun 2022 02:15:51 GMT  
		Size: 167.2 MB (167235667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ee9d891d5be5a4e92eb903eb541f1315853946c390211e455c00c983e8f2e79c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313627175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a99833e972dc9d2c86f5b2f2f1e510e566c3cef70c15fbd65da6c875133f80`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:28 GMT
ADD file:64c455af1bb18ff2c202a244e058b6e5ac147b89410ed36edc5e29f4b6f02c5d in / 
# Thu, 23 Jun 2022 00:40:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:11:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:11:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:11:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:12:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f873dfbc59b181817d5bc2b9fc31d90d8f9139c8cabb2fa7264f9bd7b418b8d2`  
		Last Modified: Thu, 23 Jun 2022 00:46:51 GMT  
		Size: 53.7 MB (53696815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7b65e0e9cdc28c8cedaabbc5cbae4652c9b107c47684de49f01a77741a5ded`  
		Last Modified: Thu, 23 Jun 2022 01:21:51 GMT  
		Size: 4.9 MB (4938760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43836e7983cba8b758620a218a0ee622daf5513308b6a9e8316f94c271ecafd`  
		Last Modified: Thu, 23 Jun 2022 01:21:51 GMT  
		Size: 10.7 MB (10656970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1209d2973c25405a6c092fa82923495c9cbf17ea31b92f3c5f9dc06d85c19a4`  
		Last Modified: Thu, 23 Jun 2022 01:22:14 GMT  
		Size: 54.7 MB (54673319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edd6fb868024e48c0b412c0ba8cbeb86125cca0fff8290da30d868475917dc2`  
		Last Modified: Thu, 23 Jun 2022 01:22:53 GMT  
		Size: 189.7 MB (189661311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:da6ea6fc7a4cc67d9fef8ba965b11344d5f6183bb1e66ce24ac808e9695ed9f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327723280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:650c2caa5dbdf8da48f8d7d860d8cc92d351f5440c13c606b8d5e0d4e3e36e6f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:17 GMT
ADD file:38ad8e7562f238cf436c2a32b21b397a0ad3dd5c8f68f29bc724458cad18a47e in / 
# Thu, 23 Jun 2022 00:39:18 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:11:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:11:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:12:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:12:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bfd9a7ec075cef3ff84a270710c704347f9a866aeb50e5a286491696168d5f5`  
		Last Modified: Thu, 23 Jun 2022 00:46:04 GMT  
		Size: 56.0 MB (56007522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45f3c7c07e8e6bb9d2c30f8b932d9db0300b97850bfbf921a5b56ebefa99769`  
		Last Modified: Thu, 23 Jun 2022 01:22:14 GMT  
		Size: 5.1 MB (5080447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f01d925e37f51b5dbeac306dc641b52957d383e5fd3d61dc8822590b97d171`  
		Last Modified: Thu, 23 Jun 2022 01:22:15 GMT  
		Size: 11.0 MB (11033739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb4b9d72cb12455c850c1823ae918d6d05a7a2052a285314d41c63c81bbc32a`  
		Last Modified: Thu, 23 Jun 2022 01:22:37 GMT  
		Size: 55.9 MB (55914398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a325e396a9724c0a906a2b3b6f2f74d2ccc7c720ef1b464f807fcfa71aa5451`  
		Last Modified: Thu, 23 Jun 2022 01:23:14 GMT  
		Size: 199.7 MB (199687174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:13c09fff1e074807595848bb4880b728c71a7b6ae8c75e49f82cdb2fc329549a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301044831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31093e199af1727f0c06cdcf58a01f1cf1e0ad07760aee6478b76c1d792f0177`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:09:48 GMT
ADD file:b4c1f4f21cc3a6a3ebc27c9c15cfab9e67c385c2df87110392754663c02722f8 in / 
# Thu, 23 Jun 2022 01:09:53 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:52:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:53:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:54:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:59:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a63618d87cd80f12f8640fecf6d13ece7ce3ac6260be88adcebe60f4da899b8`  
		Last Modified: Thu, 23 Jun 2022 01:19:34 GMT  
		Size: 53.3 MB (53273237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac43be31041e2631cd8bdabfb3934fb423e7237e142c5b86e532e192e4fe36`  
		Last Modified: Thu, 23 Jun 2022 02:19:58 GMT  
		Size: 4.9 MB (4912505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfda9893d218bf2decc23f236eb8276f1b5512b4d2647fbab36c43e9bbf96d3`  
		Last Modified: Thu, 23 Jun 2022 02:20:00 GMT  
		Size: 10.7 MB (10660150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5205b64237f8e05552a56eb9f5faffb06894bd3f477e61b3e1b2716380279e6f`  
		Last Modified: Thu, 23 Jun 2022 02:20:57 GMT  
		Size: 53.3 MB (53298997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b0c2f1d405a64bf4c2a9741495fbebc93a40357f5b2a4cb973d9a490fb51b7`  
		Last Modified: Thu, 23 Jun 2022 02:23:03 GMT  
		Size: 178.9 MB (178899942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:721aeefe3a0c447efc28198dfe19a3d3af8f593d70a109a7addd80171a4a5536
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.9 MB (330922952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dcd0098fa303a241eb35025602ad723015726c13f2a549ddafb8f99abea4b24`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 02:01:53 GMT
ADD file:8e4c382536553538abd5a62333996023e484596173131dab18020775b0731238 in / 
# Thu, 23 Jun 2022 02:01:58 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 03:54:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:00:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03691a2d4065f9ca4fafadaa8229407224c6aac10796fc0884981e6c81a43b8d`  
		Last Modified: Thu, 23 Jun 2022 02:14:21 GMT  
		Size: 58.9 MB (58903151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a26b659a43f0973605ce681b0a27a9563e32a560c64518a32cbf9284ffbe8bf`  
		Last Modified: Thu, 23 Jun 2022 04:56:06 GMT  
		Size: 5.4 MB (5405243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d46f40a862767538cfa58e9d25dca4b07caa0e31992187e566a6c24b0e11f0`  
		Last Modified: Thu, 23 Jun 2022 04:56:07 GMT  
		Size: 11.6 MB (11627442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03898d1bb379aab2aa192ab335931abcab4a1a3cb67af8d83900ba9d2045af0`  
		Last Modified: Thu, 23 Jun 2022 04:56:34 GMT  
		Size: 58.9 MB (58855018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65476b8f919067f953bff76371cbc72b97c37a96fa033b668fe7cd72731a87d`  
		Last Modified: Thu, 23 Jun 2022 04:57:23 GMT  
		Size: 196.1 MB (196132098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:05234fa63853e6c77efbf050681c93394b4cd1b1c6b6ddbb860674b2f6347408
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.0 MB (295995034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aca06da22c8620dbb261a1930b0b33f693ba8de4a9ce069e1f5c1bf51839a01`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:40 GMT
ADD file:80a08f446549ae1b71aaab0aada00625b804fd959e2a21a9c0747fb3cdb0afc0 in / 
# Thu, 23 Jun 2022 00:42:48 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:16:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:16:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:17:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:19:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e92226c94dce8ebeb505bbbebdc70207295a4a602fc736044e4e69866dc05e58`  
		Last Modified: Thu, 23 Jun 2022 00:51:36 GMT  
		Size: 53.3 MB (53276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d640cc8936c5cb6e3d305ec831be1b35a79839e07490358519cd2f48759274a`  
		Last Modified: Thu, 23 Jun 2022 01:35:00 GMT  
		Size: 5.1 MB (5140923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356e72745d061d1b1515a417d346c741fdcf0e3c58b6aa88cc86eee96ec3daac`  
		Last Modified: Thu, 23 Jun 2022 01:35:01 GMT  
		Size: 10.8 MB (10765497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f2f2ecbda16c1aa0309b44daf39322108f0e9dd6dfeaee815a8dd53cfee576`  
		Last Modified: Thu, 23 Jun 2022 01:35:19 GMT  
		Size: 54.0 MB (54045148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a279dbec4bccf345aae5f41c1b982cb7f5d871e7aebea1449dac9aa692f8bbb`  
		Last Modified: Thu, 23 Jun 2022 01:35:48 GMT  
		Size: 172.8 MB (172766694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
