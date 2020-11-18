## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:e3a105e60c8b495babdb8f1af34a2aa20ea872cdb8b7012c38d640aab577d54d
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
$ docker pull buildpack-deps@sha256:22c1e534c3e578517b1ea760e01644e61a3b7740d3103e4f40fc154e707eaf29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.5 MB (566505226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c1cab691ffc57745b6e37b92106d9a56c5f99afa144a4b616b118be861e067c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:09 GMT
ADD file:e5210ca55e6714aec9564543eeb4b4a748c57e62c0ae0c741dd0f3eb75ab72de in / 
# Tue, 17 Nov 2020 20:23:09 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:39:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:40:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:40:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:42:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:648de6ce4c8700aa65bb00de61082bc80448ba5410d2558ccd0f8c5e5616dbdf`  
		Last Modified: Tue, 17 Nov 2020 20:29:13 GMT  
		Size: 56.0 MB (55978493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330a58a1358b2808071560abfa71693ca944d1732a1543c107859d521b29bd65`  
		Last Modified: Wed, 18 Nov 2020 00:52:36 GMT  
		Size: 5.1 MB (5063542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3e6e253f47148f777fe41db1237b0eba7f14df71ec26f973f35c05182b4173`  
		Last Modified: Wed, 18 Nov 2020 00:52:36 GMT  
		Size: 10.6 MB (10646140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae65daff77b5d6ac0619bc955c2b1edd6ad35d46f9ad26b02f3de5bcd0951da7`  
		Last Modified: Wed, 18 Nov 2020 00:52:58 GMT  
		Size: 53.8 MB (53755325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155b9a2d4912e6c32ac6b9883f0eab9b129add3d6156e21d1d7cf0df74321895`  
		Last Modified: Wed, 18 Nov 2020 00:54:28 GMT  
		Size: 441.1 MB (441061726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fbec7ed65257a82d882027da954d3bf7352661c8673ea9ba740d6b49faff4dbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **523.4 MB (523374646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c7e03bf3b61a702896a81cfe4ebeddaa430b85e557e473a9d91d006ff9a2c73`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:25 GMT
ADD file:48fdddee7022ba5a0519e9f9dc9a63dd483e5294d0cfed9db93b066547405eec in / 
# Tue, 17 Nov 2020 20:23:27 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:54:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:54:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:55:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:58:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5730ec2f66f57a119aa59f80f288eee4fa0a1adebe48e9a184400d277b84ee2`  
		Last Modified: Tue, 17 Nov 2020 20:33:13 GMT  
		Size: 53.5 MB (53546003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7216d292993333f9d256b5efb205324811bb27a35f161c01af5690ebc3c5dd10`  
		Last Modified: Tue, 17 Nov 2020 22:11:18 GMT  
		Size: 5.0 MB (4974955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97e0fda183c339defd615cf109c141a20426f4d5020d3d97bff391567c03d72`  
		Last Modified: Tue, 17 Nov 2020 22:11:18 GMT  
		Size: 10.3 MB (10332185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d725a7f9c1177aabadd58343e4662e541fe14a80a7e2aba6fe018f23b442c`  
		Last Modified: Tue, 17 Nov 2020 22:11:45 GMT  
		Size: 51.5 MB (51499425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc6bd1cd9202b161cf27baa28cc98046a9a71fce76fe9d8fbd6e1a4f8578294`  
		Last Modified: Tue, 17 Nov 2020 22:13:56 GMT  
		Size: 403.0 MB (403022078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9ff56b64ca89656e9aea98d0b217e5e8fc8084f0d9356e7d1425c3e096ebada3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.6 MB (509612561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:862c88fa5eac2592a6e17b3a943130f48e710c1ed773a4b26e4cba57cbfc0e51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:06 GMT
ADD file:7bc088cc808b76314a338212bb2b1cfa40e3747a587709f883b0b3d24272ed5d in / 
# Tue, 17 Nov 2020 20:24:08 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:52:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:53:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:56:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6540e01ce43e9b114890e344f5358356defa70d487f91c1a002e0a64db73d60d`  
		Last Modified: Tue, 17 Nov 2020 20:34:10 GMT  
		Size: 51.1 MB (51125953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba56633e4f20c85ff3a7a96ebf325e3b8eb38ce01b4a19d147fba95c41307d6`  
		Last Modified: Tue, 17 Nov 2020 22:10:06 GMT  
		Size: 4.8 MB (4838976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3f95259ef99cc96a3d8352c48117cd75a72bbd30aa5c3198adc601ee244ce8`  
		Last Modified: Tue, 17 Nov 2020 22:10:07 GMT  
		Size: 10.0 MB (9971322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fe46831ed801ac2a919749edc60b1551dfa37d991390ce0b16b36fcca04a6f`  
		Last Modified: Tue, 17 Nov 2020 22:10:29 GMT  
		Size: 49.5 MB (49497168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c172ac7e8a4ef4c1b11bc92836ce1d82ea811d4ca3c8122c18c4b1ce651735d`  
		Last Modified: Tue, 17 Nov 2020 22:12:36 GMT  
		Size: 394.2 MB (394179142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fe2ca744afaf8b05bd61b87a692f26e6bff4bd81bf419a3704b0aef228ca4b51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.3 MB (542337960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d48d27c58f4e0d671c7f4cbb8abb7f00892116b3108ebdd9c55e30496173c863`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:57 GMT
ADD file:dd38237d30f418925f9d05a463817130964bc613d39a38eeea7b87b9b5d62608 in / 
# Tue, 17 Nov 2020 20:25:15 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:24:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:24:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:25:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:28:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28adf41b7f9d0f64232c0970a16416d0ef2eaa00df57f3caf5d257ccbd3b206c`  
		Last Modified: Tue, 17 Nov 2020 20:33:04 GMT  
		Size: 54.7 MB (54719929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516539a7ff1b41bcd60f56a25019366722df8db637f7a409ba85ab9918633b31`  
		Last Modified: Tue, 17 Nov 2020 22:38:10 GMT  
		Size: 5.1 MB (5055909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58beb0eca7357870a7d9572e6897310b7dbb65ea59a9f76afc5b75a63c11820`  
		Last Modified: Tue, 17 Nov 2020 22:38:10 GMT  
		Size: 10.6 MB (10648403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffef1fd67608c1c75fe7d564719a6e2a098fe43f43dfddc1dac311b1fccbd61`  
		Last Modified: Tue, 17 Nov 2020 22:38:34 GMT  
		Size: 53.9 MB (53856622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bddf2c576d92722b49ba9e3fa4118f5d40203cb0a93d662a0bef0608dd5337c`  
		Last Modified: Tue, 17 Nov 2020 22:40:25 GMT  
		Size: 418.1 MB (418057097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b4f48f5081530f06a9688d64f0b6886611d0db989156ab446429327cbae3aa72
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.6 MB (327584509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38ec6dc2e66a432e7b8ba09e78000c8a74114de074c4f64de702767626aa22a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:59 GMT
ADD file:6d6afa8490ae5ac639c8369b0f5d9f8e49c675672ebd5348a955a3c9656453f5 in / 
# Tue, 17 Nov 2020 20:22:00 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:17:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:17:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:17:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:18:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be81561500ea27b67d364b1567d73e6fbfac19e1739e5b1e5674dbea758abedd`  
		Last Modified: Tue, 17 Nov 2020 20:28:52 GMT  
		Size: 57.1 MB (57102236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc436cb880e1d23236f4f748fe380b16b0e16955049a2c0c1ab65456f67c2a49`  
		Last Modified: Tue, 17 Nov 2020 21:26:18 GMT  
		Size: 5.2 MB (5183137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca3e53afca84ddbe3333e0b6c779a68bb454199b167cfb74eda23f74fbea675`  
		Last Modified: Tue, 17 Nov 2020 21:26:19 GMT  
		Size: 11.0 MB (11022846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97dd1237dfa1a40c9c2255e2dcdec27f7d739925bf6b97716b25759ca483baf`  
		Last Modified: Tue, 17 Nov 2020 21:26:43 GMT  
		Size: 55.1 MB (55068291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cd3cf76c418768fcf3ace450c7c1799978e869f11ca050afa9e8bd5cf872cd`  
		Last Modified: Tue, 17 Nov 2020 21:27:39 GMT  
		Size: 199.2 MB (199207999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7b8f0471a4f769332705b24e14f30a18031a62d17dbb408d984f5839caed8bf2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306299582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3c07dbb49ab80847b62448b9b1155e78b6e8b25978bd9ca8f0390ec1279b445`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:54 GMT
ADD file:e6702c456d50f8685a251f68c8f1ef26036f57dc2b0b3ee32a713a0fff6192eb in / 
# Tue, 17 Nov 2020 20:19:55 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:44:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:44:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:45:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:47:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15e7eab80614971302cc43d79249de4c2eaedd05f7ae229c90002e6998c37745`  
		Last Modified: Tue, 17 Nov 2020 20:27:23 GMT  
		Size: 54.2 MB (54247133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb52b20dfb96ec0abe6e94d1493602c96b8050c535a911f580f3723be5bd3b7`  
		Last Modified: Tue, 17 Nov 2020 22:55:28 GMT  
		Size: 5.0 MB (5026356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe047368d6844c3bab8d888c6322017279e7a1ab2f8537217ab3e70de38f39d4`  
		Last Modified: Tue, 17 Nov 2020 22:55:31 GMT  
		Size: 10.7 MB (10652949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6065e8232fefa2254da6923065a6ed63fedf4ac24ab6065b69e66160d7d9b`  
		Last Modified: Tue, 17 Nov 2020 22:56:22 GMT  
		Size: 52.6 MB (52593605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8695c65d63b385ac6c8fcea862f02d5f3df1f05856a584a689daa7b3d6cebfee`  
		Last Modified: Tue, 17 Nov 2020 22:58:51 GMT  
		Size: 183.8 MB (183779539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c790cac0e67af756b066d8db3d2e787dccebec0d490b91a4c0c51d7c7b050c6b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.7 MB (343692905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864e1b70bf49af43c11b8612d98af166b3873d1d8df3f9f9c5044f14d5923e0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:24 GMT
ADD file:7998a5d3f49a86501eb252e7dc54464d086e8239a5f918b15cd85dd11e7341bb in / 
# Tue, 13 Oct 2020 01:39:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 09:10:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 09:11:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 09:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 09:27:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ab405c79eb283d457b4f978511bbef215699b366c926b3450f2a7cbc6a56e33b`  
		Last Modified: Tue, 13 Oct 2020 01:51:11 GMT  
		Size: 56.5 MB (56495338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38962ab4f4d37e5644006dc2c9a5a9b270448a5ea5ea29a387f4c7955497875d`  
		Last Modified: Tue, 13 Oct 2020 09:38:29 GMT  
		Size: 8.3 MB (8329668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8ecae68ecea0d3add456e8b38f9eef46b95731e6dfca00f430a45a774f2a19`  
		Last Modified: Tue, 13 Oct 2020 09:38:30 GMT  
		Size: 11.4 MB (11392727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfde9fce3dd7addbd894e0669be922a792dc5fa95b3ee33ffbaad4ac26cb393`  
		Last Modified: Tue, 13 Oct 2020 09:39:33 GMT  
		Size: 64.7 MB (64729412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d46a45659245d475e634ade7dc1cd46dae49e65a557b9b0552bff519712e46`  
		Last Modified: Tue, 13 Oct 2020 09:42:27 GMT  
		Size: 202.7 MB (202745760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:abbdb7e384411781431c305247b369a61269649ec02d8b201ac11fc3777100e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **510.9 MB (510921829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6c3c068ad9811cd38d613bdf5b65bb647ec3fd9c80cbfd7eb5af91d6081d0b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:51 GMT
ADD file:8962f20bb4a72e135379229e0846f699624835b74ec331608abaaebb561f33eb in / 
# Tue, 17 Nov 2020 20:19:00 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:36:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:36:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:37:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:40:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea0b76bf69e10e271efafd881a3e6209b856a27b396fee1fe5c96626da5668da`  
		Last Modified: Tue, 17 Nov 2020 20:24:00 GMT  
		Size: 54.2 MB (54214424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6fd966df630924882593f8be50b60b4dd8cbe08956bf3a1a09ab0c62129fa`  
		Last Modified: Tue, 17 Nov 2020 21:54:49 GMT  
		Size: 5.0 MB (5048615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5387e7afec1cae76ed6c62c9f9b187efd32793da95a21fba4cd0099aa37002c`  
		Last Modified: Tue, 17 Nov 2020 21:54:49 GMT  
		Size: 10.5 MB (10514414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358c5f7f1a0229f7d7aec3a9cdf564e0198552849099d872ef5cd94e80b63ed`  
		Last Modified: Tue, 17 Nov 2020 21:56:08 GMT  
		Size: 53.2 MB (53231631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8375bf98082acb7f65827d26c59492e9ad2322e1a5627d0040f30d99de0f275`  
		Last Modified: Tue, 17 Nov 2020 21:58:41 GMT  
		Size: 387.9 MB (387912745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
