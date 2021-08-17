## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:92ad4d41c3e1746f49afc7c796d54d74271d0a1fbb77099f396f480cb09466cc
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
$ docker pull buildpack-deps@sha256:2865e94ffbf88960daa4af07b1d50ec3d00715f8b2563045bd047f62522439fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321925098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb010b4b2da09832662cd74b0ea42312d686b1d1178518a9f6b7eca48120d7c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:02 GMT
ADD file:fca2ea6b8fc69f3efb8a2f21cd3877d23a9ee3fbeee6ebe4fe21541cd1606a8c in / 
# Thu, 22 Jul 2021 00:45:03 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:10:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:10:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:11:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:11:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a72d62e9d2fef13cf62e5d212cc6a3751b5c388cc6657bebf4dabc0ca3603cb`  
		Last Modified: Thu, 22 Jul 2021 00:49:21 GMT  
		Size: 54.9 MB (54904849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f297180bbe0db88491e987de8d4d906a7563841410d6277d4c2521f468f99fc`  
		Last Modified: Thu, 22 Jul 2021 01:18:44 GMT  
		Size: 5.2 MB (5153121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e579aa043ff0aad70960242128139ee1794c78c546a95105867ece202df88e`  
		Last Modified: Thu, 22 Jul 2021 01:18:45 GMT  
		Size: 10.9 MB (10871661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdc07b7fd300200574dc6b90e8ea9a32d74f4ea4b636dd9345a7ba9eddb6d63`  
		Last Modified: Thu, 22 Jul 2021 01:19:04 GMT  
		Size: 54.6 MB (54568159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2450ed8a1856eb310ca302fcfa71a1892d2190d3f2f609654d64ccf340805ea0`  
		Last Modified: Thu, 22 Jul 2021 01:19:41 GMT  
		Size: 196.4 MB (196427308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e9821bef415ec38dc109b600d28cf2ea4b8f63678bcfada6283712350c117860
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.0 MB (295024569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f973d20c18c5d7ac30b1bce9c189db4ea4bba4e8a526b91546c5169a2925668d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:48:40 GMT
ADD file:a5e191f39728e6e12b8f32edbaa7920930ceeaa50bd5db8a28faa1325a03c877 in / 
# Thu, 22 Jul 2021 00:48:41 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:58:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:58:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:59:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 02:02:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54f61193f2822104b288f4b662f2a516401b23e0fba11d7ca2215f06378c96fc`  
		Last Modified: Thu, 22 Jul 2021 00:59:59 GMT  
		Size: 52.4 MB (52443094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fe553c5962741d3f2886a01d834839adf275ab459fc0e141cb7923436d736d`  
		Last Modified: Thu, 22 Jul 2021 02:17:54 GMT  
		Size: 5.1 MB (5063630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3979ca68793ff901e46109197cce75ef32b748868c9828a1553e9884e1646bb2`  
		Last Modified: Thu, 22 Jul 2021 02:17:57 GMT  
		Size: 10.6 MB (10570938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e97cdc24ec30abe03f9627670d9c6fdc1a0ab29f0b07f7fa88f04bf60d82cbb`  
		Last Modified: Thu, 22 Jul 2021 02:18:47 GMT  
		Size: 52.3 MB (52318648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a46ddac3df295ee8e35b6704c741dfbcf346fa8431efaf9458f83ed7e6de5b0`  
		Last Modified: Thu, 22 Jul 2021 02:20:44 GMT  
		Size: 174.6 MB (174628259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e43f9c3ff4fe6195b1091dc06784d1cbe2ba5eae372eff9b19cc8b346d379403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282456279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cfb293581719ebb6d8a0d06485cd678e6270a3d3d561378acdd5a634609837c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:02:14 GMT
ADD file:e95bfea309b4c4cf7a3a7367d3a3ed606af0f897282dd0e3e2effd01a126625f in / 
# Thu, 22 Jul 2021 02:02:16 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:11:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:12:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:14:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b19ab02b95dd8c04699b4e2ac6ee9898e2f6813d01c5c529b1e3f2dd356d20f`  
		Last Modified: Thu, 22 Jul 2021 02:14:18 GMT  
		Size: 50.1 MB (50107629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81af848fbd4d3452ddcc81144117920629d972b86a2b2bfc2349748414ff4546`  
		Last Modified: Thu, 22 Jul 2021 04:32:44 GMT  
		Size: 4.9 MB (4922411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81674fdc924b9599aa9fa846f071e5ac2b8c8ab99bfd65c19012a451e9aa1eba`  
		Last Modified: Thu, 22 Jul 2021 04:32:45 GMT  
		Size: 10.2 MB (10216644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924737dbe8bd51d178f074d900158220c63f442163fdb975f36a832d0615cf50`  
		Last Modified: Thu, 22 Jul 2021 04:33:32 GMT  
		Size: 50.3 MB (50328774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b86974a59071a96688eaf30f61f2865b635bb5e1edb0740440f7532cb32a0`  
		Last Modified: Thu, 22 Jul 2021 04:35:15 GMT  
		Size: 166.9 MB (166880821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a4132ed08f2c986f6ec257b1ef23540124a285a349be620f3635f4314d61934e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313593955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c94465a6d19277b6bf42c6c09889ddbf2dd50b044c71ed3ffb95ed9eefb4e33`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:37 GMT
ADD file:6733d7f2201aa0027287de4f81a7cabfb79c331e290d9d1f16bc68c8c0ce1473 in / 
# Thu, 22 Jul 2021 00:39:37 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:14:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:14:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:14:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:15:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2fd60d6781333dbb2e2b453027f2c16737edf4afa6edc775fbe4983c9196c83`  
		Last Modified: Thu, 22 Jul 2021 00:44:34 GMT  
		Size: 53.6 MB (53590358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6475276876369c675045edd5275dfaf6d54f4ca13a77dd33835b145e4f6dbfc4`  
		Last Modified: Thu, 22 Jul 2021 01:23:42 GMT  
		Size: 5.1 MB (5142492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1a8b85717d6fe3eedef14320b0bee76ceefdae31623ffa13a264a78ae675eb`  
		Last Modified: Thu, 22 Jul 2021 01:23:42 GMT  
		Size: 10.9 MB (10872686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194bb6aa613f903b9f28f6985407c4a3ef71b0c952902f6fc70c211f30b77af6`  
		Last Modified: Thu, 22 Jul 2021 01:24:03 GMT  
		Size: 54.7 MB (54670808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd73d027bde243be7edb114a83b97069b192d4951b03597d73755310fea8516b`  
		Last Modified: Thu, 22 Jul 2021 01:24:42 GMT  
		Size: 189.3 MB (189317611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3e152f603c64c239dde1a9d75a3a5f7a1524b39b374818b31c805e692f072f20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327735799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ffb8cbbe451dff3ed35bd8100f53511feea78881731c1104163ff43f458acb1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:39:59 GMT
ADD file:9a18b2fe412d515e1cddf03975540bdf3800e8016d3f9a11f1540e5a44c1daa3 in / 
# Tue, 17 Aug 2021 01:40:00 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:57:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 01:58:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:59:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37481791ac63726d7596e6cc5512ba4153b294411573b617bc05d7179bfa2013`  
		Last Modified: Tue, 17 Aug 2021 01:49:20 GMT  
		Size: 55.9 MB (55922543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2beb9a3911783fb09a57b7bf2557a3acbe8123c446facf41a911545fbad89773`  
		Last Modified: Tue, 17 Aug 2021 02:08:01 GMT  
		Size: 5.3 MB (5282917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dc787fb26009442922f6cffec3c97af8ef1dfe851d1ee79a41349bc5ecd753`  
		Last Modified: Tue, 17 Aug 2021 02:08:02 GMT  
		Size: 11.3 MB (11250663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac24f179d09aaaee41253d80af84046a4c7653d8c464f340d58629307400078`  
		Last Modified: Tue, 17 Aug 2021 02:08:30 GMT  
		Size: 55.9 MB (55916250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d487982b5dbdf2dbd1a8a842e99d3eacec4491cea06b5aac42336a23acfafc`  
		Last Modified: Tue, 17 Aug 2021 02:09:23 GMT  
		Size: 199.4 MB (199363426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e16e2d4e4a3519349ad0295b0dc53ddba873db7ae01b81f2d0dcbcd6e3e98439
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301361292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f9c9606738b94d4a7f4a80bbf937160372daecbdea46d1da419b5712a481ab`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:08:32 GMT
ADD file:0528720276c3b3b11a00595363f8a514e2655bcf1e4d9b8ba3f79621e44f0460 in / 
# Thu, 22 Jul 2021 00:08:32 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:37:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 00:37:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 00:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 00:41:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf851126a635ad4c2c2a139ad19f922e1a4ce737641a782c32519868f02d804d`  
		Last Modified: Thu, 22 Jul 2021 00:14:07 GMT  
		Size: 53.2 MB (53156287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03208a775bdcf86ef328e8eaafb6230b1df65f5e3f7134dcb25e12a4148a24e4`  
		Last Modified: Thu, 22 Jul 2021 00:50:55 GMT  
		Size: 5.1 MB (5114712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afb8c727f6f423fc30a90decf5892b3aec16edcd914824275b6e0b56e6a3dd1`  
		Last Modified: Thu, 22 Jul 2021 00:50:57 GMT  
		Size: 10.9 MB (10873290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1798d788f2501ab1d9d5cc30f8b8d75d14f031ec0a34d2e5ef594c7e01a42c7`  
		Last Modified: Thu, 22 Jul 2021 00:51:46 GMT  
		Size: 53.3 MB (53298870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6376da5a25a254e0b6f4ec707d523fd883ebd6cc1add434f9b634d55b3c6ce7c`  
		Last Modified: Thu, 22 Jul 2021 00:53:54 GMT  
		Size: 178.9 MB (178918133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7b502db10364d9d204efca694a8c63c0f39a731bda2584a353152d7f65fded68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330473673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3316f715b461eab05f49e087d0030fd280ec614936749f437ca0412fe6afd6e3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:17:09 GMT
ADD file:aadb38c47e4a40c11e7ad3b380075dadabb62c20584e02f089c2e5c957ce04cd in / 
# Thu, 22 Jul 2021 00:17:19 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 03:44:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 03:45:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 03:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:00:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0acfc4b0736fe9b7465e9b5f83f277c5a237585bf07da22048883229ecafad7`  
		Last Modified: Thu, 22 Jul 2021 00:26:21 GMT  
		Size: 58.8 MB (58813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847221653bad212b7cc4f12cc2ae7b27ddbe29dce9a8988bdf32b8df41945d4f`  
		Last Modified: Thu, 22 Jul 2021 05:10:01 GMT  
		Size: 5.4 MB (5401706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92fec3eb594016967ad2f4e5bbef1754a9733c560b8449f5e56969c8486d27b`  
		Last Modified: Thu, 22 Jul 2021 05:10:00 GMT  
		Size: 11.6 MB (11625843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134c811e4424a1c4ddbf1f572dd8c99171109b77c4669802dc6882335b1bff31`  
		Last Modified: Thu, 22 Jul 2021 05:11:07 GMT  
		Size: 58.8 MB (58849943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3aa50e2834feeb56616af31a9d68c8e13130078bf2333faca937aeda872664`  
		Last Modified: Thu, 22 Jul 2021 05:13:18 GMT  
		Size: 195.8 MB (195782865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cf01269e05d9303021ae3c138477ad9332499622e7f234ee6574c969b9ebcc04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295539906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:462936f542e1f107203f647da81c089a8230a673ba9f79ccc2a06cc3710696b7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:34 GMT
ADD file:0a2fe191e4bb0a90f32a0829f6d49407139fa2c3517cc2097c51a94786075a8e in / 
# Thu, 22 Jul 2021 00:41:41 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:06:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:06:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:10:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:431c45f9c46bd0833127af2c090d5f6776b5c421df2849de5f3071102212923c`  
		Last Modified: Thu, 22 Jul 2021 00:47:15 GMT  
		Size: 53.2 MB (53183556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661dc83d23d8e8891a8b01ec648db5ba5f59655fd1afd8c0be9ae256c3f9840a`  
		Last Modified: Thu, 22 Jul 2021 01:26:41 GMT  
		Size: 5.1 MB (5136979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fde1e2e331c02b4294f5f9f803a4aa4f31be7389c20abd265788d916aa771a1`  
		Last Modified: Thu, 22 Jul 2021 01:26:41 GMT  
		Size: 10.8 MB (10760969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93975c70cfc2cdc91261d061f2a72ad8ea1d64b7834027ba9d534e3f9e10cff`  
		Last Modified: Thu, 22 Jul 2021 01:26:59 GMT  
		Size: 54.0 MB (54041879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83127f4fa5b07cbde07f22a2272d6bc4172f4591b959478bbbc6067dfed15e55`  
		Last Modified: Thu, 22 Jul 2021 01:27:31 GMT  
		Size: 172.4 MB (172416523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
