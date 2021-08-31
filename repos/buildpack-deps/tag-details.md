<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `buildpack-deps`

-	[`buildpack-deps:16.04`](#buildpack-deps1604)
-	[`buildpack-deps:16.04-curl`](#buildpack-deps1604-curl)
-	[`buildpack-deps:16.04-scm`](#buildpack-deps1604-scm)
-	[`buildpack-deps:18.04`](#buildpack-deps1804)
-	[`buildpack-deps:18.04-curl`](#buildpack-deps1804-curl)
-	[`buildpack-deps:18.04-scm`](#buildpack-deps1804-scm)
-	[`buildpack-deps:20.04`](#buildpack-deps2004)
-	[`buildpack-deps:20.04-curl`](#buildpack-deps2004-curl)
-	[`buildpack-deps:20.04-scm`](#buildpack-deps2004-scm)
-	[`buildpack-deps:21.04`](#buildpack-deps2104)
-	[`buildpack-deps:21.04-curl`](#buildpack-deps2104-curl)
-	[`buildpack-deps:21.04-scm`](#buildpack-deps2104-scm)
-	[`buildpack-deps:21.10`](#buildpack-deps2110)
-	[`buildpack-deps:21.10-curl`](#buildpack-deps2110-curl)
-	[`buildpack-deps:21.10-scm`](#buildpack-deps2110-scm)
-	[`buildpack-deps:bionic`](#buildpack-depsbionic)
-	[`buildpack-deps:bionic-curl`](#buildpack-depsbionic-curl)
-	[`buildpack-deps:bionic-scm`](#buildpack-depsbionic-scm)
-	[`buildpack-deps:bullseye`](#buildpack-depsbullseye)
-	[`buildpack-deps:bullseye-curl`](#buildpack-depsbullseye-curl)
-	[`buildpack-deps:bullseye-scm`](#buildpack-depsbullseye-scm)
-	[`buildpack-deps:buster`](#buildpack-depsbuster)
-	[`buildpack-deps:buster-curl`](#buildpack-depsbuster-curl)
-	[`buildpack-deps:buster-scm`](#buildpack-depsbuster-scm)
-	[`buildpack-deps:curl`](#buildpack-depscurl)
-	[`buildpack-deps:focal`](#buildpack-depsfocal)
-	[`buildpack-deps:focal-curl`](#buildpack-depsfocal-curl)
-	[`buildpack-deps:focal-scm`](#buildpack-depsfocal-scm)
-	[`buildpack-deps:hirsute`](#buildpack-depshirsute)
-	[`buildpack-deps:hirsute-curl`](#buildpack-depshirsute-curl)
-	[`buildpack-deps:hirsute-scm`](#buildpack-depshirsute-scm)
-	[`buildpack-deps:impish`](#buildpack-depsimpish)
-	[`buildpack-deps:impish-curl`](#buildpack-depsimpish-curl)
-	[`buildpack-deps:impish-scm`](#buildpack-depsimpish-scm)
-	[`buildpack-deps:latest`](#buildpack-depslatest)
-	[`buildpack-deps:oldoldstable`](#buildpack-depsoldoldstable)
-	[`buildpack-deps:oldoldstable-curl`](#buildpack-depsoldoldstable-curl)
-	[`buildpack-deps:oldoldstable-scm`](#buildpack-depsoldoldstable-scm)
-	[`buildpack-deps:oldstable`](#buildpack-depsoldstable)
-	[`buildpack-deps:oldstable-curl`](#buildpack-depsoldstable-curl)
-	[`buildpack-deps:oldstable-scm`](#buildpack-depsoldstable-scm)
-	[`buildpack-deps:scm`](#buildpack-depsscm)
-	[`buildpack-deps:sid`](#buildpack-depssid)
-	[`buildpack-deps:sid-curl`](#buildpack-depssid-curl)
-	[`buildpack-deps:sid-scm`](#buildpack-depssid-scm)
-	[`buildpack-deps:stable`](#buildpack-depsstable)
-	[`buildpack-deps:stable-curl`](#buildpack-depsstable-curl)
-	[`buildpack-deps:stable-scm`](#buildpack-depsstable-scm)
-	[`buildpack-deps:stretch`](#buildpack-depsstretch)
-	[`buildpack-deps:stretch-curl`](#buildpack-depsstretch-curl)
-	[`buildpack-deps:stretch-scm`](#buildpack-depsstretch-scm)
-	[`buildpack-deps:unstable`](#buildpack-depsunstable)
-	[`buildpack-deps:unstable-curl`](#buildpack-depsunstable-curl)
-	[`buildpack-deps:unstable-scm`](#buildpack-depsunstable-scm)
-	[`buildpack-deps:xenial`](#buildpack-depsxenial)
-	[`buildpack-deps:xenial-curl`](#buildpack-depsxenial-curl)
-	[`buildpack-deps:xenial-scm`](#buildpack-depsxenial-scm)

## `buildpack-deps:16.04`

```console
$ docker pull buildpack-deps@sha256:bb129802c0c6057515fb72e3cea6355cb13e6014d528e081c29c6679f6a35e79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:16.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:aa9e0333df32def9001a677ff89a5c09213d91d030b4439bfe9c01153f997ca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.4 MB (236392854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd46abf564eb1523a47e8d464e3a01b07d272b68fd1538cf5d850114d417d258`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 22:03:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:03:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:04:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84cf3b385fa330cddfcec4c9fe29c02ba73e5ce4eeeb01b4b1fcc16ac1c28a9`  
		Last Modified: Mon, 26 Jul 2021 22:15:57 GMT  
		Size: 7.8 MB (7790900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc0223d40ee93a1ec66a4a4c73009a6ec0aecb2dc36910248e21b9066bbe353`  
		Last Modified: Mon, 26 Jul 2021 22:16:16 GMT  
		Size: 41.9 MB (41906076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84e4d3d55d27152a8e4f53008dd952792ba5a25c167f2da2a2040fc9011fea3`  
		Last Modified: Mon, 26 Jul 2021 22:16:46 GMT  
		Size: 140.2 MB (140196965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0d52b28c376957c832f21e2bb02fa870bf44bc3e50c55e0345dd43ecad81791e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202400746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34532f92c4963d1c6422c949b4b5892473edefeb2d84cdfc6e8669bde921cfea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:53:34 GMT
ADD file:4b9fec92db5a0e4059d8b16893d817dca169e585547a48cf5ec6d4afc56e997c in / 
# Mon, 26 Jul 2021 22:53:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 22:53:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:53:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 22:53:41 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 01:31:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:34:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba10bfe0b6395fa726456c96036b4fd8ef0513d396442e7419e81550b626b4a0`  
		Last Modified: Sat, 24 Jul 2021 22:43:19 GMT  
		Size: 40.3 MB (40312522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b2be9419691b3c616ec69316c8bef11216dce2cc63b22ba203ada71a1a1f08`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2278b7cd7720a82be011f94dfd9d056b889b12068623fc864b02b096cb01ad`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e23ab739c679be25d516008b91998dc0513145f9ecb2fa75e1c762def8699`  
		Last Modified: Mon, 26 Jul 2021 22:58:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c3f69a6d2542114190cf9d0dd3b5d65d06d1e187e7573fde2c374fb1ba911f`  
		Last Modified: Tue, 27 Jul 2021 01:52:38 GMT  
		Size: 6.6 MB (6631696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d3e4de014d1c265e7133c67440a52321689ea8c718c3367d477494159d3dcf`  
		Last Modified: Tue, 27 Jul 2021 01:53:18 GMT  
		Size: 38.2 MB (38162616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c51aec69057796c4bd045f048f4f4d9f6638c1094a0cb237a2f8e1fe2055a7`  
		Last Modified: Tue, 27 Jul 2021 01:54:40 GMT  
		Size: 117.3 MB (117292380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5f1a74531a27625f7311e1d718d1bdc2373c90bf1550d7404722ebec31712bab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.1 MB (210145891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2987f35704c7cfe20318be2c51f0f799a493368655c37bbe5d9a5c7ab9af9337`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:14:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:16:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aadea1266928a0dceab31c4c15ffe7dbcda64c245cfec8104807007655c283`  
		Last Modified: Tue, 31 Aug 2021 02:23:32 GMT  
		Size: 6.8 MB (6838692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b021524e25acee25ed838c080f43172f4fbdb58e2f2b790bec964d32b0afa48`  
		Last Modified: Tue, 31 Aug 2021 02:23:51 GMT  
		Size: 39.8 MB (39808352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c042fa608c33de9985c2b60cf95d2d0e70f2e69853346af8ddf52c6c66f0e53d`  
		Last Modified: Tue, 31 Aug 2021 02:24:21 GMT  
		Size: 122.3 MB (122258097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04` - linux; 386

```console
$ docker pull buildpack-deps@sha256:774dc09a5f250b4b70cbb9eb42070e661de99639ab0a30c44fee7feed73fc45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236627828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df62604e2ff855d073d4271194e17d7ff178fbcc55537a86bd2b88e74043d7a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:03:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:03:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:07:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdc5ad45f3591df22f6cfd8a81e806096d73e75cb53dd36f2dc06bedc29cdf8`  
		Last Modified: Tue, 31 Aug 2021 02:11:05 GMT  
		Size: 7.9 MB (7933649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcec5a27c60c6c19817288510b120bb7290e04bbf035fa5d2aacfe5a35bfc3f7`  
		Last Modified: Tue, 31 Aug 2021 02:11:26 GMT  
		Size: 42.9 MB (42891141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84dec47a6a248f9ea193b70e2bdb533bcfe635eef0b254f93e60f330b0a9d921`  
		Last Modified: Tue, 31 Aug 2021 02:12:04 GMT  
		Size: 140.0 MB (139985319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fa632f14251fc91c75fd3c600e393aa69b240b725f3f5db8e60df418550e69de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.5 MB (245531703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd55efc20b2e3259d5ad6e52ceb4fd497e83f0d017a0d9cb26e4584e56211499`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:14:07 GMT
ADD file:8fe1a1dacf1dc31e5c6168e69c34f801191864c5fece1d91b13d59807f6056ca in / 
# Mon, 26 Jul 2021 23:14:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 23:14:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 23:14:28 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 04:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:07:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 04:09:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:19:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d472a4d60588bf877b1577439fb1db8b17861b63117a33841fe29225c530b95e`  
		Last Modified: Sat, 24 Jul 2021 22:43:36 GMT  
		Size: 47.5 MB (47522379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe44c44a8ee34d79983e97d8261707445db2732ccf6a93cc146c4cdbffca5696`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333f9295db0b7ef046f754b97473c3bd3514e0d9b8465d869119004c929e5261`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c736b6f8064fe10fc657f6af155f5b9827223a418712a0397b8ca50f7f19c83`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783e2b245674c811c355b44a116453c6514c3df2c057ed3df4a19bcbf9a717ac`  
		Last Modified: Tue, 27 Jul 2021 04:29:20 GMT  
		Size: 7.7 MB (7692708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3a0fe0a58f94d243f9f5cc3c5b58818b595e4658364d01f29e074a94fb2dd`  
		Last Modified: Tue, 27 Jul 2021 04:29:41 GMT  
		Size: 45.1 MB (45147746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c524fa6303aa9878acc0d304661e148adc711d79187a5cf31e6b844c296d32f`  
		Last Modified: Tue, 27 Jul 2021 04:30:19 GMT  
		Size: 145.2 MB (145167370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c6a4196d8af17c85172d35cd32e4f8366e1b3f614217582dd4dfad72a5cc00fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.0 MB (220978033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:612b92867d5821ccf9e5e4cd95953cd4499ca8f65e1f0b7baec2bae59321550f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:41:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:42:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd8a6861a80aa4b11ce96ec3537844aec4b713e8074deacba0614cd64afaf6f`  
		Last Modified: Tue, 31 Aug 2021 02:48:46 GMT  
		Size: 7.5 MB (7522004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102f08394215864198c62652fc16666081e5739d70caea25d4324e60bcab889`  
		Last Modified: Tue, 31 Aug 2021 02:49:00 GMT  
		Size: 42.7 MB (42688096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4200eefc2db30e95286e811f3f22d74a19ee78596fc4bd4b4caf13951a63a4b`  
		Last Modified: Tue, 31 Aug 2021 02:49:23 GMT  
		Size: 126.7 MB (126678714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:16.04-curl`

```console
$ docker pull buildpack-deps@sha256:f07d52aae65670c4495402c8616ee62cd4a39fa2b7b358bac4141d3f6a7d1724
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:16.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9f00f5d40c5d93d1537e58b0b41fc863e794115201436258052f285dbff3394d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54289813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5bfdc15c4830f18177a9c3efef4bf27c4a5900199e74269856f5d796d108024`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 22:03:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:03:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84cf3b385fa330cddfcec4c9fe29c02ba73e5ce4eeeb01b4b1fcc16ac1c28a9`  
		Last Modified: Mon, 26 Jul 2021 22:15:57 GMT  
		Size: 7.8 MB (7790900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5b3b0321d5806a2005a003d6171ca78704b4f354555180850039715adbebd129
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46945750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2794a265e57db998e79510b2a0959572659242687202607c0194f8c56c4c0724`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:53:34 GMT
ADD file:4b9fec92db5a0e4059d8b16893d817dca169e585547a48cf5ec6d4afc56e997c in / 
# Mon, 26 Jul 2021 22:53:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 22:53:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:53:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 22:53:41 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 01:31:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ba10bfe0b6395fa726456c96036b4fd8ef0513d396442e7419e81550b626b4a0`  
		Last Modified: Sat, 24 Jul 2021 22:43:19 GMT  
		Size: 40.3 MB (40312522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b2be9419691b3c616ec69316c8bef11216dce2cc63b22ba203ada71a1a1f08`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2278b7cd7720a82be011f94dfd9d056b889b12068623fc864b02b096cb01ad`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e23ab739c679be25d516008b91998dc0513145f9ecb2fa75e1c762def8699`  
		Last Modified: Mon, 26 Jul 2021 22:58:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c3f69a6d2542114190cf9d0dd3b5d65d06d1e187e7573fde2c374fb1ba911f`  
		Last Modified: Tue, 27 Jul 2021 01:52:38 GMT  
		Size: 6.6 MB (6631696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:53c2ad9b6d5a8f231ddac43584f00467a4b9918a7c614062fc833ffd844e857f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48079442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda81a56396c38d6854bb5ee19197cdce531349b4c380d6335aefdd57e2a1e86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:14:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aadea1266928a0dceab31c4c15ffe7dbcda64c245cfec8104807007655c283`  
		Last Modified: Tue, 31 Aug 2021 02:23:32 GMT  
		Size: 6.8 MB (6838692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:45377dd59b12b41a3c184175c0abed1b1c1c09d4dacab0d58dd20b2522c8664d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53751368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf531ac888458f106c0243748349eeae517521b381458acb72191a28a46fdc1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:03:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:03:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdc5ad45f3591df22f6cfd8a81e806096d73e75cb53dd36f2dc06bedc29cdf8`  
		Last Modified: Tue, 31 Aug 2021 02:11:05 GMT  
		Size: 7.9 MB (7933649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3b4ce36d4c54798487ae7087321faadf62daed06f811a2319250efe6eed04bad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55216587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c715c6822e85a1a0372c9e5ccff135c7dff5e30e5e4cee4eacac586cd03a5239`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:14:07 GMT
ADD file:8fe1a1dacf1dc31e5c6168e69c34f801191864c5fece1d91b13d59807f6056ca in / 
# Mon, 26 Jul 2021 23:14:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 23:14:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 23:14:28 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 04:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:07:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d472a4d60588bf877b1577439fb1db8b17861b63117a33841fe29225c530b95e`  
		Last Modified: Sat, 24 Jul 2021 22:43:36 GMT  
		Size: 47.5 MB (47522379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe44c44a8ee34d79983e97d8261707445db2732ccf6a93cc146c4cdbffca5696`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333f9295db0b7ef046f754b97473c3bd3514e0d9b8465d869119004c929e5261`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c736b6f8064fe10fc657f6af155f5b9827223a418712a0397b8ca50f7f19c83`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783e2b245674c811c355b44a116453c6514c3df2c057ed3df4a19bcbf9a717ac`  
		Last Modified: Tue, 27 Jul 2021 04:29:20 GMT  
		Size: 7.7 MB (7692708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fce0337e93d731b9480e9b84b713df100c81a878790af17ebf225f2e57ee3b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51611223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bd3c2184df3dd73fa66b9b478abedaaac68c45fef540666fe3657eb6c8efb7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd8a6861a80aa4b11ce96ec3537844aec4b713e8074deacba0614cd64afaf6f`  
		Last Modified: Tue, 31 Aug 2021 02:48:46 GMT  
		Size: 7.5 MB (7522004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:16.04-scm`

```console
$ docker pull buildpack-deps@sha256:8c152602c2aeada97c3b7553a69b7ffe2505dea9efdeb971537b168a4f0d772d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:16.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a0b568c44cbd3bf705cb7c0702fe00a82518bcf613d6576ec54692a61003aabf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.2 MB (96195889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:218c7c2a627b92b5b033c2dab9d971c7698135ad134928d70db8f8edaf8b3cc1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 22:03:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:03:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:04:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84cf3b385fa330cddfcec4c9fe29c02ba73e5ce4eeeb01b4b1fcc16ac1c28a9`  
		Last Modified: Mon, 26 Jul 2021 22:15:57 GMT  
		Size: 7.8 MB (7790900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc0223d40ee93a1ec66a4a4c73009a6ec0aecb2dc36910248e21b9066bbe353`  
		Last Modified: Mon, 26 Jul 2021 22:16:16 GMT  
		Size: 41.9 MB (41906076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eeeb88d27c0032638c5aaefe92fc8c6aea572cd80b774d91aac9fde8b8dd77cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85108366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ee7f6558335a1e9cdfb0381bb2c44c095c29c37d1b52a3b4f63dd9271d20f85`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:53:34 GMT
ADD file:4b9fec92db5a0e4059d8b16893d817dca169e585547a48cf5ec6d4afc56e997c in / 
# Mon, 26 Jul 2021 22:53:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 22:53:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:53:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 22:53:41 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 01:31:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba10bfe0b6395fa726456c96036b4fd8ef0513d396442e7419e81550b626b4a0`  
		Last Modified: Sat, 24 Jul 2021 22:43:19 GMT  
		Size: 40.3 MB (40312522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b2be9419691b3c616ec69316c8bef11216dce2cc63b22ba203ada71a1a1f08`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2278b7cd7720a82be011f94dfd9d056b889b12068623fc864b02b096cb01ad`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e23ab739c679be25d516008b91998dc0513145f9ecb2fa75e1c762def8699`  
		Last Modified: Mon, 26 Jul 2021 22:58:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c3f69a6d2542114190cf9d0dd3b5d65d06d1e187e7573fde2c374fb1ba911f`  
		Last Modified: Tue, 27 Jul 2021 01:52:38 GMT  
		Size: 6.6 MB (6631696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d3e4de014d1c265e7133c67440a52321689ea8c718c3367d477494159d3dcf`  
		Last Modified: Tue, 27 Jul 2021 01:53:18 GMT  
		Size: 38.2 MB (38162616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e47a0201f60f95b8cbea4d83e717f345ee7edcf0bc7ae671fae5cda3e24c2e3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87887794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd8ff1996a08e2ab4f9f5ac3d0a19b55f7f2a37f02054ee40f428404a97102f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:14:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aadea1266928a0dceab31c4c15ffe7dbcda64c245cfec8104807007655c283`  
		Last Modified: Tue, 31 Aug 2021 02:23:32 GMT  
		Size: 6.8 MB (6838692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b021524e25acee25ed838c080f43172f4fbdb58e2f2b790bec964d32b0afa48`  
		Last Modified: Tue, 31 Aug 2021 02:23:51 GMT  
		Size: 39.8 MB (39808352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:99c96123c812918f785aa54ef205394d0732a16ebc10b17702c921ffae070da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96642509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5002ff2050d649c8975cea3b4976206d64870dcea48d80e5220d08e654bbb0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:03:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:03:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdc5ad45f3591df22f6cfd8a81e806096d73e75cb53dd36f2dc06bedc29cdf8`  
		Last Modified: Tue, 31 Aug 2021 02:11:05 GMT  
		Size: 7.9 MB (7933649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcec5a27c60c6c19817288510b120bb7290e04bbf035fa5d2aacfe5a35bfc3f7`  
		Last Modified: Tue, 31 Aug 2021 02:11:26 GMT  
		Size: 42.9 MB (42891141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3edc5049548c99f59ab3f938bd64d7ec5a77ec92a55cb38f248158eaa6de49a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100364333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d645f0f7b9454fe7d2ac0efbd2235fa3a9744fa49227ad3118d2f175bb9a5c5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:14:07 GMT
ADD file:8fe1a1dacf1dc31e5c6168e69c34f801191864c5fece1d91b13d59807f6056ca in / 
# Mon, 26 Jul 2021 23:14:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 23:14:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 23:14:28 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 04:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:07:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 04:09:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d472a4d60588bf877b1577439fb1db8b17861b63117a33841fe29225c530b95e`  
		Last Modified: Sat, 24 Jul 2021 22:43:36 GMT  
		Size: 47.5 MB (47522379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe44c44a8ee34d79983e97d8261707445db2732ccf6a93cc146c4cdbffca5696`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333f9295db0b7ef046f754b97473c3bd3514e0d9b8465d869119004c929e5261`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c736b6f8064fe10fc657f6af155f5b9827223a418712a0397b8ca50f7f19c83`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783e2b245674c811c355b44a116453c6514c3df2c057ed3df4a19bcbf9a717ac`  
		Last Modified: Tue, 27 Jul 2021 04:29:20 GMT  
		Size: 7.7 MB (7692708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3a0fe0a58f94d243f9f5cc3c5b58818b595e4658364d01f29e074a94fb2dd`  
		Last Modified: Tue, 27 Jul 2021 04:29:41 GMT  
		Size: 45.1 MB (45147746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a203418fa9ce17ec959479c3f6715d9ecc75466fd0aa528075e0cc9f94ec900a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94299319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c60d1962866a26c61283292dd8fbc87d1d75e3fb6c73d5f60070a001b7d67f40`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:41:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd8a6861a80aa4b11ce96ec3537844aec4b713e8074deacba0614cd64afaf6f`  
		Last Modified: Tue, 31 Aug 2021 02:48:46 GMT  
		Size: 7.5 MB (7522004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102f08394215864198c62652fc16666081e5739d70caea25d4324e60bcab889`  
		Last Modified: Tue, 31 Aug 2021 02:49:00 GMT  
		Size: 42.7 MB (42688096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04`

```console
$ docker pull buildpack-deps@sha256:4cb0b413e27ed0dd741da894f4c4df2c4682bd007bcaf850d61d6971536a1185
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:18.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:db76b519fe4ec10a7e3137a305dd2be63a918c05b746f114db1b987b22e22feb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221268132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a4d488cd94239a5b2ce1397e8d915523b7d1b355c33c3261a4949dd2082a8e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:41:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:44:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b43550a14e1f5842c45eaf5b0043a8aac335974d12b11847980b58fcfd5416`  
		Last Modified: Mon, 26 Jul 2021 22:10:05 GMT  
		Size: 6.6 MB (6644948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e59c30206e4fabc53c96ec7a836fcdc7cdac49cb93fc1b8e376733f4379cfb`  
		Last Modified: Mon, 26 Jul 2021 22:10:04 GMT  
		Size: 3.0 MB (3022291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83c7b2c1eed3a521091d24d714249fb2ee4d8497ba2878141cdd2e4ef3307ef`  
		Last Modified: Mon, 26 Jul 2021 22:10:23 GMT  
		Size: 45.5 MB (45478045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b304099eada42901a68ef5bc8b9f5e19f3bccbf73f7a4062ef0e632913d707`  
		Last Modified: Mon, 26 Jul 2021 22:10:54 GMT  
		Size: 139.4 MB (139413809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d017441d8eeb74735b24ef0361d055928bb725a022644e30658ff36773cb66c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189468139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d890fd1dc3c418299ddfcd5bde9f151f59d68b6cfc60f449cdce804c20134f41`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:14:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:17:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef2837cc6a640557235061b89ed9a389330802f062137cb313376de279870b`  
		Last Modified: Tue, 27 Jul 2021 01:40:03 GMT  
		Size: 5.7 MB (5715357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec9e4b1e75d299207a4006fe43a2e34c3fda90619c762ebc07dc792b034642`  
		Last Modified: Tue, 27 Jul 2021 01:40:01 GMT  
		Size: 2.6 MB (2584467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b636a25e91fe1c88dd15eed3996e0fab60a372c08ebd491408a5eded9d63e`  
		Last Modified: Tue, 27 Jul 2021 01:40:45 GMT  
		Size: 40.7 MB (40671352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee68967ed05e4e5f5edeb14149e1f19b65ea7ff79677978279aa829747e3dfd`  
		Last Modified: Tue, 27 Jul 2021 01:42:10 GMT  
		Size: 118.2 MB (118190111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4848544ea47bd7455408a1ae8882ea0d9f5f8e9d98738aac32d9b73d1419e43e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205819460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e60a0155dcd6083f89bac96420a7a44c0124d5959d08d13db05d7dba2a7b0bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:08:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:10:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a9b8c6709cd3ea323ffea2dcfa72913a9fdc73837573db0ffa663995a44a8`  
		Last Modified: Tue, 31 Aug 2021 02:18:37 GMT  
		Size: 6.1 MB (6087650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ad199f9143cc4082ab5e445c913e284b9f2ec63abce0b6b1243561e2810a77`  
		Last Modified: Tue, 31 Aug 2021 02:18:36 GMT  
		Size: 2.8 MB (2783046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b0514655b3d63ab1f59062bfc8bb2558e7cd9fa05297f66339c11b8952f14`  
		Last Modified: Tue, 31 Aug 2021 02:18:56 GMT  
		Size: 43.3 MB (43267405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6280417b2b490b9a8901d624796b899f9b1f775f39ea1c22af94e7c56a3a34`  
		Last Modified: Tue, 31 Aug 2021 02:19:28 GMT  
		Size: 130.0 MB (129950760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f23a63bd9ab658549e68c52f94e44d1338ae54b1ddca7813c01a6eaa1fcabf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.6 MB (218557666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be5b26d5d1607ab1318e4cce89d6fa77e0516b8783f4db371ccffb3181b5b3b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:57:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:57:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 01:58:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:02:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c7d08d74fca5ace99c2318c3f53f795d5cd713e8df0f41ea3c071a3583372`  
		Last Modified: Tue, 31 Aug 2021 02:09:50 GMT  
		Size: 6.9 MB (6934539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c005ec2b9b98efae8ad7204dd1b1e216eabe229174d28fb5b62c9489ea0`  
		Last Modified: Tue, 31 Aug 2021 02:09:49 GMT  
		Size: 3.3 MB (3252591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40ed14ecd7476315d1f56a8f79f2d48dbad24c195129de044ff6bec685c1613`  
		Last Modified: Tue, 31 Aug 2021 02:10:12 GMT  
		Size: 47.1 MB (47064814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5727719ec2e3d390427c8b8e5fbb7364b3815d04a5147791810cf0fed1474ded`  
		Last Modified: Tue, 31 Aug 2021 02:10:49 GMT  
		Size: 134.1 MB (134143285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9f098d17e856cd5b8fe8ea9f3f39ddf2d77d5da7eb51377f8372fc3e58ab2293
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246217653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6b8c7e9e5a5250a8424c3a99be2d39a0b37cd1abc0fb17b6c0617016e472c3`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:58:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:00:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:06:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475513220a5f30414e690523f753a7a744d3d79b2e0d3cff2d05038e334855a4`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 7.1 MB (7057571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb47fd0ae4274e4d82eec5939329f2aa19c6aaecea4b7e24ccdf34312d95fa8`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 3.7 MB (3719539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0163b280cc161a9528fe1241bdc8a90792874475962941c0f97f2636ec4fc29b`  
		Last Modified: Tue, 27 Jul 2021 04:23:04 GMT  
		Size: 53.7 MB (53715172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61938bdfeed9504952a3e61e49ab0f2e1e17b73d45b28bbffb301cf2744b2fd`  
		Last Modified: Tue, 27 Jul 2021 04:23:43 GMT  
		Size: 151.3 MB (151287413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d2a81bb11386e6802a1e807c1339805562c882b7a1d5619dacb477d99e24e391
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.6 MB (205611586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80fb7da4bcc563d3ea3bbcb40a0c1006159dfd7da2694dff0841a6fbf42ff8f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:34:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:34:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae5daa9a040b93bff6544ad59a003cd958048bef64a9f991a5d3150888fcbed`  
		Last Modified: Tue, 31 Aug 2021 02:45:10 GMT  
		Size: 6.3 MB (6335758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bbf8f7d5625c28aa637939c7029792a4f3b624e300c59cb77575fe7aa84d14`  
		Last Modified: Tue, 31 Aug 2021 02:45:12 GMT  
		Size: 3.0 MB (2974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4165862f9e51452154c0ba3b4ce42f4a8fa2b092d9d4e6c46b46770a5ad6015`  
		Last Modified: Tue, 31 Aug 2021 02:45:26 GMT  
		Size: 45.0 MB (45016355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6def741b217bbfd1346c96876005a3004b76da3416c4839d8c26d070abf3b5`  
		Last Modified: Tue, 31 Aug 2021 02:45:50 GMT  
		Size: 125.9 MB (125918073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-curl`

```console
$ docker pull buildpack-deps@sha256:78a5c19460736d0826ae13f4b766abf2737fd1c73b3356de7cd3da0ffc11ef5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:18.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5d53242a937ee00a3323ef4e7faf6fbc84427a5a66a0581e4cb613b9d83ac099
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36376278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d8990e61ac993b6bb50cd509110e224244289b417364b5bacb145ff1c496568`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b43550a14e1f5842c45eaf5b0043a8aac335974d12b11847980b58fcfd5416`  
		Last Modified: Mon, 26 Jul 2021 22:10:05 GMT  
		Size: 6.6 MB (6644948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e59c30206e4fabc53c96ec7a836fcdc7cdac49cb93fc1b8e376733f4379cfb`  
		Last Modified: Mon, 26 Jul 2021 22:10:04 GMT  
		Size: 3.0 MB (3022291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8cd88ad50e848014c72124a58f84fbe85a33a7ce5932658c6e730d6dbb59fba9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30606676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18bd33d28415880a949129908f93919248f16bc8d8fe5d4251e57dd8bbd9107e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:14:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef2837cc6a640557235061b89ed9a389330802f062137cb313376de279870b`  
		Last Modified: Tue, 27 Jul 2021 01:40:03 GMT  
		Size: 5.7 MB (5715357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec9e4b1e75d299207a4006fe43a2e34c3fda90619c762ebc07dc792b034642`  
		Last Modified: Tue, 27 Jul 2021 01:40:01 GMT  
		Size: 2.6 MB (2584467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5d962e80ddffea4d545bda177e9840d262fb1893cdac6acc8cc3863bf9de75bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32601295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34eb7034c339584e265fb320d1e0d2496baa28988e145f56a72254e7ec081ad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:08:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a9b8c6709cd3ea323ffea2dcfa72913a9fdc73837573db0ffa663995a44a8`  
		Last Modified: Tue, 31 Aug 2021 02:18:37 GMT  
		Size: 6.1 MB (6087650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ad199f9143cc4082ab5e445c913e284b9f2ec63abce0b6b1243561e2810a77`  
		Last Modified: Tue, 31 Aug 2021 02:18:36 GMT  
		Size: 2.8 MB (2783046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:77c62e1928a0a02b1eb69d7cda933975816c77ee2ba1e333f2cb8d916bd3bf92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e6101ebd52b5a1c60f03a674e775c8fa0244a300cbadc8c8f42793a4f5e1b6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:57:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:57:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c7d08d74fca5ace99c2318c3f53f795d5cd713e8df0f41ea3c071a3583372`  
		Last Modified: Tue, 31 Aug 2021 02:09:50 GMT  
		Size: 6.9 MB (6934539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c005ec2b9b98efae8ad7204dd1b1e216eabe229174d28fb5b62c9489ea0`  
		Last Modified: Tue, 31 Aug 2021 02:09:49 GMT  
		Size: 3.3 MB (3252591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2d73cdf00577962a4ff175511e9ae4165e9772824f2aaf3bf2fd988eab5e593e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41215068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232490ed0858a7bf31e6a80f877808b2daea11c077fe994699f1d5db1808aa43`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:58:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475513220a5f30414e690523f753a7a744d3d79b2e0d3cff2d05038e334855a4`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 7.1 MB (7057571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb47fd0ae4274e4d82eec5939329f2aa19c6aaecea4b7e24ccdf34312d95fa8`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 3.7 MB (3719539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b1f689b30d2ae3be28a65adc94df539028bd0f5346b14cbeb8e12d90f6cc549b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34677158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849662eb467d6d767b9ef21110d9f00f5b75c83c278ee84bef70c174b2e1af68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:34:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:34:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae5daa9a040b93bff6544ad59a003cd958048bef64a9f991a5d3150888fcbed`  
		Last Modified: Tue, 31 Aug 2021 02:45:10 GMT  
		Size: 6.3 MB (6335758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bbf8f7d5625c28aa637939c7029792a4f3b624e300c59cb77575fe7aa84d14`  
		Last Modified: Tue, 31 Aug 2021 02:45:12 GMT  
		Size: 3.0 MB (2974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-scm`

```console
$ docker pull buildpack-deps@sha256:a644d5154527dfdb870b98ab060a5383cfe5956bd32b0cda170d8d72e6aa4a7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:18.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d86fa220ec910630351b465c36ec06dff76bee05696b129299e2c652fc02770c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81854323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5862355d4afcb1279e2c4f94df12c33a3edf245e67c761982addc0a96aed5f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:41:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b43550a14e1f5842c45eaf5b0043a8aac335974d12b11847980b58fcfd5416`  
		Last Modified: Mon, 26 Jul 2021 22:10:05 GMT  
		Size: 6.6 MB (6644948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e59c30206e4fabc53c96ec7a836fcdc7cdac49cb93fc1b8e376733f4379cfb`  
		Last Modified: Mon, 26 Jul 2021 22:10:04 GMT  
		Size: 3.0 MB (3022291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83c7b2c1eed3a521091d24d714249fb2ee4d8497ba2878141cdd2e4ef3307ef`  
		Last Modified: Mon, 26 Jul 2021 22:10:23 GMT  
		Size: 45.5 MB (45478045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eb9be4475bf74a12bd2dc33ceda28b14add9042751ede89f1fb2a6d9faa22520
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71278028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76e3a6ee7bd29db1e8e162d6139a74479adf24b065995e04ca0ef15da83f92ba`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:14:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef2837cc6a640557235061b89ed9a389330802f062137cb313376de279870b`  
		Last Modified: Tue, 27 Jul 2021 01:40:03 GMT  
		Size: 5.7 MB (5715357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec9e4b1e75d299207a4006fe43a2e34c3fda90619c762ebc07dc792b034642`  
		Last Modified: Tue, 27 Jul 2021 01:40:01 GMT  
		Size: 2.6 MB (2584467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b636a25e91fe1c88dd15eed3996e0fab60a372c08ebd491408a5eded9d63e`  
		Last Modified: Tue, 27 Jul 2021 01:40:45 GMT  
		Size: 40.7 MB (40671352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:879d52f67da8265f7281b54a011a310ae60d4259ed0dfa396bbadd952a903194
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75868700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea1033b4a10ea257078c5937872da1e61e4c54657bab409800e24b6fa9b8387`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:08:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a9b8c6709cd3ea323ffea2dcfa72913a9fdc73837573db0ffa663995a44a8`  
		Last Modified: Tue, 31 Aug 2021 02:18:37 GMT  
		Size: 6.1 MB (6087650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ad199f9143cc4082ab5e445c913e284b9f2ec63abce0b6b1243561e2810a77`  
		Last Modified: Tue, 31 Aug 2021 02:18:36 GMT  
		Size: 2.8 MB (2783046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b0514655b3d63ab1f59062bfc8bb2558e7cd9fa05297f66339c11b8952f14`  
		Last Modified: Tue, 31 Aug 2021 02:18:56 GMT  
		Size: 43.3 MB (43267405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:80ed2caa4aebc97f6433751e1a0dec62b247c6441fc9dfc5e03d5ecf077e74a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84414381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187f4d53dff720ac9125839acc899f6410afcdf09c08c95113c58bdddc96e0de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:57:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:57:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 01:58:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c7d08d74fca5ace99c2318c3f53f795d5cd713e8df0f41ea3c071a3583372`  
		Last Modified: Tue, 31 Aug 2021 02:09:50 GMT  
		Size: 6.9 MB (6934539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c005ec2b9b98efae8ad7204dd1b1e216eabe229174d28fb5b62c9489ea0`  
		Last Modified: Tue, 31 Aug 2021 02:09:49 GMT  
		Size: 3.3 MB (3252591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40ed14ecd7476315d1f56a8f79f2d48dbad24c195129de044ff6bec685c1613`  
		Last Modified: Tue, 31 Aug 2021 02:10:12 GMT  
		Size: 47.1 MB (47064814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5560e162ea83b6f1a2733d0220352b08ebd8bc5fc91cc006df0bef9e6e17eca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94930240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c560aaa81eaecde3e480a2c97282274c384cda23e6a51e23e9cad9abf5044b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:58:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:00:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475513220a5f30414e690523f753a7a744d3d79b2e0d3cff2d05038e334855a4`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 7.1 MB (7057571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb47fd0ae4274e4d82eec5939329f2aa19c6aaecea4b7e24ccdf34312d95fa8`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 3.7 MB (3719539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0163b280cc161a9528fe1241bdc8a90792874475962941c0f97f2636ec4fc29b`  
		Last Modified: Tue, 27 Jul 2021 04:23:04 GMT  
		Size: 53.7 MB (53715172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6096e767e06165c5154a89c49c3e30bfd9416c6cd6063469118001dbaff6bacd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79693513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709ce7c063bed950b79272f6ad291f8ee966181136bbb2c9bd8ac20f2f4f3617`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:34:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:34:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae5daa9a040b93bff6544ad59a003cd958048bef64a9f991a5d3150888fcbed`  
		Last Modified: Tue, 31 Aug 2021 02:45:10 GMT  
		Size: 6.3 MB (6335758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bbf8f7d5625c28aa637939c7029792a4f3b624e300c59cb77575fe7aa84d14`  
		Last Modified: Tue, 31 Aug 2021 02:45:12 GMT  
		Size: 3.0 MB (2974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4165862f9e51452154c0ba3b4ce42f4a8fa2b092d9d4e6c46b46770a5ad6015`  
		Last Modified: Tue, 31 Aug 2021 02:45:26 GMT  
		Size: 45.0 MB (45016355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:ac5935233587846ba1b87bf3c95e7c055858e4bf5763a246e4abd27292db881f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4b7fe67099dceda7bfcb13dd7aa48258e2b6640b854349481f4d68e27a03c873
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241800863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c060b0cd98ed5dc24171eb227d217cbcc64a9c73a25d7c29cfb9092919ff6fb0`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:45:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:46:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:49:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844d0dd6bf6aa5959f603bad64a331fca5cda171d344450ca89c77e67410ac3`  
		Last Modified: Mon, 26 Jul 2021 22:11:07 GMT  
		Size: 7.8 MB (7769926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e2a2dd7363ebee0e3b7e3d44204409298c305ea2a5f38345f68c7b769033b`  
		Last Modified: Mon, 26 Jul 2021 22:11:06 GMT  
		Size: 3.6 MB (3624037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaacada9b3485ee466ed24e835156869e37b446a2fe7a324d2f9349b81b4d0e`  
		Last Modified: Mon, 26 Jul 2021 22:11:30 GMT  
		Size: 60.7 MB (60718930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b6cb30d1604a69cf710ee8afbc920594fe5ae63e17de53cf47ded9036b7cc2`  
		Last Modified: Mon, 26 Jul 2021 22:12:06 GMT  
		Size: 141.1 MB (141120026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:efc1ca89c89167e69a4f61948d72c6f9c84c5d329b79367248d9b4688c4b65bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207232409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486b525c7c1498a7b327ecca4c676e8ccdb6f6b1b6c6533b3f87511fc1c31e83`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:18:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:19:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:21:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0761e0b1ad0205162c66dfa83bf91ca0344921eca2bdd1d64b0970a5c75f0c`  
		Last Modified: Tue, 27 Jul 2021 01:42:27 GMT  
		Size: 6.8 MB (6767075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c226da21dd821a4b4f19689b2131f6e34d29095f42b4046f2eb48cf954e0076`  
		Last Modified: Tue, 27 Jul 2021 01:42:24 GMT  
		Size: 3.1 MB (3103731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305b0cc7ca4c4e47790a52a092d4cc7774810f9fee0f20387a45833bc8740475`  
		Last Modified: Tue, 27 Jul 2021 01:43:20 GMT  
		Size: 55.5 MB (55454116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ed4d0e81d3335f5c0ef3c7022d19556dbfe4f0b5fd02ab59f0b927a976f597`  
		Last Modified: Tue, 27 Jul 2021 01:44:43 GMT  
		Size: 117.8 MB (117843249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e3839ead7897c13b52908329bd10baca50cb1ef66360966dadfa8b39f983bea4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231941624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d0fe256db32a56a7dc4ec312196c1b98ea8f189e4cf3089cdf49195453cd42`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:10:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:10:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:10:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b8ef0ef6610d6e720afe76a3df03bf2afed7f16cc8b12dab2279c75b1c408`  
		Last Modified: Tue, 31 Aug 2021 02:19:41 GMT  
		Size: 7.6 MB (7636852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a226690073506846a68b797c6c96615eec776aefa661831f4abff3715172704`  
		Last Modified: Tue, 31 Aug 2021 02:19:40 GMT  
		Size: 3.6 MB (3600358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d5c6943027b3d6294ec2bbad85003c7584f70a77a2b64b363ee36bbf30920b`  
		Last Modified: Tue, 31 Aug 2021 02:20:04 GMT  
		Size: 60.8 MB (60766232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93e2b0312aef41acc2f08ed835204fdfe90ab144ae3a37f8a4d4b1769a51f2d`  
		Last Modified: Tue, 31 Aug 2021 02:20:37 GMT  
		Size: 132.8 MB (132765083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:168c59e783ee4016bd0eb2e7f29b4f70fe3a05f40aa246546db37b649e7ceff1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.4 MB (265373323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d9fdf0ea0302149f5068e3e1092e7eba8267bc0a59dad98d5aeb03424a1c4f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:09:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:11:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:20:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f198532bfc08536f5ad0c1f1242b55d34d7aac9ce9dc059a6109c2d7e20b7`  
		Last Modified: Tue, 27 Jul 2021 04:23:58 GMT  
		Size: 8.7 MB (8722787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8f157ddc9f96bd79c6823da12b4c54366d23b79691f3d8f39665ef321ff86e`  
		Last Modified: Tue, 27 Jul 2021 04:23:57 GMT  
		Size: 4.5 MB (4456512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a51a75aca451f998a1dcf27f7a8ece4fb2c2aaf4f7a09896e4664873136d52d`  
		Last Modified: Tue, 27 Jul 2021 04:24:25 GMT  
		Size: 69.4 MB (69386343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cad91e4250099e76cca3f45f2a9042659f5e576e115493fdefb69344c5bfa74`  
		Last Modified: Tue, 27 Jul 2021 04:25:07 GMT  
		Size: 149.5 MB (149517254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:faffd9346d55fa6213130fb0c9a38b4be7304ab9e3c4356c535890f3cf5aefe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222647738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa0dac2fbda7f28429e6b30a06ba7fa724f82ebb53389e9a32ecdff324cc0c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748dba3041b2bd31a240176639b763492a369d59b429da56c854b823820b27b3`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 7.4 MB (7428812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e0c13c39c1426302723ee65c5c58538ee64cf9d25b9629ac690cedd2a7169b`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 3.5 MB (3542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80abe2f24b0566481303d246a8e9996957224b079b7ff282fae87f647409e82c`  
		Last Modified: Tue, 31 Aug 2021 02:46:16 GMT  
		Size: 60.0 MB (60019295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce138a57132ff0b82fe8f962631a86073cbae19bfe4574d55a0d7e6e908d5210`  
		Last Modified: Tue, 31 Aug 2021 02:46:43 GMT  
		Size: 124.5 MB (124530018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:8e7cd12c1a76ba2c6906fc2bf3995dbffb57089f7bfcdead09c0ef7acdf99d90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:20.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8ad7989339bd5853dee1b4694129b35e8f3da4f9bd367566525e02f4bc25430c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39961907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c7b26ba20fb907bc6e40ebdec0384394f1a12802265f68c178e8f2919a646a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:45:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844d0dd6bf6aa5959f603bad64a331fca5cda171d344450ca89c77e67410ac3`  
		Last Modified: Mon, 26 Jul 2021 22:11:07 GMT  
		Size: 7.8 MB (7769926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e2a2dd7363ebee0e3b7e3d44204409298c305ea2a5f38345f68c7b769033b`  
		Last Modified: Mon, 26 Jul 2021 22:11:06 GMT  
		Size: 3.6 MB (3624037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4d6589f264d3d82306ab179d8ff852a670346027a7b62190c0babd4b8d34a958
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33935044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02443af7132a39831ae2d9b9d585c88205154e162e5bbf922e0c3084d7be59d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:18:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0761e0b1ad0205162c66dfa83bf91ca0344921eca2bdd1d64b0970a5c75f0c`  
		Last Modified: Tue, 27 Jul 2021 01:42:27 GMT  
		Size: 6.8 MB (6767075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c226da21dd821a4b4f19689b2131f6e34d29095f42b4046f2eb48cf954e0076`  
		Last Modified: Tue, 27 Jul 2021 01:42:24 GMT  
		Size: 3.1 MB (3103731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:de885f7309d9ab073f94e98a098a4c7c899de49d976b4e1f5a082b722b954785
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38410309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67275e237ee034fba2cbf875eb175b0f631d2b6852b862ac1d3569199a21e87`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:10:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:10:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b8ef0ef6610d6e720afe76a3df03bf2afed7f16cc8b12dab2279c75b1c408`  
		Last Modified: Tue, 31 Aug 2021 02:19:41 GMT  
		Size: 7.6 MB (7636852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a226690073506846a68b797c6c96615eec776aefa661831f4abff3715172704`  
		Last Modified: Tue, 31 Aug 2021 02:19:40 GMT  
		Size: 3.6 MB (3600358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e09bd25d95c7b0f0855b35269f866c1505a2f3b7531a2dc7239ce7bb47f9f068
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46469726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b2ecb47ee2780a093931cf3725b04c02ec822c6aed0eb4a7471d2df82d45663`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:09:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f198532bfc08536f5ad0c1f1242b55d34d7aac9ce9dc059a6109c2d7e20b7`  
		Last Modified: Tue, 27 Jul 2021 04:23:58 GMT  
		Size: 8.7 MB (8722787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8f157ddc9f96bd79c6823da12b4c54366d23b79691f3d8f39665ef321ff86e`  
		Last Modified: Tue, 27 Jul 2021 04:23:57 GMT  
		Size: 4.5 MB (4456512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c5d73e180ba8a80aa23037f5d711ff640e8c4ec80d23ffcbd25059cba22dc138
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34121380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d72b46ed7de7fd72c1870742a2ccea279cef0774ff6b94a241b981033ac58b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:15:32 GMT
ADD file:9492642ba0098006a011dce4d8ce4aa68e0920ff935c864dbcb82561d98740a5 in / 
# Tue, 31 Aug 2021 01:15:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:01:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e7b9bc251112be9d180cbc3a028c58259667feb9a3641efdfd3e35108b2f0c59`  
		Last Modified: Tue, 31 Aug 2021 01:30:41 GMT  
		Size: 24.2 MB (24229065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284ff38f39508e263a7b2fc045b5cea3b705b539db48287b68e6dc16cfa3352`  
		Last Modified: Tue, 31 Aug 2021 02:43:02 GMT  
		Size: 6.7 MB (6747870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4356ee79579dda81c7c5bbf4631f471e2e2f99d800cc4e172d3758e96b2c3136`  
		Last Modified: Tue, 31 Aug 2021 02:42:57 GMT  
		Size: 3.1 MB (3144445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:46a0507904553bff68a72de9063f2851dc892f8a862a5ff7b40bb85a037ad564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38098425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e403f7770ab2a035d85b0bc3bb58bb9414238c54cbdb03c5a8f278ec51daae08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748dba3041b2bd31a240176639b763492a369d59b429da56c854b823820b27b3`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 7.4 MB (7428812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e0c13c39c1426302723ee65c5c58538ee64cf9d25b9629ac690cedd2a7169b`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 3.5 MB (3542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:6315aec3d3d0c866c492bd9485e890c45a220196aa07c375cd62d8a3652ba2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a72c32c022e2d1cebdcbefa2fc0810ed6a0c7be253660f8ad5ea9c521ee826b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100680837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b4080e2629487fd86346ead8e8e820c05cb893949b1970238bd1ea0e4cc8ae`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:45:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:46:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844d0dd6bf6aa5959f603bad64a331fca5cda171d344450ca89c77e67410ac3`  
		Last Modified: Mon, 26 Jul 2021 22:11:07 GMT  
		Size: 7.8 MB (7769926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e2a2dd7363ebee0e3b7e3d44204409298c305ea2a5f38345f68c7b769033b`  
		Last Modified: Mon, 26 Jul 2021 22:11:06 GMT  
		Size: 3.6 MB (3624037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaacada9b3485ee466ed24e835156869e37b446a2fe7a324d2f9349b81b4d0e`  
		Last Modified: Mon, 26 Jul 2021 22:11:30 GMT  
		Size: 60.7 MB (60718930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dee7b6f04c4f83196ef597f3f808046a2dd9027ef167d781f8e63e8863dd65b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89389160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a657cdf3fbed62a72c2fe65d674734ce4b12fbee60d88edce235c8aa2e5a041f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:18:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:19:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0761e0b1ad0205162c66dfa83bf91ca0344921eca2bdd1d64b0970a5c75f0c`  
		Last Modified: Tue, 27 Jul 2021 01:42:27 GMT  
		Size: 6.8 MB (6767075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c226da21dd821a4b4f19689b2131f6e34d29095f42b4046f2eb48cf954e0076`  
		Last Modified: Tue, 27 Jul 2021 01:42:24 GMT  
		Size: 3.1 MB (3103731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305b0cc7ca4c4e47790a52a092d4cc7774810f9fee0f20387a45833bc8740475`  
		Last Modified: Tue, 27 Jul 2021 01:43:20 GMT  
		Size: 55.5 MB (55454116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:19b36271f8dc3c3e32d2efe26aee8d1196a466b9e9daa03445d90e2db344a923
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99176541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88006fc39d950f9ac4bcaac8419a7dcf84b7b72b94bfecdf46a55135c344309f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:10:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:10:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:10:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b8ef0ef6610d6e720afe76a3df03bf2afed7f16cc8b12dab2279c75b1c408`  
		Last Modified: Tue, 31 Aug 2021 02:19:41 GMT  
		Size: 7.6 MB (7636852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a226690073506846a68b797c6c96615eec776aefa661831f4abff3715172704`  
		Last Modified: Tue, 31 Aug 2021 02:19:40 GMT  
		Size: 3.6 MB (3600358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d5c6943027b3d6294ec2bbad85003c7584f70a77a2b64b363ee36bbf30920b`  
		Last Modified: Tue, 31 Aug 2021 02:20:04 GMT  
		Size: 60.8 MB (60766232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3c557088facf8e21f8cb162d5da3b29b0b4d22b7978c6e5330f1abcf4069d200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115856069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81f3ab03184adf9e5ddbbaaf4424797d4ab33a9a2a2acc21b05608758876dbd`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:09:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:11:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f198532bfc08536f5ad0c1f1242b55d34d7aac9ce9dc059a6109c2d7e20b7`  
		Last Modified: Tue, 27 Jul 2021 04:23:58 GMT  
		Size: 8.7 MB (8722787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8f157ddc9f96bd79c6823da12b4c54366d23b79691f3d8f39665ef321ff86e`  
		Last Modified: Tue, 27 Jul 2021 04:23:57 GMT  
		Size: 4.5 MB (4456512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a51a75aca451f998a1dcf27f7a8ece4fb2c2aaf4f7a09896e4664873136d52d`  
		Last Modified: Tue, 27 Jul 2021 04:24:25 GMT  
		Size: 69.4 MB (69386343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:87aef79db204a762d5f40f658ce076db36ab3efc621aa006c6405230ae43653a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98117720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b46e24901559406cd7200c4359b8f96650d7eb96bb6cd9a829fc4b415f1ad1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748dba3041b2bd31a240176639b763492a369d59b429da56c854b823820b27b3`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 7.4 MB (7428812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e0c13c39c1426302723ee65c5c58538ee64cf9d25b9629ac690cedd2a7169b`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 3.5 MB (3542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80abe2f24b0566481303d246a8e9996957224b079b7ff282fae87f647409e82c`  
		Last Modified: Tue, 31 Aug 2021 02:46:16 GMT  
		Size: 60.0 MB (60019295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.04`

```console
$ docker pull buildpack-deps@sha256:0763bfd59ca79835896bb02e6be807329761ba61f5cb9e6f3292f07d7f7242cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:21.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:91e9acc792f026674dd45f446df640319265b7262c1005bde38528222773d568
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248920500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe66bef49b8843238f7319eab8d5305a356c059489e901289f25b7ea66d4e34c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:55:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:58:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9939f009cb8ebf9ee9b4f6b6f99c0a7ca437c96b046a6345f065cbfcc3dde`  
		Last Modified: Mon, 26 Jul 2021 22:13:53 GMT  
		Size: 43.5 MB (43540366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111c706438d96ec9682736266bade1a4ac6bc3b0a5c98d469c32eddc94a5acbc`  
		Last Modified: Mon, 26 Jul 2021 22:14:30 GMT  
		Size: 164.4 MB (164449942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:786b965a9d6a8aa7384f2db07ae95fa6fb61ce55efe86186d39ffca8a2ed1056
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208923584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f552a257abc3da22a3250ecfc6d93dec61196503231879dba0c59f3b55dea58b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:32 GMT
ADD file:76353e48968f6c84802b150e577cc7fb1bc50985e78e1b499ecd8debfe50d8e5 in / 
# Mon, 26 Jul 2021 22:52:33 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:681a32f1cee4135c0497939e80766271e03a995a197d8293224e8f6bd470bfdd`  
		Last Modified: Mon, 26 Jul 2021 22:57:17 GMT  
		Size: 26.9 MB (26857313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d081ccdbe67f74ab6dab322dc6e8e84a9b56cb1909518f7d199a8fc8936d`  
		Last Modified: Tue, 27 Jul 2021 01:47:35 GMT  
		Size: 4.9 MB (4858897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb191db7ef79ad38fdcde76e18b9267b765696ecf8c500929ef80b649f800`  
		Last Modified: Tue, 27 Jul 2021 01:47:34 GMT  
		Size: 3.1 MB (3138386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b923df82160d2d4eea0012b206b82fae9ca16efd703aacc1069a7bb396b558`  
		Last Modified: Tue, 27 Jul 2021 01:48:15 GMT  
		Size: 40.0 MB (39956131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81972472b3986b3a6bbc0402e59a3d8f113ad7e7069d8918c442e57619255ef6`  
		Last Modified: Tue, 27 Jul 2021 01:49:48 GMT  
		Size: 134.1 MB (134112857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7e5f6e0a00dda48a76aa17bdd9632efad49c2d5e958de1da097c4ba901fcab89
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239569400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd905178021460f6c7f78fa90eceb02ac097094f0e7b4fa0619328671c28a7f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:53 GMT
ADD file:93dcfc1791d96861438a84bfd38f5c0520353febfcc59bde5510c9e85eab2cf8 in / 
# Tue, 31 Aug 2021 01:40:54 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:11:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4fbd1b15195364f20d4b603e346a2b5c64ae93e9de90f5c1bd82a61e92851632`  
		Last Modified: Tue, 31 Aug 2021 01:42:57 GMT  
		Size: 30.2 MB (30162874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54fbc3de08027791a7280c6d2d7f821165cc126fd0e08c6cba66c1d6fc122`  
		Last Modified: Tue, 31 Aug 2021 02:20:51 GMT  
		Size: 5.4 MB (5401544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7180cc8ab79571bbc48658748543060674d12cbbdf7683a598d89f6086677`  
		Last Modified: Tue, 31 Aug 2021 02:20:50 GMT  
		Size: 3.6 MB (3638240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826a66d619e21f0b3656bcd20cb8925d105fc0e444b4a72eb69d81408ecf67ed`  
		Last Modified: Tue, 31 Aug 2021 02:21:10 GMT  
		Size: 43.5 MB (43525534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0590f0535def702f02a4c077e4c3fe732c276f278986df7dc19c8a7c463603`  
		Last Modified: Tue, 31 Aug 2021 02:21:45 GMT  
		Size: 156.8 MB (156841208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e912d8844618c3e84df88afdb02d2fcc5ed1713afcb23c067a3e0d469ab40951
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.2 MB (268194289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428d43eec21252ab8aa929510a3955ba8fa3a1e59f0f8d49cbf487fc2abf9cd`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:18 GMT
ADD file:42c46f2fd1479c7d309139946c738ffe5c5379a9561b96a8d7511bdb0090481e in / 
# Mon, 26 Jul 2021 23:13:21 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:38:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:47:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:50f10986101895abb3160c75977e8e8eb7b79e82f78fa9dd1883692b644e4675`  
		Last Modified: Mon, 26 Jul 2021 23:16:36 GMT  
		Size: 37.4 MB (37352998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72f19678043711c11465b507df75ce318af4bd2b392f685ca3841dbba055aa`  
		Last Modified: Tue, 27 Jul 2021 04:26:44 GMT  
		Size: 6.1 MB (6133314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a982650c2954b338afda90c5ba86d7603861d62a22b2e3800362985c59823f`  
		Last Modified: Tue, 27 Jul 2021 04:26:43 GMT  
		Size: 4.5 MB (4523551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4da86ef0de66c418b38e81b81a9690c0e7b660053a2b63e8a7b090c8ffdd23`  
		Last Modified: Tue, 27 Jul 2021 04:27:06 GMT  
		Size: 49.5 MB (49482660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df05ea742cc84cf005f5b1fbce3aa2099c7974bbd0654675d0c0ff8c7dbab40f`  
		Last Modified: Tue, 27 Jul 2021 04:27:48 GMT  
		Size: 170.7 MB (170701766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ac52edf6a4ea4ab1f8ee0096caf69ad869cac3a58b760bee7eb927b04a48d6a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.9 MB (257914485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8b02dfe5db83585a676ecaa8de2d87d02ca0e88a0eb635baf0a58f8a5a54119`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:17:33 GMT
ADD file:c9125fcbdad41a027e81c7fc0616e4698eefb4bf591e9c215748c44001492a71 in / 
# Tue, 31 Aug 2021 01:17:35 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:03:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de98d6361415ec89b2135480af53817e96bf60ae2c78c53dad37c447f0f7b040`  
		Last Modified: Tue, 31 Aug 2021 01:33:15 GMT  
		Size: 27.1 MB (27143365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225134e3c31562a8c1d476ee61f8672ab2a39bc9f6dd1aa9d2334027bacf22c0`  
		Last Modified: Tue, 31 Aug 2021 02:44:14 GMT  
		Size: 4.9 MB (4945167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ca77fa5925540bdc2a4cf61c8acfdf7fc0d169793ae57fd6e0b7a6465022d`  
		Last Modified: Tue, 31 Aug 2021 02:44:11 GMT  
		Size: 3.2 MB (3177763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98a854c5e99476d386d6334136c9b5839b261270f40552a56a5557336599fcd`  
		Last Modified: Tue, 31 Aug 2021 02:46:12 GMT  
		Size: 40.3 MB (40329103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c567f920ef8255eb4f50d24bf8b4329ffc4253128705dc547c32723ea2c15bec`  
		Last Modified: Tue, 31 Aug 2021 02:51:50 GMT  
		Size: 182.3 MB (182319087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:16cbc9689a2459ec88062d9374e59c88dd2d38965300fa2f3d8afa87b6141c1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241418909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b8f027f78486d0ae43707e9e3128407eb00ebf6a230cfd375abfca1a96e8690`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:38 GMT
ADD file:ba5c2c420b69d0c125e25122344e156fa468282be3e91af99f6941eb676f308d in / 
# Tue, 31 Aug 2021 01:42:41 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e7ad6541ebda77ecfec574e1268bb944ba28f14ca69dab7bad1d63702975176`  
		Last Modified: Tue, 31 Aug 2021 01:44:29 GMT  
		Size: 32.5 MB (32491578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66e7ecd9588795e7cf09605e17fa940cd2b5566b310df2b484b60ba5faee036`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 5.8 MB (5802191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36acc9b914fe8f7ad986a1869bcd54799c01524d5a43634c1cff6407f77d9a14`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 4.2 MB (4185117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceeae36ed176d953e43f3ac748df4f3d272212947102e33987f59a8cecb55002`  
		Last Modified: Tue, 31 Aug 2021 02:47:06 GMT  
		Size: 47.4 MB (47400028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beaf975b1e5ae8c6fbc46716b09e0482ee34d077a5e324a7cb39c58d7d7e096`  
		Last Modified: Tue, 31 Aug 2021 02:47:32 GMT  
		Size: 151.5 MB (151539995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.04-curl`

```console
$ docker pull buildpack-deps@sha256:3a72acc16fe1512414241dee6ddcb2a633d22a9b56c8f3047b71fa90a6a8b98f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:21.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:87e3c232b29e67193cb8e3a360f59ef5bd082bac752150ac2e8f3dfd8dab5d67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40930192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0edd837b914a819d7989e4d055fee59b4f440b93324d3251e9e278f6af6ae9a1`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a130bec7346768f9e8fb6ac3803a47561327abb05a55c28428690c9fb241360d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34854596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:951f0804064fd4937066c5d9915e51e7a80326b9dffb2c8211540cc7ed1b4b71`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:32 GMT
ADD file:76353e48968f6c84802b150e577cc7fb1bc50985e78e1b499ecd8debfe50d8e5 in / 
# Mon, 26 Jul 2021 22:52:33 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:681a32f1cee4135c0497939e80766271e03a995a197d8293224e8f6bd470bfdd`  
		Last Modified: Mon, 26 Jul 2021 22:57:17 GMT  
		Size: 26.9 MB (26857313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d081ccdbe67f74ab6dab322dc6e8e84a9b56cb1909518f7d199a8fc8936d`  
		Last Modified: Tue, 27 Jul 2021 01:47:35 GMT  
		Size: 4.9 MB (4858897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb191db7ef79ad38fdcde76e18b9267b765696ecf8c500929ef80b649f800`  
		Last Modified: Tue, 27 Jul 2021 01:47:34 GMT  
		Size: 3.1 MB (3138386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1be6a6a353e2c9182de84c02a356036c8dde9815bb83505c0c329d064a55a6db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39202658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a37e4fd97a4962d1b26f3ab8d4d4b3037cf0f744a21cd18626183658d36514b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:53 GMT
ADD file:93dcfc1791d96861438a84bfd38f5c0520353febfcc59bde5510c9e85eab2cf8 in / 
# Tue, 31 Aug 2021 01:40:54 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:11:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4fbd1b15195364f20d4b603e346a2b5c64ae93e9de90f5c1bd82a61e92851632`  
		Last Modified: Tue, 31 Aug 2021 01:42:57 GMT  
		Size: 30.2 MB (30162874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54fbc3de08027791a7280c6d2d7f821165cc126fd0e08c6cba66c1d6fc122`  
		Last Modified: Tue, 31 Aug 2021 02:20:51 GMT  
		Size: 5.4 MB (5401544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7180cc8ab79571bbc48658748543060674d12cbbdf7683a598d89f6086677`  
		Last Modified: Tue, 31 Aug 2021 02:20:50 GMT  
		Size: 3.6 MB (3638240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0d986d60b7c68efa0428ba53ce2fca6f2363653c7ff5b21a2f8137d5f6d82650
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48009863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceb6d2da938e4f3e8ce68f5a01892235875704d7e88689eee9deac09bac85051`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:18 GMT
ADD file:42c46f2fd1479c7d309139946c738ffe5c5379a9561b96a8d7511bdb0090481e in / 
# Mon, 26 Jul 2021 23:13:21 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:50f10986101895abb3160c75977e8e8eb7b79e82f78fa9dd1883692b644e4675`  
		Last Modified: Mon, 26 Jul 2021 23:16:36 GMT  
		Size: 37.4 MB (37352998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72f19678043711c11465b507df75ce318af4bd2b392f685ca3841dbba055aa`  
		Last Modified: Tue, 27 Jul 2021 04:26:44 GMT  
		Size: 6.1 MB (6133314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a982650c2954b338afda90c5ba86d7603861d62a22b2e3800362985c59823f`  
		Last Modified: Tue, 27 Jul 2021 04:26:43 GMT  
		Size: 4.5 MB (4523551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:64c1efaa41585b95c9ae764b82ee6479920b3d19ee810a1fd0dc22c8a73f687c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35266295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1affb32245af279b11f5c62e61f3660f196c615fed09a9a21d3a0e5c8fa2a41b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:17:33 GMT
ADD file:c9125fcbdad41a027e81c7fc0616e4698eefb4bf591e9c215748c44001492a71 in / 
# Tue, 31 Aug 2021 01:17:35 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:03:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:de98d6361415ec89b2135480af53817e96bf60ae2c78c53dad37c447f0f7b040`  
		Last Modified: Tue, 31 Aug 2021 01:33:15 GMT  
		Size: 27.1 MB (27143365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225134e3c31562a8c1d476ee61f8672ab2a39bc9f6dd1aa9d2334027bacf22c0`  
		Last Modified: Tue, 31 Aug 2021 02:44:14 GMT  
		Size: 4.9 MB (4945167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ca77fa5925540bdc2a4cf61c8acfdf7fc0d169793ae57fd6e0b7a6465022d`  
		Last Modified: Tue, 31 Aug 2021 02:44:11 GMT  
		Size: 3.2 MB (3177763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a3a6241c11d52798f69cd608769182ec132e3c3557678a5b7d53de38c8cd7495
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42478886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c486f889ee86ee0e24365015f7d20301cd102b59e96a42c55b86db311ca2572`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:38 GMT
ADD file:ba5c2c420b69d0c125e25122344e156fa468282be3e91af99f6941eb676f308d in / 
# Tue, 31 Aug 2021 01:42:41 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2e7ad6541ebda77ecfec574e1268bb944ba28f14ca69dab7bad1d63702975176`  
		Last Modified: Tue, 31 Aug 2021 01:44:29 GMT  
		Size: 32.5 MB (32491578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66e7ecd9588795e7cf09605e17fa940cd2b5566b310df2b484b60ba5faee036`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 5.8 MB (5802191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36acc9b914fe8f7ad986a1869bcd54799c01524d5a43634c1cff6407f77d9a14`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 4.2 MB (4185117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.04-scm`

```console
$ docker pull buildpack-deps@sha256:3fb49365cba4d74083cb480597e51047a6f356345efc6538476b62d078215bfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:21.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:03c440ab93f47f6f25a8234febc88184480f28020791200b902ad758cc4fc7fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84470558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:823cef2ec1834c9343ac135b8763c224793328b28dd2afae1dad1a2da3016cac`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:55:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9939f009cb8ebf9ee9b4f6b6f99c0a7ca437c96b046a6345f065cbfcc3dde`  
		Last Modified: Mon, 26 Jul 2021 22:13:53 GMT  
		Size: 43.5 MB (43540366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6fcc5afd47847c2e97114df73dfbdb7cb98b3dba59c9d5e0460f5353e0ab2cd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74810727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12dc9111323484a0279e67f569d4cb21203c02f93aa3dcaa657dcc5ac889e26f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:32 GMT
ADD file:76353e48968f6c84802b150e577cc7fb1bc50985e78e1b499ecd8debfe50d8e5 in / 
# Mon, 26 Jul 2021 22:52:33 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:681a32f1cee4135c0497939e80766271e03a995a197d8293224e8f6bd470bfdd`  
		Last Modified: Mon, 26 Jul 2021 22:57:17 GMT  
		Size: 26.9 MB (26857313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d081ccdbe67f74ab6dab322dc6e8e84a9b56cb1909518f7d199a8fc8936d`  
		Last Modified: Tue, 27 Jul 2021 01:47:35 GMT  
		Size: 4.9 MB (4858897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb191db7ef79ad38fdcde76e18b9267b765696ecf8c500929ef80b649f800`  
		Last Modified: Tue, 27 Jul 2021 01:47:34 GMT  
		Size: 3.1 MB (3138386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b923df82160d2d4eea0012b206b82fae9ca16efd703aacc1069a7bb396b558`  
		Last Modified: Tue, 27 Jul 2021 01:48:15 GMT  
		Size: 40.0 MB (39956131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a0e40d34528ab940355ef0e5c6e5a4331f9bb512e5e3104310ea9db74dc73d59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82728192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca32f751faa503b8fea9beef96876f4dbec6142b5dce0a0f3112fd89eb7c213c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:53 GMT
ADD file:93dcfc1791d96861438a84bfd38f5c0520353febfcc59bde5510c9e85eab2cf8 in / 
# Tue, 31 Aug 2021 01:40:54 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:11:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4fbd1b15195364f20d4b603e346a2b5c64ae93e9de90f5c1bd82a61e92851632`  
		Last Modified: Tue, 31 Aug 2021 01:42:57 GMT  
		Size: 30.2 MB (30162874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54fbc3de08027791a7280c6d2d7f821165cc126fd0e08c6cba66c1d6fc122`  
		Last Modified: Tue, 31 Aug 2021 02:20:51 GMT  
		Size: 5.4 MB (5401544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7180cc8ab79571bbc48658748543060674d12cbbdf7683a598d89f6086677`  
		Last Modified: Tue, 31 Aug 2021 02:20:50 GMT  
		Size: 3.6 MB (3638240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826a66d619e21f0b3656bcd20cb8925d105fc0e444b4a72eb69d81408ecf67ed`  
		Last Modified: Tue, 31 Aug 2021 02:21:10 GMT  
		Size: 43.5 MB (43525534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f27c67b36f263760a8087131c54011ace3bd5d7db22c6529665d6abadf899e03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97492523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8b571049a41e25671a9c46d043cc1d74fe7567e153df521e45039f369392ac`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:18 GMT
ADD file:42c46f2fd1479c7d309139946c738ffe5c5379a9561b96a8d7511bdb0090481e in / 
# Mon, 26 Jul 2021 23:13:21 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:38:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:50f10986101895abb3160c75977e8e8eb7b79e82f78fa9dd1883692b644e4675`  
		Last Modified: Mon, 26 Jul 2021 23:16:36 GMT  
		Size: 37.4 MB (37352998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72f19678043711c11465b507df75ce318af4bd2b392f685ca3841dbba055aa`  
		Last Modified: Tue, 27 Jul 2021 04:26:44 GMT  
		Size: 6.1 MB (6133314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a982650c2954b338afda90c5ba86d7603861d62a22b2e3800362985c59823f`  
		Last Modified: Tue, 27 Jul 2021 04:26:43 GMT  
		Size: 4.5 MB (4523551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4da86ef0de66c418b38e81b81a9690c0e7b660053a2b63e8a7b090c8ffdd23`  
		Last Modified: Tue, 27 Jul 2021 04:27:06 GMT  
		Size: 49.5 MB (49482660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:92d46888b25701d05c84398baa31995dd2f2f9cece8d00a6d36ae0b98b41ed12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75595398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a3029ed135684d6a7d55a4aa6663061bf0bddaaac730e68a265ebb4392da89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:17:33 GMT
ADD file:c9125fcbdad41a027e81c7fc0616e4698eefb4bf591e9c215748c44001492a71 in / 
# Tue, 31 Aug 2021 01:17:35 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:03:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de98d6361415ec89b2135480af53817e96bf60ae2c78c53dad37c447f0f7b040`  
		Last Modified: Tue, 31 Aug 2021 01:33:15 GMT  
		Size: 27.1 MB (27143365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225134e3c31562a8c1d476ee61f8672ab2a39bc9f6dd1aa9d2334027bacf22c0`  
		Last Modified: Tue, 31 Aug 2021 02:44:14 GMT  
		Size: 4.9 MB (4945167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ca77fa5925540bdc2a4cf61c8acfdf7fc0d169793ae57fd6e0b7a6465022d`  
		Last Modified: Tue, 31 Aug 2021 02:44:11 GMT  
		Size: 3.2 MB (3177763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98a854c5e99476d386d6334136c9b5839b261270f40552a56a5557336599fcd`  
		Last Modified: Tue, 31 Aug 2021 02:46:12 GMT  
		Size: 40.3 MB (40329103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:946ba36daa4e4c0d9d38cda5253c2dfd87343e5523921f9a8f70978f0698ae7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89878914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e2cfd6247f86f57d874973213ecadf290768b88929aad3faf6c98c3ffda491`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:38 GMT
ADD file:ba5c2c420b69d0c125e25122344e156fa468282be3e91af99f6941eb676f308d in / 
# Tue, 31 Aug 2021 01:42:41 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e7ad6541ebda77ecfec574e1268bb944ba28f14ca69dab7bad1d63702975176`  
		Last Modified: Tue, 31 Aug 2021 01:44:29 GMT  
		Size: 32.5 MB (32491578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66e7ecd9588795e7cf09605e17fa940cd2b5566b310df2b484b60ba5faee036`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 5.8 MB (5802191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36acc9b914fe8f7ad986a1869bcd54799c01524d5a43634c1cff6407f77d9a14`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 4.2 MB (4185117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceeae36ed176d953e43f3ac748df4f3d272212947102e33987f59a8cecb55002`  
		Last Modified: Tue, 31 Aug 2021 02:47:06 GMT  
		Size: 47.4 MB (47400028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.10`

```console
$ docker pull buildpack-deps@sha256:c7231b3b249de0235336e685852ad6cb611a1c60e593056efb47bb34e3090328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:21.10` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f1fbd344d391628950235e7ebbc2e73a07ec866504c8a8cf07eb080c0424ea23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.0 MB (241014503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29c1f84f1b4abbb17e66779835d3e04817d65d23dac76136a79263e383606b5e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:01 GMT
ADD file:aad4137373f37cc2272f1632b0fa50a91b4c0c878ca72ae8de8fee51ffa2f392 in / 
# Mon, 26 Jul 2021 21:22:02 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:59:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:02:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c8d2949e37d3f87c8d42e502aebe8d287cc56bd1f5846a5265a2124c60cb49c`  
		Last Modified: Mon, 26 Jul 2021 21:24:04 GMT  
		Size: 31.5 MB (31519889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad149f781f55b2a85f0e013b5220678d294bfdc9a113255a07b8fd871224219`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.7 MB (3692251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11936e1d3aa1eb439ea9dac0215a97aa74b71b1eabeed3965b276ff2c836d5e`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.6 MB (3552048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8ee9b3c3bd20f022701661feb52a5704b01f803876f6ebed7ce76763e8308e`  
		Last Modified: Mon, 26 Jul 2021 22:15:03 GMT  
		Size: 37.9 MB (37878472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0aa8dd8688cfc9a43656760d3e978006c45b87ca791b9167139138d70a1b24`  
		Last Modified: Mon, 26 Jul 2021 22:15:39 GMT  
		Size: 164.4 MB (164371843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5928a111b753c3ea702c899aa1dadf079dbfebd238622fe69088e94070f72bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.2 MB (208201657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99da5a03dde9bc7c4517e415d7d5005cf746dd8520e1cc643bfa0671a3071b31`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:54 GMT
ADD file:7c7c93de372cabbc1cbc45bb3618b626ecd538c81cdb8a09c63b397ac79615ca in / 
# Mon, 26 Jul 2021 22:52:55 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:29:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:31:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa3fdc2705d50f3ad184e38a8ae9a54c70a75ef26a8f2036c5cc36454c57b49a`  
		Last Modified: Mon, 26 Jul 2021 22:57:52 GMT  
		Size: 26.9 MB (26876142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05927c7769ed8e7aa2c01453e69c9f65172154a601b0218204df2a1c260a6`  
		Last Modified: Tue, 27 Jul 2021 01:50:05 GMT  
		Size: 3.4 MB (3438752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c89b675bf7d9d2c4ea66630864775dc5879d8e56b1c77d25f08550fd9f882b`  
		Last Modified: Tue, 27 Jul 2021 01:50:04 GMT  
		Size: 3.7 MB (3742290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebac5e3a405d40889f25f311860e0142aaa8172e0dc5fe0de50562f4f0c3a13`  
		Last Modified: Tue, 27 Jul 2021 01:50:46 GMT  
		Size: 40.1 MB (40055381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0958d8b812ecd19d60e605cda443527872d489da05c24b268b265ad90455c7a`  
		Last Modified: Tue, 27 Jul 2021 01:52:18 GMT  
		Size: 134.1 MB (134089092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9fba45e42da203add658a83d947b8063b6e3e8821e9d87f2735a0e7c94861c62
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.5 MB (399490006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d91834fc28eab00910a8bc6ab02bf69640dc79fd4c237189ec0b270e505a452`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:02 GMT
ADD file:ed3a8c55fbedc627dd5d33aecf52df10becbd9bd492f7c3f4f0a710b15629618 in / 
# Tue, 31 Aug 2021 01:41:03 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:13:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:14:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:835dcfefc46e2b5551a40002ffed802b6b70970071e61e3f9dce0dd0404c2a12`  
		Last Modified: Tue, 31 Aug 2021 01:43:19 GMT  
		Size: 29.0 MB (29033527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76d237fe2a405ec5c0175da7117764a3725e495a5280fa68824281d0209f48`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.7 MB (3677477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972cd7eb9f3f8f76c354e0777c1e299b4979c519af36ee25c5a4b5176d14c93b`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.5 MB (3533509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f0c095fc735f206fea57d94ba168122a4d321e4718f54f2db7b3f7c503ed6`  
		Last Modified: Tue, 31 Aug 2021 02:22:17 GMT  
		Size: 38.1 MB (38076803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feef883879fbaff65f9ee52b7386798fbbe6f94a0b6031c782a0345fbb93d11`  
		Last Modified: Tue, 31 Aug 2021 02:23:17 GMT  
		Size: 325.2 MB (325168690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:026f6496bf6d4bafc2b039e06e34dde5dde8d61220141f114a7305ce9e8e2ca3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258293115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c20ecec8e3efdf1ba1eb0ccb7ca993541ac9081c97fa86d026a768ca4c722e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:33 GMT
ADD file:5419572ba3a583506859cb346c0715939486d87fcc143e308557a18a73bb92b2 in / 
# Mon, 26 Jul 2021 23:13:37 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:49:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:50:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:52:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:05:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:415d912bb08e4b766d9582ddc3d0e3c55a978420909d0ce62488cfc6ddcd065d`  
		Last Modified: Mon, 26 Jul 2021 23:17:00 GMT  
		Size: 37.2 MB (37160030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03ededf19de330d97ae5f2cd78f381456f81c19eb46ff80cebace0dbe476eac`  
		Last Modified: Tue, 27 Jul 2021 04:28:02 GMT  
		Size: 4.1 MB (4095072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ec3f753c3934e1f67de00b1cde7c52b2558b372872daab551be31f8ee74787`  
		Last Modified: Tue, 27 Jul 2021 04:28:01 GMT  
		Size: 4.2 MB (4241926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946929704f815af80a61ae55d86531279d22d2292a2f74bf22ed5819c842bb88`  
		Last Modified: Tue, 27 Jul 2021 04:28:22 GMT  
		Size: 42.3 MB (42289669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0c649aac611e54d363fe1b342ef3f246007e65e9ed1524344fb03a95842bd7`  
		Last Modified: Tue, 27 Jul 2021 04:29:05 GMT  
		Size: 170.5 MB (170506418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:e8938656e5921a5d321c930f895539216d4881311214c803e2643503210f917c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.4 MB (267418888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cccfa4b5ab59d8bd311ab4a7f824737ab812260d9622df726a8bf3f0eecd481`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:19:36 GMT
ADD file:84d3daa77b3c4590ccb1b2c1bdfa7b2ea2629a8e289c7e0df33678a72ef40f4c in / 
# Tue, 31 Aug 2021 01:19:38 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:16:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:20:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:26:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2027d80189558886be09b6f8194607cd27258802c79f3c3f228e92404c40c304`  
		Last Modified: Tue, 31 Aug 2021 01:35:47 GMT  
		Size: 27.2 MB (27192169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccb43db8246e726e33f90f4887b26c5c6e5c0eb9b7c4fd223c18539a9963369`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 3.5 MB (3483280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a66489e611edd2a918d67c7aa380888b297b1b1170487f8cf4d412010e9da74`  
		Last Modified: Tue, 31 Aug 2021 02:53:00 GMT  
		Size: 3.8 MB (3803155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2a8d532c190bc5429a7b1a5b15e55c1c120cd8fd520ce5adcdeacadde8c6cb`  
		Last Modified: Tue, 31 Aug 2021 02:55:01 GMT  
		Size: 40.7 MB (40741042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fcfc294837d6a343623ab80428c480526c29b2bb2550c72deb28922f97489f`  
		Last Modified: Tue, 31 Aug 2021 03:00:51 GMT  
		Size: 192.2 MB (192199242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2813c9e36e8aa79b52e8baaa49202e6b8118da28adf2c05c0474ee676685cc4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.4 MB (370398338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c30fa68204d8cf8bba78b5f70b8a1b3fe9b5adefe038d919dc178471b101048`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:54 GMT
ADD file:4748ab039bb7c33cbda2bba944346ecf2e0e6238971d842acc53ec7e8c77df92 in / 
# Tue, 31 Aug 2021 01:42:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:39:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:39:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2abd65908848180c8f2b1a3f2a6493d9c7c22253fc30bc557fce0bbf12327e7`  
		Last Modified: Tue, 31 Aug 2021 01:44:45 GMT  
		Size: 31.3 MB (31308069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f61cb11476011700fc2feeb76881a7eeceb9638e97fa4c33603d64dab544155`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3950090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7802bd74770db74806622bc0f14aa9cc4666241c5b47c5aee05c1b85aa17ebe5`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3962603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e8b1ada6b39a4ab9001051926a2b823d061ce3d31ae907a24efa8fa9961ec`  
		Last Modified: Tue, 31 Aug 2021 02:47:54 GMT  
		Size: 38.9 MB (38858118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62018211b9b26fc8460e4b465948a6eecc369f5b26a1014a1453ed9a8ac2ed7c`  
		Last Modified: Tue, 31 Aug 2021 02:48:36 GMT  
		Size: 292.3 MB (292319458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.10-curl`

```console
$ docker pull buildpack-deps@sha256:e7b8414d525774e5b4628a305abdae6ff90e2fc7b84fedaf62402035b5456292
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:21.10-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c8382f9699ecc7686190ed3ba75041ec06511c7ae5be650adba6abe1a2d1e4a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38764188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f9bb8a11c0d1b625f74b36eed098e3671e1079814f7535e6fa39d4773adb19`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:01 GMT
ADD file:aad4137373f37cc2272f1632b0fa50a91b4c0c878ca72ae8de8fee51ffa2f392 in / 
# Mon, 26 Jul 2021 21:22:02 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:59:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6c8d2949e37d3f87c8d42e502aebe8d287cc56bd1f5846a5265a2124c60cb49c`  
		Last Modified: Mon, 26 Jul 2021 21:24:04 GMT  
		Size: 31.5 MB (31519889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad149f781f55b2a85f0e013b5220678d294bfdc9a113255a07b8fd871224219`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.7 MB (3692251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11936e1d3aa1eb439ea9dac0215a97aa74b71b1eabeed3965b276ff2c836d5e`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.6 MB (3552048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:14cb8487c3b5aea4627a0dd934cbc37283b95eb342ad6ccc08e89753ade64ae9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34057184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f2e381f6175d4348fc21d1d747335f18ba51395951d01822be790604501efd9`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:54 GMT
ADD file:7c7c93de372cabbc1cbc45bb3618b626ecd538c81cdb8a09c63b397ac79615ca in / 
# Mon, 26 Jul 2021 22:52:55 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fa3fdc2705d50f3ad184e38a8ae9a54c70a75ef26a8f2036c5cc36454c57b49a`  
		Last Modified: Mon, 26 Jul 2021 22:57:52 GMT  
		Size: 26.9 MB (26876142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05927c7769ed8e7aa2c01453e69c9f65172154a601b0218204df2a1c260a6`  
		Last Modified: Tue, 27 Jul 2021 01:50:05 GMT  
		Size: 3.4 MB (3438752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c89b675bf7d9d2c4ea66630864775dc5879d8e56b1c77d25f08550fd9f882b`  
		Last Modified: Tue, 27 Jul 2021 01:50:04 GMT  
		Size: 3.7 MB (3742290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a443fd6e3736e490f466797038af04904d36fc0129968f8a26a2d0c0f5411654
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36244513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651cadc9706f04ce4ca19d0656ea6e725e8b0099e4f8ac8a95e0c9db590029d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:02 GMT
ADD file:ed3a8c55fbedc627dd5d33aecf52df10becbd9bd492f7c3f4f0a710b15629618 in / 
# Tue, 31 Aug 2021 01:41:03 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:13:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:835dcfefc46e2b5551a40002ffed802b6b70970071e61e3f9dce0dd0404c2a12`  
		Last Modified: Tue, 31 Aug 2021 01:43:19 GMT  
		Size: 29.0 MB (29033527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76d237fe2a405ec5c0175da7117764a3725e495a5280fa68824281d0209f48`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.7 MB (3677477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972cd7eb9f3f8f76c354e0777c1e299b4979c519af36ee25c5a4b5176d14c93b`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.5 MB (3533509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fb1ae578b0181287cdee49a1ddf90688b5634cddd1742a265064aeb8ca520596
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45497028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b814659ec88c950bcc0e38be82a3b5cbca6e6929da1fe08971ca5efa510f66`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:33 GMT
ADD file:5419572ba3a583506859cb346c0715939486d87fcc143e308557a18a73bb92b2 in / 
# Mon, 26 Jul 2021 23:13:37 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:49:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:50:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:415d912bb08e4b766d9582ddc3d0e3c55a978420909d0ce62488cfc6ddcd065d`  
		Last Modified: Mon, 26 Jul 2021 23:17:00 GMT  
		Size: 37.2 MB (37160030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03ededf19de330d97ae5f2cd78f381456f81c19eb46ff80cebace0dbe476eac`  
		Last Modified: Tue, 27 Jul 2021 04:28:02 GMT  
		Size: 4.1 MB (4095072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ec3f753c3934e1f67de00b1cde7c52b2558b372872daab551be31f8ee74787`  
		Last Modified: Tue, 27 Jul 2021 04:28:01 GMT  
		Size: 4.2 MB (4241926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:97bd04e7cd9db63b4fdfd2f347aa020ccedf795d142138f5bc2fbd99b3405f27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34478604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221e715de9dc218092a332bbdf4433b434c800e4703c3f3ab14ad8b5106fbae8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:19:36 GMT
ADD file:84d3daa77b3c4590ccb1b2c1bdfa7b2ea2629a8e289c7e0df33678a72ef40f4c in / 
# Tue, 31 Aug 2021 01:19:38 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:16:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2027d80189558886be09b6f8194607cd27258802c79f3c3f228e92404c40c304`  
		Last Modified: Tue, 31 Aug 2021 01:35:47 GMT  
		Size: 27.2 MB (27192169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccb43db8246e726e33f90f4887b26c5c6e5c0eb9b7c4fd223c18539a9963369`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 3.5 MB (3483280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a66489e611edd2a918d67c7aa380888b297b1b1170487f8cf4d412010e9da74`  
		Last Modified: Tue, 31 Aug 2021 02:53:00 GMT  
		Size: 3.8 MB (3803155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b3f1c9e13e18f3a6e5662bf31762ed9c77414c91bab87c7de91de6a71e1935e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39220762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cc85733e213410e8138f3ac19e6603d3c39f436a8584a4f0df250ce43cb4d2b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:54 GMT
ADD file:4748ab039bb7c33cbda2bba944346ecf2e0e6238971d842acc53ec7e8c77df92 in / 
# Tue, 31 Aug 2021 01:42:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:39:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2abd65908848180c8f2b1a3f2a6493d9c7c22253fc30bc557fce0bbf12327e7`  
		Last Modified: Tue, 31 Aug 2021 01:44:45 GMT  
		Size: 31.3 MB (31308069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f61cb11476011700fc2feeb76881a7eeceb9638e97fa4c33603d64dab544155`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3950090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7802bd74770db74806622bc0f14aa9cc4666241c5b47c5aee05c1b85aa17ebe5`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3962603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.10-scm`

```console
$ docker pull buildpack-deps@sha256:b741ca3cf6c93c9c8a833e446bf46c9b00bc74364aceab9ae0552f81563244f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:21.10-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1568944d072c74d3848ea3b159daa499efb19b8ca24a27be213e3e6706358db2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76642660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99660b61d6e2e864495950c7bade0adea9062dd182f11d88cc8c4554a8e4c3e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:01 GMT
ADD file:aad4137373f37cc2272f1632b0fa50a91b4c0c878ca72ae8de8fee51ffa2f392 in / 
# Mon, 26 Jul 2021 21:22:02 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:59:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c8d2949e37d3f87c8d42e502aebe8d287cc56bd1f5846a5265a2124c60cb49c`  
		Last Modified: Mon, 26 Jul 2021 21:24:04 GMT  
		Size: 31.5 MB (31519889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad149f781f55b2a85f0e013b5220678d294bfdc9a113255a07b8fd871224219`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.7 MB (3692251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11936e1d3aa1eb439ea9dac0215a97aa74b71b1eabeed3965b276ff2c836d5e`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.6 MB (3552048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8ee9b3c3bd20f022701661feb52a5704b01f803876f6ebed7ce76763e8308e`  
		Last Modified: Mon, 26 Jul 2021 22:15:03 GMT  
		Size: 37.9 MB (37878472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:af9428118519e17bc6c573f6e9c0997f45932bd2ccd1de24b26ca842ff185561
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74112565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f107b16cd8f0186dee68e0dc6d339ebdf055d86f1a61044e769517f2b951da30`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:54 GMT
ADD file:7c7c93de372cabbc1cbc45bb3618b626ecd538c81cdb8a09c63b397ac79615ca in / 
# Mon, 26 Jul 2021 22:52:55 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:29:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa3fdc2705d50f3ad184e38a8ae9a54c70a75ef26a8f2036c5cc36454c57b49a`  
		Last Modified: Mon, 26 Jul 2021 22:57:52 GMT  
		Size: 26.9 MB (26876142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05927c7769ed8e7aa2c01453e69c9f65172154a601b0218204df2a1c260a6`  
		Last Modified: Tue, 27 Jul 2021 01:50:05 GMT  
		Size: 3.4 MB (3438752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c89b675bf7d9d2c4ea66630864775dc5879d8e56b1c77d25f08550fd9f882b`  
		Last Modified: Tue, 27 Jul 2021 01:50:04 GMT  
		Size: 3.7 MB (3742290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebac5e3a405d40889f25f311860e0142aaa8172e0dc5fe0de50562f4f0c3a13`  
		Last Modified: Tue, 27 Jul 2021 01:50:46 GMT  
		Size: 40.1 MB (40055381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9b14a5032f9cecabfdd36fdd1f4cf36fe9e77c69c67df42361a09c52ab0056ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3ed19e94cacde52671ebc1c2fc041af08a623bce8a636b1f779768b6f239f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:02 GMT
ADD file:ed3a8c55fbedc627dd5d33aecf52df10becbd9bd492f7c3f4f0a710b15629618 in / 
# Tue, 31 Aug 2021 01:41:03 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:13:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:835dcfefc46e2b5551a40002ffed802b6b70970071e61e3f9dce0dd0404c2a12`  
		Last Modified: Tue, 31 Aug 2021 01:43:19 GMT  
		Size: 29.0 MB (29033527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76d237fe2a405ec5c0175da7117764a3725e495a5280fa68824281d0209f48`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.7 MB (3677477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972cd7eb9f3f8f76c354e0777c1e299b4979c519af36ee25c5a4b5176d14c93b`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.5 MB (3533509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f0c095fc735f206fea57d94ba168122a4d321e4718f54f2db7b3f7c503ed6`  
		Last Modified: Tue, 31 Aug 2021 02:22:17 GMT  
		Size: 38.1 MB (38076803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1465a3eb205a891ac7628435a12af70e11d4d65c5154790ac85cf87d9fff0815
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87786697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12eea146d6a5af6407383e3d75078ee099d3f782c5a9277e03fea2051086cfa`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:33 GMT
ADD file:5419572ba3a583506859cb346c0715939486d87fcc143e308557a18a73bb92b2 in / 
# Mon, 26 Jul 2021 23:13:37 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:49:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:50:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:52:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:415d912bb08e4b766d9582ddc3d0e3c55a978420909d0ce62488cfc6ddcd065d`  
		Last Modified: Mon, 26 Jul 2021 23:17:00 GMT  
		Size: 37.2 MB (37160030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03ededf19de330d97ae5f2cd78f381456f81c19eb46ff80cebace0dbe476eac`  
		Last Modified: Tue, 27 Jul 2021 04:28:02 GMT  
		Size: 4.1 MB (4095072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ec3f753c3934e1f67de00b1cde7c52b2558b372872daab551be31f8ee74787`  
		Last Modified: Tue, 27 Jul 2021 04:28:01 GMT  
		Size: 4.2 MB (4241926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946929704f815af80a61ae55d86531279d22d2292a2f74bf22ed5819c842bb88`  
		Last Modified: Tue, 27 Jul 2021 04:28:22 GMT  
		Size: 42.3 MB (42289669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:614636c66a9fe0c5bdf74d262aea3147673d5e6029e0be438a16320cde474ad5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75219646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df26d2ad97a6b07536755961bac409c36c72d1d41a9afaa589a2659cd1e18050`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:19:36 GMT
ADD file:84d3daa77b3c4590ccb1b2c1bdfa7b2ea2629a8e289c7e0df33678a72ef40f4c in / 
# Tue, 31 Aug 2021 01:19:38 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:16:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:20:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2027d80189558886be09b6f8194607cd27258802c79f3c3f228e92404c40c304`  
		Last Modified: Tue, 31 Aug 2021 01:35:47 GMT  
		Size: 27.2 MB (27192169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccb43db8246e726e33f90f4887b26c5c6e5c0eb9b7c4fd223c18539a9963369`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 3.5 MB (3483280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a66489e611edd2a918d67c7aa380888b297b1b1170487f8cf4d412010e9da74`  
		Last Modified: Tue, 31 Aug 2021 02:53:00 GMT  
		Size: 3.8 MB (3803155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2a8d532c190bc5429a7b1a5b15e55c1c120cd8fd520ce5adcdeacadde8c6cb`  
		Last Modified: Tue, 31 Aug 2021 02:55:01 GMT  
		Size: 40.7 MB (40741042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:182a5862cbeafa138059b2c711748f5fb7b509f7a52ed4488b483b78a2736457
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.1 MB (78078880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd61715f5db10dc5a7fd9b64563d7002600c850a3a00b72c4217f99b4d3dac1f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:54 GMT
ADD file:4748ab039bb7c33cbda2bba944346ecf2e0e6238971d842acc53ec7e8c77df92 in / 
# Tue, 31 Aug 2021 01:42:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:39:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:39:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2abd65908848180c8f2b1a3f2a6493d9c7c22253fc30bc557fce0bbf12327e7`  
		Last Modified: Tue, 31 Aug 2021 01:44:45 GMT  
		Size: 31.3 MB (31308069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f61cb11476011700fc2feeb76881a7eeceb9638e97fa4c33603d64dab544155`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3950090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7802bd74770db74806622bc0f14aa9cc4666241c5b47c5aee05c1b85aa17ebe5`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3962603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e8b1ada6b39a4ab9001051926a2b823d061ce3d31ae907a24efa8fa9961ec`  
		Last Modified: Tue, 31 Aug 2021 02:47:54 GMT  
		Size: 38.9 MB (38858118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:4cb0b413e27ed0dd741da894f4c4df2c4682bd007bcaf850d61d6971536a1185
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:db76b519fe4ec10a7e3137a305dd2be63a918c05b746f114db1b987b22e22feb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221268132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a4d488cd94239a5b2ce1397e8d915523b7d1b355c33c3261a4949dd2082a8e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:41:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:44:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b43550a14e1f5842c45eaf5b0043a8aac335974d12b11847980b58fcfd5416`  
		Last Modified: Mon, 26 Jul 2021 22:10:05 GMT  
		Size: 6.6 MB (6644948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e59c30206e4fabc53c96ec7a836fcdc7cdac49cb93fc1b8e376733f4379cfb`  
		Last Modified: Mon, 26 Jul 2021 22:10:04 GMT  
		Size: 3.0 MB (3022291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83c7b2c1eed3a521091d24d714249fb2ee4d8497ba2878141cdd2e4ef3307ef`  
		Last Modified: Mon, 26 Jul 2021 22:10:23 GMT  
		Size: 45.5 MB (45478045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b304099eada42901a68ef5bc8b9f5e19f3bccbf73f7a4062ef0e632913d707`  
		Last Modified: Mon, 26 Jul 2021 22:10:54 GMT  
		Size: 139.4 MB (139413809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d017441d8eeb74735b24ef0361d055928bb725a022644e30658ff36773cb66c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189468139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d890fd1dc3c418299ddfcd5bde9f151f59d68b6cfc60f449cdce804c20134f41`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:14:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:17:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef2837cc6a640557235061b89ed9a389330802f062137cb313376de279870b`  
		Last Modified: Tue, 27 Jul 2021 01:40:03 GMT  
		Size: 5.7 MB (5715357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec9e4b1e75d299207a4006fe43a2e34c3fda90619c762ebc07dc792b034642`  
		Last Modified: Tue, 27 Jul 2021 01:40:01 GMT  
		Size: 2.6 MB (2584467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b636a25e91fe1c88dd15eed3996e0fab60a372c08ebd491408a5eded9d63e`  
		Last Modified: Tue, 27 Jul 2021 01:40:45 GMT  
		Size: 40.7 MB (40671352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee68967ed05e4e5f5edeb14149e1f19b65ea7ff79677978279aa829747e3dfd`  
		Last Modified: Tue, 27 Jul 2021 01:42:10 GMT  
		Size: 118.2 MB (118190111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4848544ea47bd7455408a1ae8882ea0d9f5f8e9d98738aac32d9b73d1419e43e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205819460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e60a0155dcd6083f89bac96420a7a44c0124d5959d08d13db05d7dba2a7b0bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:08:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:10:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a9b8c6709cd3ea323ffea2dcfa72913a9fdc73837573db0ffa663995a44a8`  
		Last Modified: Tue, 31 Aug 2021 02:18:37 GMT  
		Size: 6.1 MB (6087650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ad199f9143cc4082ab5e445c913e284b9f2ec63abce0b6b1243561e2810a77`  
		Last Modified: Tue, 31 Aug 2021 02:18:36 GMT  
		Size: 2.8 MB (2783046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b0514655b3d63ab1f59062bfc8bb2558e7cd9fa05297f66339c11b8952f14`  
		Last Modified: Tue, 31 Aug 2021 02:18:56 GMT  
		Size: 43.3 MB (43267405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6280417b2b490b9a8901d624796b899f9b1f775f39ea1c22af94e7c56a3a34`  
		Last Modified: Tue, 31 Aug 2021 02:19:28 GMT  
		Size: 130.0 MB (129950760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f23a63bd9ab658549e68c52f94e44d1338ae54b1ddca7813c01a6eaa1fcabf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.6 MB (218557666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be5b26d5d1607ab1318e4cce89d6fa77e0516b8783f4db371ccffb3181b5b3b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:57:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:57:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 01:58:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:02:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c7d08d74fca5ace99c2318c3f53f795d5cd713e8df0f41ea3c071a3583372`  
		Last Modified: Tue, 31 Aug 2021 02:09:50 GMT  
		Size: 6.9 MB (6934539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c005ec2b9b98efae8ad7204dd1b1e216eabe229174d28fb5b62c9489ea0`  
		Last Modified: Tue, 31 Aug 2021 02:09:49 GMT  
		Size: 3.3 MB (3252591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40ed14ecd7476315d1f56a8f79f2d48dbad24c195129de044ff6bec685c1613`  
		Last Modified: Tue, 31 Aug 2021 02:10:12 GMT  
		Size: 47.1 MB (47064814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5727719ec2e3d390427c8b8e5fbb7364b3815d04a5147791810cf0fed1474ded`  
		Last Modified: Tue, 31 Aug 2021 02:10:49 GMT  
		Size: 134.1 MB (134143285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9f098d17e856cd5b8fe8ea9f3f39ddf2d77d5da7eb51377f8372fc3e58ab2293
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246217653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6b8c7e9e5a5250a8424c3a99be2d39a0b37cd1abc0fb17b6c0617016e472c3`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:58:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:00:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:06:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475513220a5f30414e690523f753a7a744d3d79b2e0d3cff2d05038e334855a4`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 7.1 MB (7057571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb47fd0ae4274e4d82eec5939329f2aa19c6aaecea4b7e24ccdf34312d95fa8`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 3.7 MB (3719539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0163b280cc161a9528fe1241bdc8a90792874475962941c0f97f2636ec4fc29b`  
		Last Modified: Tue, 27 Jul 2021 04:23:04 GMT  
		Size: 53.7 MB (53715172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61938bdfeed9504952a3e61e49ab0f2e1e17b73d45b28bbffb301cf2744b2fd`  
		Last Modified: Tue, 27 Jul 2021 04:23:43 GMT  
		Size: 151.3 MB (151287413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d2a81bb11386e6802a1e807c1339805562c882b7a1d5619dacb477d99e24e391
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.6 MB (205611586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80fb7da4bcc563d3ea3bbcb40a0c1006159dfd7da2694dff0841a6fbf42ff8f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:34:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:34:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae5daa9a040b93bff6544ad59a003cd958048bef64a9f991a5d3150888fcbed`  
		Last Modified: Tue, 31 Aug 2021 02:45:10 GMT  
		Size: 6.3 MB (6335758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bbf8f7d5625c28aa637939c7029792a4f3b624e300c59cb77575fe7aa84d14`  
		Last Modified: Tue, 31 Aug 2021 02:45:12 GMT  
		Size: 3.0 MB (2974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4165862f9e51452154c0ba3b4ce42f4a8fa2b092d9d4e6c46b46770a5ad6015`  
		Last Modified: Tue, 31 Aug 2021 02:45:26 GMT  
		Size: 45.0 MB (45016355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6def741b217bbfd1346c96876005a3004b76da3416c4839d8c26d070abf3b5`  
		Last Modified: Tue, 31 Aug 2021 02:45:50 GMT  
		Size: 125.9 MB (125918073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:78a5c19460736d0826ae13f4b766abf2737fd1c73b3356de7cd3da0ffc11ef5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5d53242a937ee00a3323ef4e7faf6fbc84427a5a66a0581e4cb613b9d83ac099
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36376278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d8990e61ac993b6bb50cd509110e224244289b417364b5bacb145ff1c496568`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b43550a14e1f5842c45eaf5b0043a8aac335974d12b11847980b58fcfd5416`  
		Last Modified: Mon, 26 Jul 2021 22:10:05 GMT  
		Size: 6.6 MB (6644948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e59c30206e4fabc53c96ec7a836fcdc7cdac49cb93fc1b8e376733f4379cfb`  
		Last Modified: Mon, 26 Jul 2021 22:10:04 GMT  
		Size: 3.0 MB (3022291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8cd88ad50e848014c72124a58f84fbe85a33a7ce5932658c6e730d6dbb59fba9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30606676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18bd33d28415880a949129908f93919248f16bc8d8fe5d4251e57dd8bbd9107e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:14:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef2837cc6a640557235061b89ed9a389330802f062137cb313376de279870b`  
		Last Modified: Tue, 27 Jul 2021 01:40:03 GMT  
		Size: 5.7 MB (5715357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec9e4b1e75d299207a4006fe43a2e34c3fda90619c762ebc07dc792b034642`  
		Last Modified: Tue, 27 Jul 2021 01:40:01 GMT  
		Size: 2.6 MB (2584467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5d962e80ddffea4d545bda177e9840d262fb1893cdac6acc8cc3863bf9de75bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32601295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34eb7034c339584e265fb320d1e0d2496baa28988e145f56a72254e7ec081ad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:08:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a9b8c6709cd3ea323ffea2dcfa72913a9fdc73837573db0ffa663995a44a8`  
		Last Modified: Tue, 31 Aug 2021 02:18:37 GMT  
		Size: 6.1 MB (6087650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ad199f9143cc4082ab5e445c913e284b9f2ec63abce0b6b1243561e2810a77`  
		Last Modified: Tue, 31 Aug 2021 02:18:36 GMT  
		Size: 2.8 MB (2783046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:77c62e1928a0a02b1eb69d7cda933975816c77ee2ba1e333f2cb8d916bd3bf92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e6101ebd52b5a1c60f03a674e775c8fa0244a300cbadc8c8f42793a4f5e1b6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:57:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:57:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c7d08d74fca5ace99c2318c3f53f795d5cd713e8df0f41ea3c071a3583372`  
		Last Modified: Tue, 31 Aug 2021 02:09:50 GMT  
		Size: 6.9 MB (6934539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c005ec2b9b98efae8ad7204dd1b1e216eabe229174d28fb5b62c9489ea0`  
		Last Modified: Tue, 31 Aug 2021 02:09:49 GMT  
		Size: 3.3 MB (3252591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2d73cdf00577962a4ff175511e9ae4165e9772824f2aaf3bf2fd988eab5e593e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41215068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232490ed0858a7bf31e6a80f877808b2daea11c077fe994699f1d5db1808aa43`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:58:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475513220a5f30414e690523f753a7a744d3d79b2e0d3cff2d05038e334855a4`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 7.1 MB (7057571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb47fd0ae4274e4d82eec5939329f2aa19c6aaecea4b7e24ccdf34312d95fa8`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 3.7 MB (3719539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b1f689b30d2ae3be28a65adc94df539028bd0f5346b14cbeb8e12d90f6cc549b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34677158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849662eb467d6d767b9ef21110d9f00f5b75c83c278ee84bef70c174b2e1af68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:34:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:34:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae5daa9a040b93bff6544ad59a003cd958048bef64a9f991a5d3150888fcbed`  
		Last Modified: Tue, 31 Aug 2021 02:45:10 GMT  
		Size: 6.3 MB (6335758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bbf8f7d5625c28aa637939c7029792a4f3b624e300c59cb77575fe7aa84d14`  
		Last Modified: Tue, 31 Aug 2021 02:45:12 GMT  
		Size: 3.0 MB (2974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:a644d5154527dfdb870b98ab060a5383cfe5956bd32b0cda170d8d72e6aa4a7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d86fa220ec910630351b465c36ec06dff76bee05696b129299e2c652fc02770c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81854323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5862355d4afcb1279e2c4f94df12c33a3edf245e67c761982addc0a96aed5f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:41:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b43550a14e1f5842c45eaf5b0043a8aac335974d12b11847980b58fcfd5416`  
		Last Modified: Mon, 26 Jul 2021 22:10:05 GMT  
		Size: 6.6 MB (6644948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e59c30206e4fabc53c96ec7a836fcdc7cdac49cb93fc1b8e376733f4379cfb`  
		Last Modified: Mon, 26 Jul 2021 22:10:04 GMT  
		Size: 3.0 MB (3022291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83c7b2c1eed3a521091d24d714249fb2ee4d8497ba2878141cdd2e4ef3307ef`  
		Last Modified: Mon, 26 Jul 2021 22:10:23 GMT  
		Size: 45.5 MB (45478045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eb9be4475bf74a12bd2dc33ceda28b14add9042751ede89f1fb2a6d9faa22520
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71278028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76e3a6ee7bd29db1e8e162d6139a74479adf24b065995e04ca0ef15da83f92ba`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:14:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef2837cc6a640557235061b89ed9a389330802f062137cb313376de279870b`  
		Last Modified: Tue, 27 Jul 2021 01:40:03 GMT  
		Size: 5.7 MB (5715357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec9e4b1e75d299207a4006fe43a2e34c3fda90619c762ebc07dc792b034642`  
		Last Modified: Tue, 27 Jul 2021 01:40:01 GMT  
		Size: 2.6 MB (2584467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b636a25e91fe1c88dd15eed3996e0fab60a372c08ebd491408a5eded9d63e`  
		Last Modified: Tue, 27 Jul 2021 01:40:45 GMT  
		Size: 40.7 MB (40671352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:879d52f67da8265f7281b54a011a310ae60d4259ed0dfa396bbadd952a903194
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75868700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea1033b4a10ea257078c5937872da1e61e4c54657bab409800e24b6fa9b8387`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:08:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a9b8c6709cd3ea323ffea2dcfa72913a9fdc73837573db0ffa663995a44a8`  
		Last Modified: Tue, 31 Aug 2021 02:18:37 GMT  
		Size: 6.1 MB (6087650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ad199f9143cc4082ab5e445c913e284b9f2ec63abce0b6b1243561e2810a77`  
		Last Modified: Tue, 31 Aug 2021 02:18:36 GMT  
		Size: 2.8 MB (2783046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b0514655b3d63ab1f59062bfc8bb2558e7cd9fa05297f66339c11b8952f14`  
		Last Modified: Tue, 31 Aug 2021 02:18:56 GMT  
		Size: 43.3 MB (43267405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:80ed2caa4aebc97f6433751e1a0dec62b247c6441fc9dfc5e03d5ecf077e74a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84414381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187f4d53dff720ac9125839acc899f6410afcdf09c08c95113c58bdddc96e0de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:57:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:57:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 01:58:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c7d08d74fca5ace99c2318c3f53f795d5cd713e8df0f41ea3c071a3583372`  
		Last Modified: Tue, 31 Aug 2021 02:09:50 GMT  
		Size: 6.9 MB (6934539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c005ec2b9b98efae8ad7204dd1b1e216eabe229174d28fb5b62c9489ea0`  
		Last Modified: Tue, 31 Aug 2021 02:09:49 GMT  
		Size: 3.3 MB (3252591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40ed14ecd7476315d1f56a8f79f2d48dbad24c195129de044ff6bec685c1613`  
		Last Modified: Tue, 31 Aug 2021 02:10:12 GMT  
		Size: 47.1 MB (47064814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5560e162ea83b6f1a2733d0220352b08ebd8bc5fc91cc006df0bef9e6e17eca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94930240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c560aaa81eaecde3e480a2c97282274c384cda23e6a51e23e9cad9abf5044b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:58:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:00:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475513220a5f30414e690523f753a7a744d3d79b2e0d3cff2d05038e334855a4`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 7.1 MB (7057571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb47fd0ae4274e4d82eec5939329f2aa19c6aaecea4b7e24ccdf34312d95fa8`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 3.7 MB (3719539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0163b280cc161a9528fe1241bdc8a90792874475962941c0f97f2636ec4fc29b`  
		Last Modified: Tue, 27 Jul 2021 04:23:04 GMT  
		Size: 53.7 MB (53715172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6096e767e06165c5154a89c49c3e30bfd9416c6cd6063469118001dbaff6bacd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79693513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709ce7c063bed950b79272f6ad291f8ee966181136bbb2c9bd8ac20f2f4f3617`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:34:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:34:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae5daa9a040b93bff6544ad59a003cd958048bef64a9f991a5d3150888fcbed`  
		Last Modified: Tue, 31 Aug 2021 02:45:10 GMT  
		Size: 6.3 MB (6335758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bbf8f7d5625c28aa637939c7029792a4f3b624e300c59cb77575fe7aa84d14`  
		Last Modified: Tue, 31 Aug 2021 02:45:12 GMT  
		Size: 3.0 MB (2974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4165862f9e51452154c0ba3b4ce42f4a8fa2b092d9d4e6c46b46770a5ad6015`  
		Last Modified: Tue, 31 Aug 2021 02:45:26 GMT  
		Size: 45.0 MB (45016355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:f84b3ee2dd5104bbb1d77aae6a898d8f1e2a7fa0af22f175b7550ec17ba09df1
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
$ docker pull buildpack-deps@sha256:cafaa221feb7c182ed3c3f83f0086da57bc7156c30159366155c5897a86d915b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (321951029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe8fece98de2233a5a26a59d08ff969b8b55b7fbc1a1c6e7ceb6b22ec659b884`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf565088aae3ef2159885f29853bce88eb16082b0c98fcacd08fc9008c84b9`  
		Last Modified: Tue, 17 Aug 2021 09:29:09 GMT  
		Size: 5.2 MB (5153283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c0dd0dc0d3d367cc5b85f86d8881afb658e8eb341a86daf3835c2f14159ac`  
		Last Modified: Tue, 17 Aug 2021 09:29:10 GMT  
		Size: 10.9 MB (10871829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf06daf65610482c638dcc63479a8281e667e37f7842219d66f2dedf63718f4`  
		Last Modified: Tue, 17 Aug 2021 09:29:34 GMT  
		Size: 54.6 MB (54565734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942374d5c11438b68e78d44b36c9eac8fe0a2570c33681d7263b0f3f069c06b9`  
		Last Modified: Tue, 17 Aug 2021 09:30:21 GMT  
		Size: 196.4 MB (196445179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b9c95648c1c4f6bc00721365da71edf685136b260eb2cc57266229470473ce2c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.0 MB (295049846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c41fc84b081c31c9c20ab9f272e38b3482520d7acbd98f04ae0efeaecc5abf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:18:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:21:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b0b6b82f848e8ef423a421d5d46194f7787ebf23e3dcc69fb177eb4dc49f6`  
		Last Modified: Tue, 17 Aug 2021 09:36:54 GMT  
		Size: 5.1 MB (5063684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02ecba39f2b03f1bc47ed6ba17c15a62b11e7eb2ae7397ba374851a864efc67`  
		Last Modified: Tue, 17 Aug 2021 09:36:55 GMT  
		Size: 10.6 MB (10570968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f083cd711c027bf75e496fb0a9b4e8e2ac1a102c5fc0d01c3375757fc102a526`  
		Last Modified: Tue, 17 Aug 2021 09:37:46 GMT  
		Size: 52.3 MB (52319253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c87f1282078740238a813920e2dab455ea24e91c18b10b6e89bfc34d3dabe5`  
		Last Modified: Tue, 17 Aug 2021 09:39:41 GMT  
		Size: 174.6 MB (174643701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:20a100f794f73d9565aeb095033cbd7d03958c4f5cace47051a44b242b46e4e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282478824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648d40b55ba7c2d96aacdb0170baba32efd26ffb7e7e26cb74e8422a52c6fdce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:12:37 GMT
ADD file:579ac9b41923db9165f333faac1330f2924a14f90cab7605ffd66c1815249adf in / 
# Tue, 17 Aug 2021 02:12:38 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:20:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1ce31b8c318c8eac9eba15cdf329f397a64952ab575a09c167fc9ddc5a991a98`  
		Last Modified: Tue, 17 Aug 2021 02:28:44 GMT  
		Size: 50.1 MB (50118546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5a38f951962ad43cfef6137e6638004e3a3f066bb26e2c3b52489258a4b5c`  
		Last Modified: Tue, 17 Aug 2021 15:38:06 GMT  
		Size: 4.9 MB (4922570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a545de7dcb8f9fe8fd65b3b1f104abbb20cee600bc8602beef63ccc4f6259`  
		Last Modified: Tue, 17 Aug 2021 15:38:08 GMT  
		Size: 10.2 MB (10216795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0801bbb4cc34f3ceed00d5e57c23d39f3f1763075f34e2b90a80f078ae6d486a`  
		Last Modified: Tue, 17 Aug 2021 15:38:59 GMT  
		Size: 50.3 MB (50328392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3d7c49ff6810d965ef9be32d59d7da22bf3dd967c4d1f3b3414a7aed7b5ed9`  
		Last Modified: Tue, 17 Aug 2021 15:40:48 GMT  
		Size: 166.9 MB (166892521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c5716ed801cb5ff800dbe3f9364795dc7bbbb0bcea2c08b0b00a0a9def980c69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313622714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787980177678b9ae90f4b44fc98c5baf6b6e494714c2a083736d7ed49fed43db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:52:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:52:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495d06e79f81fe42766bacea59684f27db9d24960b6dd7efeea81f48820d0f6`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 5.1 MB (5142588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd18a2d3ce3a400515ed7a845aeb9d8cd17b023f1efe77ff81292bd63addcc0`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 10.9 MB (10872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfd3a44e1c9b9d3df6b60162d29469b5fe3aaddecba7bf2b122ced08e2a848`  
		Last Modified: Tue, 17 Aug 2021 08:01:25 GMT  
		Size: 54.7 MB (54670308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e87d255e4f38e1f000f523e71beef3ea90c78d187cbca6373c8bcdc15dab325`  
		Last Modified: Tue, 17 Aug 2021 08:02:07 GMT  
		Size: 189.3 MB (189336134 bytes)  
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
$ docker pull buildpack-deps@sha256:e56dff8e57c911a088985665f4838cb934b32307330794016163f6bc43f101c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301388823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0407593e24bc9c23a80aec36f20f500b78d2e8635f06aecd1e722db0bc94edf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:42:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:45:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d42212351d464cda967a0b9462fdbf31cf8b926ec739f94ca92a04924b59b44`  
		Last Modified: Tue, 17 Aug 2021 20:53:57 GMT  
		Size: 5.1 MB (5114876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f443b77bd62cad6049ac9b935c37714988629b9b90804c902ebf5d94db0947`  
		Last Modified: Tue, 17 Aug 2021 20:53:59 GMT  
		Size: 10.9 MB (10873298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f994e51a722336aa2b759033a359755271ce92b5d1948340ac2760bd28d90a8`  
		Last Modified: Tue, 17 Aug 2021 20:54:52 GMT  
		Size: 53.3 MB (53297838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb32760aefab4b67e850394277f734a5e65f8191fb6c3dd5e43b4c1577e4c61`  
		Last Modified: Tue, 17 Aug 2021 20:57:03 GMT  
		Size: 178.9 MB (178935476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3035d395cdd02846678666bf0e6fdbafe0fcc72f36134d4cc968c3fc48667386
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330493921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d3e26c8948f38abc9f03d8319b316eb0204deca02aa44662b8ef9338ec5ed0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 14:34:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:53:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f9b82c933b317ed127f45e6f56d6d7508514459e0ef09073b467d3dd8425e`  
		Last Modified: Tue, 17 Aug 2021 15:58:19 GMT  
		Size: 5.4 MB (5401864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a6114ee4fe00702ca86cd44f229643d9324c4b202ed6583f35d2eca848a4a`  
		Last Modified: Tue, 17 Aug 2021 15:58:18 GMT  
		Size: 11.6 MB (11626128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e91c7e9879fdf8ce8ef16f2ba105dac2bc4d76888c86b7b5c63973c05f7ed4`  
		Last Modified: Tue, 17 Aug 2021 16:00:07 GMT  
		Size: 58.8 MB (58849860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8542edff3433d9f519b8030bb7b7f200e5cec504915eda9435d627020680c`  
		Last Modified: Tue, 17 Aug 2021 16:04:00 GMT  
		Size: 195.8 MB (195800037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8b7e5e3f28327cce774548f9e1559535aacb731aa486537b0b1c5458c81caddf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295572826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:186802d3daef183bcf0a403c0ce38346f8c731d225920fe8893adc7c58b07151`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:32:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:32:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20bd918649e02578e4e6f19a2c873dbcc6da7009f7b4ee3088a3e2f594fe6e`  
		Last Modified: Tue, 17 Aug 2021 07:43:16 GMT  
		Size: 5.1 MB (5137099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e43baff5e6307dfe51df170140aa3c7c4b7a4cb3fb03b3a2255a8038c9542`  
		Last Modified: Tue, 17 Aug 2021 07:43:17 GMT  
		Size: 10.8 MB (10761504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163c4ba4cbac76aa2dccf627dc69a5f47c32176dc12e23d0bbbfaa6723a446`  
		Last Modified: Tue, 17 Aug 2021 07:43:35 GMT  
		Size: 54.1 MB (54050153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc89d77adebd4b8848cee8bc0ed80f335c59bbc0b93c29b608cef22175243fe`  
		Last Modified: Tue, 17 Aug 2021 07:44:05 GMT  
		Size: 172.4 MB (172430038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:fdd2452507132b7a4c6b432c32e159f15d955afa4258e5b8f64b7fdc7add487f
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f2aebefdccca99d265c8e84738ee9f99c36f4212ca051d43b4683798dfb42636
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70940116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6fe7405525d60b20905a08baa979b62312fdb03b9a48e235baebfc59977f2c2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf565088aae3ef2159885f29853bce88eb16082b0c98fcacd08fc9008c84b9`  
		Last Modified: Tue, 17 Aug 2021 09:29:09 GMT  
		Size: 5.2 MB (5153283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c0dd0dc0d3d367cc5b85f86d8881afb658e8eb341a86daf3835c2f14159ac`  
		Last Modified: Tue, 17 Aug 2021 09:29:10 GMT  
		Size: 10.9 MB (10871829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b2e1e86e8147e79ba83867e74aa1a9fa3b677f764ef0a9d7e3cae46c5ad2669d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68086892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c4086386b6b216789ae1d7d834ccfd24e3cae7f8d6d9f2d9dfa493924d3cc3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:18:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b0b6b82f848e8ef423a421d5d46194f7787ebf23e3dcc69fb177eb4dc49f6`  
		Last Modified: Tue, 17 Aug 2021 09:36:54 GMT  
		Size: 5.1 MB (5063684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02ecba39f2b03f1bc47ed6ba17c15a62b11e7eb2ae7397ba374851a864efc67`  
		Last Modified: Tue, 17 Aug 2021 09:36:55 GMT  
		Size: 10.6 MB (10570968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:65059ed8ae5f1dcdde3da0bb274969b7cca178755ccd40eee90ae54fde9e89fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65257911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c4021355832ed254e558058a0774730787867c0d43269189b5abea64f2fe0b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:12:37 GMT
ADD file:579ac9b41923db9165f333faac1330f2924a14f90cab7605ffd66c1815249adf in / 
# Tue, 17 Aug 2021 02:12:38 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1ce31b8c318c8eac9eba15cdf329f397a64952ab575a09c167fc9ddc5a991a98`  
		Last Modified: Tue, 17 Aug 2021 02:28:44 GMT  
		Size: 50.1 MB (50118546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5a38f951962ad43cfef6137e6638004e3a3f066bb26e2c3b52489258a4b5c`  
		Last Modified: Tue, 17 Aug 2021 15:38:06 GMT  
		Size: 4.9 MB (4922570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a545de7dcb8f9fe8fd65b3b1f104abbb20cee600bc8602beef63ccc4f6259`  
		Last Modified: Tue, 17 Aug 2021 15:38:08 GMT  
		Size: 10.2 MB (10216795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fe66fbc885d81fdafbe18713a6165c8028b9ed9939b65497ab53bdf98e963213
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69616272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48afe04239a66261d25a64f298c4fa2467895f8861bcf70bcc11a0248523fb5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:52:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:52:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495d06e79f81fe42766bacea59684f27db9d24960b6dd7efeea81f48820d0f6`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 5.1 MB (5142588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd18a2d3ce3a400515ed7a845aeb9d8cd17b023f1efe77ff81292bd63addcc0`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 10.9 MB (10872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e593b0b7e666a4ee388aec91360e9d8414ec6b6846bab3c97d2fad8f754445d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72456123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f08f2eeb7d00459ae8f10b008928c02a6c5ad7cbd65e4e0ab0ead6da5ba4b05c`
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

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5617c8a692ae2f2d66e61c9353dd8f51a5584d8d3bc9247c10af1c8ed8b9fa49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69155509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efea973f65ee025f05845863859e9962cff13e166db36866230ec2619834163e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d42212351d464cda967a0b9462fdbf31cf8b926ec739f94ca92a04924b59b44`  
		Last Modified: Tue, 17 Aug 2021 20:53:57 GMT  
		Size: 5.1 MB (5114876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f443b77bd62cad6049ac9b935c37714988629b9b90804c902ebf5d94db0947`  
		Last Modified: Tue, 17 Aug 2021 20:53:59 GMT  
		Size: 10.9 MB (10873298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7c55dd439b7bc0da37bc1d85c237a140966ff47444714b599ceb42724bb68232
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75844024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c6a017b4350c90fd80678152fdf7e17a772a4b8585ddad57bdb2cb34e56a59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f9b82c933b317ed127f45e6f56d6d7508514459e0ef09073b467d3dd8425e`  
		Last Modified: Tue, 17 Aug 2021 15:58:19 GMT  
		Size: 5.4 MB (5401864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a6114ee4fe00702ca86cd44f229643d9324c4b202ed6583f35d2eca848a4a`  
		Last Modified: Tue, 17 Aug 2021 15:58:18 GMT  
		Size: 11.6 MB (11626128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:86da00cec8807a6fca2c5dc68ebe2887651da5b291cee956ee1b61e0a2ec85d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69092635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1b1429c9e37360be6c7c7fb3e2850f6c59962e4669641fdc1cbb2dfe99a8241`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:32:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20bd918649e02578e4e6f19a2c873dbcc6da7009f7b4ee3088a3e2f594fe6e`  
		Last Modified: Tue, 17 Aug 2021 07:43:16 GMT  
		Size: 5.1 MB (5137099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e43baff5e6307dfe51df170140aa3c7c4b7a4cb3fb03b3a2255a8038c9542`  
		Last Modified: Tue, 17 Aug 2021 07:43:17 GMT  
		Size: 10.8 MB (10761504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:7c9700c28be70bfd3bae7ec1bca0be928e089a0dabeac1547d9d01821dc1137e
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

### `buildpack-deps:bullseye-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fcf696e81fbb39515e31895fbeedb08b0bf07e1bc8bfac1094b1f4adfebad8e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125505850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f8c023a59a00085d55f58463800a73350f5a479bc85bd8fec65c6d63c59b9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf565088aae3ef2159885f29853bce88eb16082b0c98fcacd08fc9008c84b9`  
		Last Modified: Tue, 17 Aug 2021 09:29:09 GMT  
		Size: 5.2 MB (5153283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c0dd0dc0d3d367cc5b85f86d8881afb658e8eb341a86daf3835c2f14159ac`  
		Last Modified: Tue, 17 Aug 2021 09:29:10 GMT  
		Size: 10.9 MB (10871829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf06daf65610482c638dcc63479a8281e667e37f7842219d66f2dedf63718f4`  
		Last Modified: Tue, 17 Aug 2021 09:29:34 GMT  
		Size: 54.6 MB (54565734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f4f9aaf82aa16a66de2601280af242b6eed140501fdefc27dbddaee1a2abd04d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120406145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7f7ffa4516f21995c9d82c55032542d253b9c19f3e8a3c7a5a351e3f28904bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:18:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b0b6b82f848e8ef423a421d5d46194f7787ebf23e3dcc69fb177eb4dc49f6`  
		Last Modified: Tue, 17 Aug 2021 09:36:54 GMT  
		Size: 5.1 MB (5063684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02ecba39f2b03f1bc47ed6ba17c15a62b11e7eb2ae7397ba374851a864efc67`  
		Last Modified: Tue, 17 Aug 2021 09:36:55 GMT  
		Size: 10.6 MB (10570968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f083cd711c027bf75e496fb0a9b4e8e2ac1a102c5fc0d01c3375757fc102a526`  
		Last Modified: Tue, 17 Aug 2021 09:37:46 GMT  
		Size: 52.3 MB (52319253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:952205bc7cddbbfb9fa8d02a6b6359b25693f6c583577f30ae38f6fc953128d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115586303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67953dbcbb8bcfebe0afc9db6d95f9f661b8a7f422c688642a536fd858e9d5a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:12:37 GMT
ADD file:579ac9b41923db9165f333faac1330f2924a14f90cab7605ffd66c1815249adf in / 
# Tue, 17 Aug 2021 02:12:38 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1ce31b8c318c8eac9eba15cdf329f397a64952ab575a09c167fc9ddc5a991a98`  
		Last Modified: Tue, 17 Aug 2021 02:28:44 GMT  
		Size: 50.1 MB (50118546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5a38f951962ad43cfef6137e6638004e3a3f066bb26e2c3b52489258a4b5c`  
		Last Modified: Tue, 17 Aug 2021 15:38:06 GMT  
		Size: 4.9 MB (4922570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a545de7dcb8f9fe8fd65b3b1f104abbb20cee600bc8602beef63ccc4f6259`  
		Last Modified: Tue, 17 Aug 2021 15:38:08 GMT  
		Size: 10.2 MB (10216795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0801bbb4cc34f3ceed00d5e57c23d39f3f1763075f34e2b90a80f078ae6d486a`  
		Last Modified: Tue, 17 Aug 2021 15:38:59 GMT  
		Size: 50.3 MB (50328392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7466552e59983c946898f07f77837b743f3b156ff789fc751ee98a02a9add3b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124286580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d51b8f3ab483064d973aecc62a3b04b730815b474f7f9793cd107f3f79f6dad2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:52:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:52:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495d06e79f81fe42766bacea59684f27db9d24960b6dd7efeea81f48820d0f6`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 5.1 MB (5142588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd18a2d3ce3a400515ed7a845aeb9d8cd17b023f1efe77ff81292bd63addcc0`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 10.9 MB (10872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfd3a44e1c9b9d3df6b60162d29469b5fe3aaddecba7bf2b122ced08e2a848`  
		Last Modified: Tue, 17 Aug 2021 08:01:25 GMT  
		Size: 54.7 MB (54670308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:00be0f57bc7e719a20f1fa7c7544e0df9c6853fb707efac9b901c65b6c06ba5a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128372373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca098a2a0c1d25e4bb10cde9432093d0aa17de51005d3952d00ec8f1d6b262b2`
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

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:03f5904c242d11766ad5bf5183be9e7630b9e37d9670519c71a54b93a9c4d095
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122453347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63db1c68912deb8496753716857c5912bdf02ca2a4bad7229ef3b7bdeab044a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:42:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d42212351d464cda967a0b9462fdbf31cf8b926ec739f94ca92a04924b59b44`  
		Last Modified: Tue, 17 Aug 2021 20:53:57 GMT  
		Size: 5.1 MB (5114876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f443b77bd62cad6049ac9b935c37714988629b9b90804c902ebf5d94db0947`  
		Last Modified: Tue, 17 Aug 2021 20:53:59 GMT  
		Size: 10.9 MB (10873298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f994e51a722336aa2b759033a359755271ce92b5d1948340ac2760bd28d90a8`  
		Last Modified: Tue, 17 Aug 2021 20:54:52 GMT  
		Size: 53.3 MB (53297838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fcbc2251bc93c2efb3d7fba801d28ae0f31bcd293b3ba7c7a232d9dd37ba5578
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134693884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d90068795b93d0a5374de038dbf136ba1114dd082e28d5b649c0406f044c8fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 14:34:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f9b82c933b317ed127f45e6f56d6d7508514459e0ef09073b467d3dd8425e`  
		Last Modified: Tue, 17 Aug 2021 15:58:19 GMT  
		Size: 5.4 MB (5401864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a6114ee4fe00702ca86cd44f229643d9324c4b202ed6583f35d2eca848a4a`  
		Last Modified: Tue, 17 Aug 2021 15:58:18 GMT  
		Size: 11.6 MB (11626128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e91c7e9879fdf8ce8ef16f2ba105dac2bc4d76888c86b7b5c63973c05f7ed4`  
		Last Modified: Tue, 17 Aug 2021 16:00:07 GMT  
		Size: 58.8 MB (58849860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5bae3f8d99ee48e52b19e9cd49f9ecfd1154979fb8ab49ec52a4f4d74ba5cdae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123142788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8878de09ccb0b4cf42119e9df2aaefcfc61cbfc3ce818b2f70133e76585d8413`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:32:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:32:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20bd918649e02578e4e6f19a2c873dbcc6da7009f7b4ee3088a3e2f594fe6e`  
		Last Modified: Tue, 17 Aug 2021 07:43:16 GMT  
		Size: 5.1 MB (5137099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e43baff5e6307dfe51df170140aa3c7c4b7a4cb3fb03b3a2255a8038c9542`  
		Last Modified: Tue, 17 Aug 2021 07:43:17 GMT  
		Size: 10.8 MB (10761504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163c4ba4cbac76aa2dccf627dc69a5f47c32176dc12e23d0bbbfaa6723a446`  
		Last Modified: Tue, 17 Aug 2021 07:43:35 GMT  
		Size: 54.1 MB (54050153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:ad1d4fa28be6745ab3df67d99e62f5833dd59d4960ecbd707335306fa85ff442
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

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ff472a5ff4bd7253818dfb92e99eee39991da84764d17477d3fad07f06ab1141
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312501525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95271c703a8640d6bc8140abe60bf7dab2e0d95b99f10c284404dcc42e9fce73`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:21:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4099a935a96edef1e9378de34e314d07fb3aea1b7205774055a1fa44a3819f4`  
		Last Modified: Tue, 17 Aug 2021 09:30:37 GMT  
		Size: 7.8 MB (7833079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e2960d83651b1494b4da6c97686e79cc760aa90a75948eed56786726f86928`  
		Last Modified: Tue, 17 Aug 2021 09:30:38 GMT  
		Size: 10.0 MB (9997209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffd4e6385927b79e4d4daa2d00523e766502eed6dd1934e1eda583d348abd8b`  
		Last Modified: Tue, 17 Aug 2021 09:30:58 GMT  
		Size: 51.8 MB (51841042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce46ad6f244a871abfead80f28a613b68fba68e165467d817e09453b369252f`  
		Last Modified: Tue, 17 Aug 2021 09:31:38 GMT  
		Size: 192.4 MB (192393994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:364f2e1bd615a23683b10fdfdb92ae50c06489c895c1ff397dce0c8cc208c57c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286119589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15cdf2a53ae111b3303afe4ac8fbae51a121204bbf99d9e1da4b96b85a705d9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:56:17 GMT
ADD file:784cabdb8b1e35aff6dcfa7acb3c6da5d76ee575188460537a190bab6ef49655 in / 
# Tue, 17 Aug 2021 01:56:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:25:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce5dcedb6ed028586f61d36e8067567349cb049735f9b1fbeb748a005636b9d9`  
		Last Modified: Tue, 17 Aug 2021 02:11:57 GMT  
		Size: 48.2 MB (48153800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1036818934ab73ac9c3e731432ae2c2c576a342f8ac27c0de1654407945f2b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 7.4 MB (7376657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33acf22e716d76b46aa215be86d402b346c30583ac243161d878e673e2e55f3b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824ed8f5821cf4dcfd3bd99d56b7aa9c5eae5312be30686e88b07808d8c0cdc`  
		Last Modified: Tue, 17 Aug 2021 09:40:52 GMT  
		Size: 49.6 MB (49574573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e758f7a7e0da372de0f1611d7468674233f2987fcd71261075cd789d9e68c376`  
		Last Modified: Tue, 17 Aug 2021 09:42:43 GMT  
		Size: 171.3 MB (171327019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d9fa7ab94996efb32eaab7c8363d856078c4236005a258221b1bb956b0e35553
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278336342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfdda06dd06bb9126a7313b6e12f595b0f2c2e92f8f8999e5814c02e077a6e2c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:48 GMT
ADD file:335c38ff88b5e08b7ac0de8108215837affe91919978ea400e32196f7601b991 in / 
# Tue, 17 Aug 2021 02:13:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:21:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:21:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:22:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:24:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:978724337d55541757ceda31b51cc0dcbdb70d7d5bc63ebcc0aaceab90aa8acf`  
		Last Modified: Tue, 17 Aug 2021 02:30:16 GMT  
		Size: 45.9 MB (45917818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f0b0065a7e3b0a78d7b7e0691152e1474bfd7bc177bb8a2383c8b14b0c9dab`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 7.1 MB (7124489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6ed7bdd30c985279190b4c2a50b4257a03d5706663e8ec8c766f425014c39c`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 9.3 MB (9343798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54854fad8c30eacd3b5b5484549685dbf93460ecf31ea30835ec3aa3e3cfa49`  
		Last Modified: Tue, 17 Aug 2021 15:41:54 GMT  
		Size: 47.4 MB (47357324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c39822934191a8ed942f48d7d0005d1f051e099931a35baf8688726dc3ec632`  
		Last Modified: Tue, 17 Aug 2021 15:43:40 GMT  
		Size: 168.6 MB (168592913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:91996eae68b6eaf9ef2e8da9977f75957df26e91cce6e7ee57512071962c18bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (303045063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904acaa22971fd0fb987aab79cd5d55ad3052d4f940c4dd7d20511e547513a04`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:54:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:54:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0eab8670a99c796e5d1a5613581de4cf56c052c3ff83593ca70565c7c45683`  
		Last Modified: Tue, 17 Aug 2021 08:02:43 GMT  
		Size: 52.2 MB (52167867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510a11c58681da817539e7455b4ea1dec3b803bd34d93a7d261508fcdb4a6f74`  
		Last Modified: Tue, 17 Aug 2021 08:03:20 GMT  
		Size: 184.0 MB (183975288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8a5d000723d1d7e1dde9372d4466c86060fcc7d0a75d5f77505d838505df5697
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321916207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08baf0563c53b9fbc69d9dd212ee8b008f0c9955f963977ffa5509d397fd67df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:51 GMT
ADD file:98d4857c154cb75c011be69c57275c4a1304d441ddb03fe8388342bc0e2a9689 in / 
# Tue, 17 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:59:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:00:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:01:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17ec3e1e9f7b10e3075002c6dd4297be244b5386198d7a417a9d22302080b6f7`  
		Last Modified: Tue, 17 Aug 2021 01:50:25 GMT  
		Size: 51.2 MB (51207344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54b2adab88b38d8137579946b8da20be9bdb174381dc3e02340d5a786c41ac`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 8.0 MB (7998779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea932812b2c3a1292981a835c426875eb75f95cb82d925268ceca609a2f23315`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 10.3 MB (10340001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51f590108a6abf5786a02b71f872bd665de64cbee36555dd51fcf8df17b74a`  
		Last Modified: Tue, 17 Aug 2021 02:10:05 GMT  
		Size: 53.4 MB (53437804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ed94c24c31fc57f522ffc87f8d4d7bea22c7b1c41b056fcf497994d3568d1`  
		Last Modified: Tue, 17 Aug 2021 02:11:15 GMT  
		Size: 198.9 MB (198932279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2b0e48869fbf3f77ec60d613fe4f2451863692d821ca110ac445c46ef2314f9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297104024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b277e856e0dbfb86d7a235699dce3f54b041c07fa42b95e67bcbf8c9464bb75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:02 GMT
ADD file:a8c2c0d0623fc8523c52507da1bb3e33e40086f0387a0ec12df9480599a1799e in / 
# Tue, 17 Aug 2021 01:12:03 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:45:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:46:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:49:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e36b8e9dc7a490231e9a4577c7c920ea6252b0b035d31b18e0115e0743d5ca97`  
		Last Modified: Tue, 17 Aug 2021 01:21:04 GMT  
		Size: 49.1 MB (49079655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf1e19e8c366bbeed533597a718657c71c55ace29aedda5015330b7811605a`  
		Last Modified: Tue, 17 Aug 2021 20:57:20 GMT  
		Size: 7.3 MB (7252790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab553f775efe1ebe386c27726c3f1723f48e32fb8865b49e910c181e3cfab788`  
		Last Modified: Tue, 17 Aug 2021 20:57:21 GMT  
		Size: 10.0 MB (10016441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28044c83fd33e51894666e65c54e1691250d8298a8687b14d7a079df5afd69c`  
		Last Modified: Tue, 17 Aug 2021 20:58:09 GMT  
		Size: 50.8 MB (50843141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a254e959b3e0b79e2ecebd56f2318cd2299b7983a3afc46b2ccf4c7400d3cb`  
		Last Modified: Tue, 17 Aug 2021 21:00:16 GMT  
		Size: 179.9 MB (179911997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2e1857e66330a9c88bcd4c611ab4957d2748a322519d057ab23fe1bc854c6d81
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333925560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50fc7bc98fca33962c2d053a05d960cd2f3e563582e2a3ca49919b18a46d8b19`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:35 GMT
ADD file:cd847762c4d814b1302366ad14c10c4fc83be52d52ede8336744b1f0bf988112 in / 
# Tue, 17 Aug 2021 01:33:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:22:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4b39f6d7e8772c5450fb8b799577a194b8bdd1a2935d732d4836f0713e6518a`  
		Last Modified: Tue, 17 Aug 2021 01:47:16 GMT  
		Size: 54.2 MB (54182973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b2ff2b66aeb977708310cb04f7b6110efbc73ff8a538b6f003df129f2fb0f3`  
		Last Modified: Tue, 17 Aug 2021 16:04:35 GMT  
		Size: 8.3 MB (8272123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edeeefbd9326b5c8dbf6c5b3a60d602c1e0f2d0af22dc2cfc28842351dc6b95`  
		Last Modified: Tue, 17 Aug 2021 16:04:33 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350768736925f68aafac882b13a3e7593640560819c88b60d0f566ec1781de0b`  
		Last Modified: Tue, 17 Aug 2021 16:05:58 GMT  
		Size: 57.5 MB (57457638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59be0c0011a56689a0699ad31ad26e9a7da01ae88b4764884cf262f2cb31c28`  
		Last Modified: Tue, 17 Aug 2021 16:10:04 GMT  
		Size: 203.3 MB (203284992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:80d92f21c111dc9c416e40575b17808f5f13edb19cd80fb284baf097ac00d767
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294546507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1088c269f2788cf285d144ee0886437b648e27560a62606824856ada90dc66a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:25 GMT
ADD file:0443e797578f02bf4a9404844d217d992a5dafb634ae3a03ed9e181313f78d4c in / 
# Tue, 17 Aug 2021 01:49:33 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:34:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b14cfca9681354c01ba0c52718b98b1783ccc6a88170ff1b5d491a86f389ccee`  
		Last Modified: Tue, 17 Aug 2021 01:57:51 GMT  
		Size: 49.0 MB (49004330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398cc2dd69156863e1a916460d85ea681c1fea50e25611f3fa0bf634ecda0a97`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 7.4 MB (7400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc3c2fc42de3b04bcd5e6a2d4b4004ba2295b0580a1ae1d2e01ea1d65200a0`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 9.9 MB (9883198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723dbf1359b8c022bdec44c42d0fda155c8ca45da7152e885954f7c17d70c05c`  
		Last Modified: Tue, 17 Aug 2021 07:44:31 GMT  
		Size: 51.4 MB (51380299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0234edac00c22e8e9fac61c99ce359d2968b0d2eed6a0bc430c1312fcb980c`  
		Last Modified: Tue, 17 Aug 2021 07:45:00 GMT  
		Size: 176.9 MB (176877890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:362d5c697af8f484f7ae13c85deea3cab6b00f9ba746c57100d923e9f77084ad
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

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:497fe7d6785c18b508d94d41decc6f8f7747217ed3fa71e5fba86a1cf85c3739
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68266489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1136d707940b8ca41c39cf5bf8ef4e5c65cec971cceb3160138971badc108967`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4099a935a96edef1e9378de34e314d07fb3aea1b7205774055a1fa44a3819f4`  
		Last Modified: Tue, 17 Aug 2021 09:30:37 GMT  
		Size: 7.8 MB (7833079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e2960d83651b1494b4da6c97686e79cc760aa90a75948eed56786726f86928`  
		Last Modified: Tue, 17 Aug 2021 09:30:38 GMT  
		Size: 10.0 MB (9997209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:da5b8eb187b6b53bf095f163c217b3eecc10198c815c9a0c1f26628bb8c26334
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65217997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d44190dbb507ef58f05cf66da856e9c1aa332e05aa3bf37ae7ad4602e90a3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:56:17 GMT
ADD file:784cabdb8b1e35aff6dcfa7acb3c6da5d76ee575188460537a190bab6ef49655 in / 
# Tue, 17 Aug 2021 01:56:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ce5dcedb6ed028586f61d36e8067567349cb049735f9b1fbeb748a005636b9d9`  
		Last Modified: Tue, 17 Aug 2021 02:11:57 GMT  
		Size: 48.2 MB (48153800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1036818934ab73ac9c3e731432ae2c2c576a342f8ac27c0de1654407945f2b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 7.4 MB (7376657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33acf22e716d76b46aa215be86d402b346c30583ac243161d878e673e2e55f3b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:db039b572fd5a9af2d28931774fccafc924168089530272c19bbe8bbc5e2dd91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62386105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d071eaa7bc77231a9601b9803544237251f24da0051d72372ba6d6a08ddd550`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:48 GMT
ADD file:335c38ff88b5e08b7ac0de8108215837affe91919978ea400e32196f7601b991 in / 
# Tue, 17 Aug 2021 02:13:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:21:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:21:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:978724337d55541757ceda31b51cc0dcbdb70d7d5bc63ebcc0aaceab90aa8acf`  
		Last Modified: Tue, 17 Aug 2021 02:30:16 GMT  
		Size: 45.9 MB (45917818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f0b0065a7e3b0a78d7b7e0691152e1474bfd7bc177bb8a2383c8b14b0c9dab`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 7.1 MB (7124489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6ed7bdd30c985279190b4c2a50b4257a03d5706663e8ec8c766f425014c39c`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 9.3 MB (9343798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:32d342f1ccb22c5aab6bbac3708e207a49ee70e3d283dea19a81b8abdfac1ea0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66901908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12cc124d374de8b5eca7edb432d729a09f24f12ddb3bd30040f8f781c80bbffd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0f44fa0a78c1b024b7b57c7dfdaf67fd1d83e6a47c25ba6951db73d1b87367fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69546124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca2a445c5ff6e65a07e933e73aa21587acb1ac2b1a7d72c2c7f2a19b28473ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:51 GMT
ADD file:98d4857c154cb75c011be69c57275c4a1304d441ddb03fe8388342bc0e2a9689 in / 
# Tue, 17 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:59:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:17ec3e1e9f7b10e3075002c6dd4297be244b5386198d7a417a9d22302080b6f7`  
		Last Modified: Tue, 17 Aug 2021 01:50:25 GMT  
		Size: 51.2 MB (51207344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54b2adab88b38d8137579946b8da20be9bdb174381dc3e02340d5a786c41ac`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 8.0 MB (7998779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea932812b2c3a1292981a835c426875eb75f95cb82d925268ceca609a2f23315`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 10.3 MB (10340001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4c8071c6e8cb4d846d227e025984b053fad4a3dd2e703d7125cc81f7db73838d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66348886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f297322b38395246036055fe978a89876b94ff9397851939a20e4d360bc2243`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:02 GMT
ADD file:a8c2c0d0623fc8523c52507da1bb3e33e40086f0387a0ec12df9480599a1799e in / 
# Tue, 17 Aug 2021 01:12:03 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:45:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e36b8e9dc7a490231e9a4577c7c920ea6252b0b035d31b18e0115e0743d5ca97`  
		Last Modified: Tue, 17 Aug 2021 01:21:04 GMT  
		Size: 49.1 MB (49079655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf1e19e8c366bbeed533597a718657c71c55ace29aedda5015330b7811605a`  
		Last Modified: Tue, 17 Aug 2021 20:57:20 GMT  
		Size: 7.3 MB (7252790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab553f775efe1ebe386c27726c3f1723f48e32fb8865b49e910c181e3cfab788`  
		Last Modified: Tue, 17 Aug 2021 20:57:21 GMT  
		Size: 10.0 MB (10016441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f0132bbc40fe6f19e70d6ed09d2468ac0f2aa7e9775e7513f35beb3ca3aa75c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73182930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c52f522da9b38f0d62f5476be6f4360207f575044814019f3f07de43154563d9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:35 GMT
ADD file:cd847762c4d814b1302366ad14c10c4fc83be52d52ede8336744b1f0bf988112 in / 
# Tue, 17 Aug 2021 01:33:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a4b39f6d7e8772c5450fb8b799577a194b8bdd1a2935d732d4836f0713e6518a`  
		Last Modified: Tue, 17 Aug 2021 01:47:16 GMT  
		Size: 54.2 MB (54182973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b2ff2b66aeb977708310cb04f7b6110efbc73ff8a538b6f003df129f2fb0f3`  
		Last Modified: Tue, 17 Aug 2021 16:04:35 GMT  
		Size: 8.3 MB (8272123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edeeefbd9326b5c8dbf6c5b3a60d602c1e0f2d0af22dc2cfc28842351dc6b95`  
		Last Modified: Tue, 17 Aug 2021 16:04:33 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d6f10cb7018413f6e061cee9cf7e810d23904e165779fdf4b8216569577e4d1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66288318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d2ff06a71ed154e37eba7dfe06067e8775954cd4c0746db42a3e636ad810039`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:25 GMT
ADD file:0443e797578f02bf4a9404844d217d992a5dafb634ae3a03ed9e181313f78d4c in / 
# Tue, 17 Aug 2021 01:49:33 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:34:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b14cfca9681354c01ba0c52718b98b1783ccc6a88170ff1b5d491a86f389ccee`  
		Last Modified: Tue, 17 Aug 2021 01:57:51 GMT  
		Size: 49.0 MB (49004330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398cc2dd69156863e1a916460d85ea681c1fea50e25611f3fa0bf634ecda0a97`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 7.4 MB (7400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc3c2fc42de3b04bcd5e6a2d4b4004ba2295b0580a1ae1d2e01ea1d65200a0`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 9.9 MB (9883198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:222c0ca0bba33fec8b59689bc4c25b5213eb0757a28d7f8ef3fe6572327ae4e6
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

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5f0efe6cb5460b8e4c226ac7b8800efd073be90c013db2cecc723fafe67f5a94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120107531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba2bc828a3e5dbc792e59263153ca7d43e8eaea225ac12335765983dae56b210`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:21:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4099a935a96edef1e9378de34e314d07fb3aea1b7205774055a1fa44a3819f4`  
		Last Modified: Tue, 17 Aug 2021 09:30:37 GMT  
		Size: 7.8 MB (7833079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e2960d83651b1494b4da6c97686e79cc760aa90a75948eed56786726f86928`  
		Last Modified: Tue, 17 Aug 2021 09:30:38 GMT  
		Size: 10.0 MB (9997209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffd4e6385927b79e4d4daa2d00523e766502eed6dd1934e1eda583d348abd8b`  
		Last Modified: Tue, 17 Aug 2021 09:30:58 GMT  
		Size: 51.8 MB (51841042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:31841421c87e0d139b3dd546eef3887a00ac38e6a3cd6021e1cb94390646347c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114792570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f63086e65411b3f81d2b2d5de7844c8af328a16f5177a6a77beece3cdee972b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:56:17 GMT
ADD file:784cabdb8b1e35aff6dcfa7acb3c6da5d76ee575188460537a190bab6ef49655 in / 
# Tue, 17 Aug 2021 01:56:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce5dcedb6ed028586f61d36e8067567349cb049735f9b1fbeb748a005636b9d9`  
		Last Modified: Tue, 17 Aug 2021 02:11:57 GMT  
		Size: 48.2 MB (48153800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1036818934ab73ac9c3e731432ae2c2c576a342f8ac27c0de1654407945f2b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 7.4 MB (7376657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33acf22e716d76b46aa215be86d402b346c30583ac243161d878e673e2e55f3b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824ed8f5821cf4dcfd3bd99d56b7aa9c5eae5312be30686e88b07808d8c0cdc`  
		Last Modified: Tue, 17 Aug 2021 09:40:52 GMT  
		Size: 49.6 MB (49574573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:be696c95b2e45c5098978d1443ea5388283dc86a32693296f1ccde7af6276cfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109743429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae06312e8b3ee525f6a2780c2ca3676bbfb804f21eb366f50128fa9ba2a2d0b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:48 GMT
ADD file:335c38ff88b5e08b7ac0de8108215837affe91919978ea400e32196f7601b991 in / 
# Tue, 17 Aug 2021 02:13:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:21:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:21:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:22:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:978724337d55541757ceda31b51cc0dcbdb70d7d5bc63ebcc0aaceab90aa8acf`  
		Last Modified: Tue, 17 Aug 2021 02:30:16 GMT  
		Size: 45.9 MB (45917818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f0b0065a7e3b0a78d7b7e0691152e1474bfd7bc177bb8a2383c8b14b0c9dab`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 7.1 MB (7124489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6ed7bdd30c985279190b4c2a50b4257a03d5706663e8ec8c766f425014c39c`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 9.3 MB (9343798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54854fad8c30eacd3b5b5484549685dbf93460ecf31ea30835ec3aa3e3cfa49`  
		Last Modified: Tue, 17 Aug 2021 15:41:54 GMT  
		Size: 47.4 MB (47357324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f205f4ce2ab7ca9500880d60a78bdbfc28690cb36152742749166702d5c614ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119069775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be45f7fa2e70d1185fbc4913782c90d5e841037e8a39892d75443ec7e2284882`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:54:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0eab8670a99c796e5d1a5613581de4cf56c052c3ff83593ca70565c7c45683`  
		Last Modified: Tue, 17 Aug 2021 08:02:43 GMT  
		Size: 52.2 MB (52167867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b93315610788a1790a30e09d35f401e86e379b24ac307d2f5034f6563b506d83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122983928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae3516212cddb6fe0af927d0804199bcd75b7f211eeca85b15c17500ea4bdeb2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:51 GMT
ADD file:98d4857c154cb75c011be69c57275c4a1304d441ddb03fe8388342bc0e2a9689 in / 
# Tue, 17 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:59:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:00:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17ec3e1e9f7b10e3075002c6dd4297be244b5386198d7a417a9d22302080b6f7`  
		Last Modified: Tue, 17 Aug 2021 01:50:25 GMT  
		Size: 51.2 MB (51207344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54b2adab88b38d8137579946b8da20be9bdb174381dc3e02340d5a786c41ac`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 8.0 MB (7998779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea932812b2c3a1292981a835c426875eb75f95cb82d925268ceca609a2f23315`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 10.3 MB (10340001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51f590108a6abf5786a02b71f872bd665de64cbee36555dd51fcf8df17b74a`  
		Last Modified: Tue, 17 Aug 2021 02:10:05 GMT  
		Size: 53.4 MB (53437804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:cdd5f0a255e2b203fda9f9da748b29d1cbd1c436a3fab250c00d98a766f0811a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117192027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b8420dbc34754e42504603d5492904047f7b20448d055a240048862336a2e9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:02 GMT
ADD file:a8c2c0d0623fc8523c52507da1bb3e33e40086f0387a0ec12df9480599a1799e in / 
# Tue, 17 Aug 2021 01:12:03 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:45:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:46:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e36b8e9dc7a490231e9a4577c7c920ea6252b0b035d31b18e0115e0743d5ca97`  
		Last Modified: Tue, 17 Aug 2021 01:21:04 GMT  
		Size: 49.1 MB (49079655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf1e19e8c366bbeed533597a718657c71c55ace29aedda5015330b7811605a`  
		Last Modified: Tue, 17 Aug 2021 20:57:20 GMT  
		Size: 7.3 MB (7252790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab553f775efe1ebe386c27726c3f1723f48e32fb8865b49e910c181e3cfab788`  
		Last Modified: Tue, 17 Aug 2021 20:57:21 GMT  
		Size: 10.0 MB (10016441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28044c83fd33e51894666e65c54e1691250d8298a8687b14d7a079df5afd69c`  
		Last Modified: Tue, 17 Aug 2021 20:58:09 GMT  
		Size: 50.8 MB (50843141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:986a9620f9dde7ab2ba404bf95257d683551ad4cdb24c380d99d6742723a2faf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130640568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60fea57c4f4e9377c6d9ebfba03667f4f5c98dbf30cd02020d8ed9da9e950dd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:35 GMT
ADD file:cd847762c4d814b1302366ad14c10c4fc83be52d52ede8336744b1f0bf988112 in / 
# Tue, 17 Aug 2021 01:33:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4b39f6d7e8772c5450fb8b799577a194b8bdd1a2935d732d4836f0713e6518a`  
		Last Modified: Tue, 17 Aug 2021 01:47:16 GMT  
		Size: 54.2 MB (54182973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b2ff2b66aeb977708310cb04f7b6110efbc73ff8a538b6f003df129f2fb0f3`  
		Last Modified: Tue, 17 Aug 2021 16:04:35 GMT  
		Size: 8.3 MB (8272123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edeeefbd9326b5c8dbf6c5b3a60d602c1e0f2d0af22dc2cfc28842351dc6b95`  
		Last Modified: Tue, 17 Aug 2021 16:04:33 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350768736925f68aafac882b13a3e7593640560819c88b60d0f566ec1781de0b`  
		Last Modified: Tue, 17 Aug 2021 16:05:58 GMT  
		Size: 57.5 MB (57457638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bd5e99eae2c75ab38c62bb8c506df389296ceef68663a6cf77c3c9574b582396
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117668617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd52a53fd4d502b1e8e07b671196e14bac22b39fc9ff3c5f64b4092d60e97af6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:25 GMT
ADD file:0443e797578f02bf4a9404844d217d992a5dafb634ae3a03ed9e181313f78d4c in / 
# Tue, 17 Aug 2021 01:49:33 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:34:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b14cfca9681354c01ba0c52718b98b1783ccc6a88170ff1b5d491a86f389ccee`  
		Last Modified: Tue, 17 Aug 2021 01:57:51 GMT  
		Size: 49.0 MB (49004330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398cc2dd69156863e1a916460d85ea681c1fea50e25611f3fa0bf634ecda0a97`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 7.4 MB (7400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc3c2fc42de3b04bcd5e6a2d4b4004ba2295b0580a1ae1d2e01ea1d65200a0`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 9.9 MB (9883198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723dbf1359b8c022bdec44c42d0fda155c8ca45da7152e885954f7c17d70c05c`  
		Last Modified: Tue, 17 Aug 2021 07:44:31 GMT  
		Size: 51.4 MB (51380299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:fdd2452507132b7a4c6b432c32e159f15d955afa4258e5b8f64b7fdc7add487f
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

### `buildpack-deps:curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f2aebefdccca99d265c8e84738ee9f99c36f4212ca051d43b4683798dfb42636
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70940116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6fe7405525d60b20905a08baa979b62312fdb03b9a48e235baebfc59977f2c2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf565088aae3ef2159885f29853bce88eb16082b0c98fcacd08fc9008c84b9`  
		Last Modified: Tue, 17 Aug 2021 09:29:09 GMT  
		Size: 5.2 MB (5153283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c0dd0dc0d3d367cc5b85f86d8881afb658e8eb341a86daf3835c2f14159ac`  
		Last Modified: Tue, 17 Aug 2021 09:29:10 GMT  
		Size: 10.9 MB (10871829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b2e1e86e8147e79ba83867e74aa1a9fa3b677f764ef0a9d7e3cae46c5ad2669d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68086892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c4086386b6b216789ae1d7d834ccfd24e3cae7f8d6d9f2d9dfa493924d3cc3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:18:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b0b6b82f848e8ef423a421d5d46194f7787ebf23e3dcc69fb177eb4dc49f6`  
		Last Modified: Tue, 17 Aug 2021 09:36:54 GMT  
		Size: 5.1 MB (5063684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02ecba39f2b03f1bc47ed6ba17c15a62b11e7eb2ae7397ba374851a864efc67`  
		Last Modified: Tue, 17 Aug 2021 09:36:55 GMT  
		Size: 10.6 MB (10570968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:65059ed8ae5f1dcdde3da0bb274969b7cca178755ccd40eee90ae54fde9e89fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65257911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c4021355832ed254e558058a0774730787867c0d43269189b5abea64f2fe0b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:12:37 GMT
ADD file:579ac9b41923db9165f333faac1330f2924a14f90cab7605ffd66c1815249adf in / 
# Tue, 17 Aug 2021 02:12:38 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1ce31b8c318c8eac9eba15cdf329f397a64952ab575a09c167fc9ddc5a991a98`  
		Last Modified: Tue, 17 Aug 2021 02:28:44 GMT  
		Size: 50.1 MB (50118546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5a38f951962ad43cfef6137e6638004e3a3f066bb26e2c3b52489258a4b5c`  
		Last Modified: Tue, 17 Aug 2021 15:38:06 GMT  
		Size: 4.9 MB (4922570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a545de7dcb8f9fe8fd65b3b1f104abbb20cee600bc8602beef63ccc4f6259`  
		Last Modified: Tue, 17 Aug 2021 15:38:08 GMT  
		Size: 10.2 MB (10216795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fe66fbc885d81fdafbe18713a6165c8028b9ed9939b65497ab53bdf98e963213
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69616272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48afe04239a66261d25a64f298c4fa2467895f8861bcf70bcc11a0248523fb5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:52:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:52:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495d06e79f81fe42766bacea59684f27db9d24960b6dd7efeea81f48820d0f6`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 5.1 MB (5142588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd18a2d3ce3a400515ed7a845aeb9d8cd17b023f1efe77ff81292bd63addcc0`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 10.9 MB (10872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e593b0b7e666a4ee388aec91360e9d8414ec6b6846bab3c97d2fad8f754445d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72456123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f08f2eeb7d00459ae8f10b008928c02a6c5ad7cbd65e4e0ab0ead6da5ba4b05c`
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

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5617c8a692ae2f2d66e61c9353dd8f51a5584d8d3bc9247c10af1c8ed8b9fa49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69155509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efea973f65ee025f05845863859e9962cff13e166db36866230ec2619834163e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d42212351d464cda967a0b9462fdbf31cf8b926ec739f94ca92a04924b59b44`  
		Last Modified: Tue, 17 Aug 2021 20:53:57 GMT  
		Size: 5.1 MB (5114876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f443b77bd62cad6049ac9b935c37714988629b9b90804c902ebf5d94db0947`  
		Last Modified: Tue, 17 Aug 2021 20:53:59 GMT  
		Size: 10.9 MB (10873298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7c55dd439b7bc0da37bc1d85c237a140966ff47444714b599ceb42724bb68232
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75844024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c6a017b4350c90fd80678152fdf7e17a772a4b8585ddad57bdb2cb34e56a59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f9b82c933b317ed127f45e6f56d6d7508514459e0ef09073b467d3dd8425e`  
		Last Modified: Tue, 17 Aug 2021 15:58:19 GMT  
		Size: 5.4 MB (5401864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a6114ee4fe00702ca86cd44f229643d9324c4b202ed6583f35d2eca848a4a`  
		Last Modified: Tue, 17 Aug 2021 15:58:18 GMT  
		Size: 11.6 MB (11626128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:86da00cec8807a6fca2c5dc68ebe2887651da5b291cee956ee1b61e0a2ec85d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69092635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1b1429c9e37360be6c7c7fb3e2850f6c59962e4669641fdc1cbb2dfe99a8241`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:32:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20bd918649e02578e4e6f19a2c873dbcc6da7009f7b4ee3088a3e2f594fe6e`  
		Last Modified: Tue, 17 Aug 2021 07:43:16 GMT  
		Size: 5.1 MB (5137099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e43baff5e6307dfe51df170140aa3c7c4b7a4cb3fb03b3a2255a8038c9542`  
		Last Modified: Tue, 17 Aug 2021 07:43:17 GMT  
		Size: 10.8 MB (10761504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:ac5935233587846ba1b87bf3c95e7c055858e4bf5763a246e4abd27292db881f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4b7fe67099dceda7bfcb13dd7aa48258e2b6640b854349481f4d68e27a03c873
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241800863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c060b0cd98ed5dc24171eb227d217cbcc64a9c73a25d7c29cfb9092919ff6fb0`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:45:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:46:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:49:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844d0dd6bf6aa5959f603bad64a331fca5cda171d344450ca89c77e67410ac3`  
		Last Modified: Mon, 26 Jul 2021 22:11:07 GMT  
		Size: 7.8 MB (7769926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e2a2dd7363ebee0e3b7e3d44204409298c305ea2a5f38345f68c7b769033b`  
		Last Modified: Mon, 26 Jul 2021 22:11:06 GMT  
		Size: 3.6 MB (3624037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaacada9b3485ee466ed24e835156869e37b446a2fe7a324d2f9349b81b4d0e`  
		Last Modified: Mon, 26 Jul 2021 22:11:30 GMT  
		Size: 60.7 MB (60718930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b6cb30d1604a69cf710ee8afbc920594fe5ae63e17de53cf47ded9036b7cc2`  
		Last Modified: Mon, 26 Jul 2021 22:12:06 GMT  
		Size: 141.1 MB (141120026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:efc1ca89c89167e69a4f61948d72c6f9c84c5d329b79367248d9b4688c4b65bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207232409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486b525c7c1498a7b327ecca4c676e8ccdb6f6b1b6c6533b3f87511fc1c31e83`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:18:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:19:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:21:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0761e0b1ad0205162c66dfa83bf91ca0344921eca2bdd1d64b0970a5c75f0c`  
		Last Modified: Tue, 27 Jul 2021 01:42:27 GMT  
		Size: 6.8 MB (6767075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c226da21dd821a4b4f19689b2131f6e34d29095f42b4046f2eb48cf954e0076`  
		Last Modified: Tue, 27 Jul 2021 01:42:24 GMT  
		Size: 3.1 MB (3103731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305b0cc7ca4c4e47790a52a092d4cc7774810f9fee0f20387a45833bc8740475`  
		Last Modified: Tue, 27 Jul 2021 01:43:20 GMT  
		Size: 55.5 MB (55454116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ed4d0e81d3335f5c0ef3c7022d19556dbfe4f0b5fd02ab59f0b927a976f597`  
		Last Modified: Tue, 27 Jul 2021 01:44:43 GMT  
		Size: 117.8 MB (117843249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e3839ead7897c13b52908329bd10baca50cb1ef66360966dadfa8b39f983bea4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231941624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d0fe256db32a56a7dc4ec312196c1b98ea8f189e4cf3089cdf49195453cd42`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:10:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:10:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:10:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b8ef0ef6610d6e720afe76a3df03bf2afed7f16cc8b12dab2279c75b1c408`  
		Last Modified: Tue, 31 Aug 2021 02:19:41 GMT  
		Size: 7.6 MB (7636852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a226690073506846a68b797c6c96615eec776aefa661831f4abff3715172704`  
		Last Modified: Tue, 31 Aug 2021 02:19:40 GMT  
		Size: 3.6 MB (3600358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d5c6943027b3d6294ec2bbad85003c7584f70a77a2b64b363ee36bbf30920b`  
		Last Modified: Tue, 31 Aug 2021 02:20:04 GMT  
		Size: 60.8 MB (60766232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93e2b0312aef41acc2f08ed835204fdfe90ab144ae3a37f8a4d4b1769a51f2d`  
		Last Modified: Tue, 31 Aug 2021 02:20:37 GMT  
		Size: 132.8 MB (132765083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:168c59e783ee4016bd0eb2e7f29b4f70fe3a05f40aa246546db37b649e7ceff1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.4 MB (265373323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d9fdf0ea0302149f5068e3e1092e7eba8267bc0a59dad98d5aeb03424a1c4f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:09:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:11:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:20:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f198532bfc08536f5ad0c1f1242b55d34d7aac9ce9dc059a6109c2d7e20b7`  
		Last Modified: Tue, 27 Jul 2021 04:23:58 GMT  
		Size: 8.7 MB (8722787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8f157ddc9f96bd79c6823da12b4c54366d23b79691f3d8f39665ef321ff86e`  
		Last Modified: Tue, 27 Jul 2021 04:23:57 GMT  
		Size: 4.5 MB (4456512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a51a75aca451f998a1dcf27f7a8ece4fb2c2aaf4f7a09896e4664873136d52d`  
		Last Modified: Tue, 27 Jul 2021 04:24:25 GMT  
		Size: 69.4 MB (69386343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cad91e4250099e76cca3f45f2a9042659f5e576e115493fdefb69344c5bfa74`  
		Last Modified: Tue, 27 Jul 2021 04:25:07 GMT  
		Size: 149.5 MB (149517254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:faffd9346d55fa6213130fb0c9a38b4be7304ab9e3c4356c535890f3cf5aefe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222647738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa0dac2fbda7f28429e6b30a06ba7fa724f82ebb53389e9a32ecdff324cc0c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748dba3041b2bd31a240176639b763492a369d59b429da56c854b823820b27b3`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 7.4 MB (7428812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e0c13c39c1426302723ee65c5c58538ee64cf9d25b9629ac690cedd2a7169b`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 3.5 MB (3542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80abe2f24b0566481303d246a8e9996957224b079b7ff282fae87f647409e82c`  
		Last Modified: Tue, 31 Aug 2021 02:46:16 GMT  
		Size: 60.0 MB (60019295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce138a57132ff0b82fe8f962631a86073cbae19bfe4574d55a0d7e6e908d5210`  
		Last Modified: Tue, 31 Aug 2021 02:46:43 GMT  
		Size: 124.5 MB (124530018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:8e7cd12c1a76ba2c6906fc2bf3995dbffb57089f7bfcdead09c0ef7acdf99d90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:focal-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8ad7989339bd5853dee1b4694129b35e8f3da4f9bd367566525e02f4bc25430c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39961907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c7b26ba20fb907bc6e40ebdec0384394f1a12802265f68c178e8f2919a646a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:45:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844d0dd6bf6aa5959f603bad64a331fca5cda171d344450ca89c77e67410ac3`  
		Last Modified: Mon, 26 Jul 2021 22:11:07 GMT  
		Size: 7.8 MB (7769926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e2a2dd7363ebee0e3b7e3d44204409298c305ea2a5f38345f68c7b769033b`  
		Last Modified: Mon, 26 Jul 2021 22:11:06 GMT  
		Size: 3.6 MB (3624037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4d6589f264d3d82306ab179d8ff852a670346027a7b62190c0babd4b8d34a958
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33935044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02443af7132a39831ae2d9b9d585c88205154e162e5bbf922e0c3084d7be59d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:18:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0761e0b1ad0205162c66dfa83bf91ca0344921eca2bdd1d64b0970a5c75f0c`  
		Last Modified: Tue, 27 Jul 2021 01:42:27 GMT  
		Size: 6.8 MB (6767075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c226da21dd821a4b4f19689b2131f6e34d29095f42b4046f2eb48cf954e0076`  
		Last Modified: Tue, 27 Jul 2021 01:42:24 GMT  
		Size: 3.1 MB (3103731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:de885f7309d9ab073f94e98a098a4c7c899de49d976b4e1f5a082b722b954785
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38410309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67275e237ee034fba2cbf875eb175b0f631d2b6852b862ac1d3569199a21e87`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:10:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:10:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b8ef0ef6610d6e720afe76a3df03bf2afed7f16cc8b12dab2279c75b1c408`  
		Last Modified: Tue, 31 Aug 2021 02:19:41 GMT  
		Size: 7.6 MB (7636852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a226690073506846a68b797c6c96615eec776aefa661831f4abff3715172704`  
		Last Modified: Tue, 31 Aug 2021 02:19:40 GMT  
		Size: 3.6 MB (3600358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e09bd25d95c7b0f0855b35269f866c1505a2f3b7531a2dc7239ce7bb47f9f068
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46469726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b2ecb47ee2780a093931cf3725b04c02ec822c6aed0eb4a7471d2df82d45663`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:09:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f198532bfc08536f5ad0c1f1242b55d34d7aac9ce9dc059a6109c2d7e20b7`  
		Last Modified: Tue, 27 Jul 2021 04:23:58 GMT  
		Size: 8.7 MB (8722787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8f157ddc9f96bd79c6823da12b4c54366d23b79691f3d8f39665ef321ff86e`  
		Last Modified: Tue, 27 Jul 2021 04:23:57 GMT  
		Size: 4.5 MB (4456512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c5d73e180ba8a80aa23037f5d711ff640e8c4ec80d23ffcbd25059cba22dc138
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34121380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d72b46ed7de7fd72c1870742a2ccea279cef0774ff6b94a241b981033ac58b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:15:32 GMT
ADD file:9492642ba0098006a011dce4d8ce4aa68e0920ff935c864dbcb82561d98740a5 in / 
# Tue, 31 Aug 2021 01:15:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:01:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e7b9bc251112be9d180cbc3a028c58259667feb9a3641efdfd3e35108b2f0c59`  
		Last Modified: Tue, 31 Aug 2021 01:30:41 GMT  
		Size: 24.2 MB (24229065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284ff38f39508e263a7b2fc045b5cea3b705b539db48287b68e6dc16cfa3352`  
		Last Modified: Tue, 31 Aug 2021 02:43:02 GMT  
		Size: 6.7 MB (6747870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4356ee79579dda81c7c5bbf4631f471e2e2f99d800cc4e172d3758e96b2c3136`  
		Last Modified: Tue, 31 Aug 2021 02:42:57 GMT  
		Size: 3.1 MB (3144445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:46a0507904553bff68a72de9063f2851dc892f8a862a5ff7b40bb85a037ad564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38098425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e403f7770ab2a035d85b0bc3bb58bb9414238c54cbdb03c5a8f278ec51daae08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748dba3041b2bd31a240176639b763492a369d59b429da56c854b823820b27b3`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 7.4 MB (7428812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e0c13c39c1426302723ee65c5c58538ee64cf9d25b9629ac690cedd2a7169b`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 3.5 MB (3542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:6315aec3d3d0c866c492bd9485e890c45a220196aa07c375cd62d8a3652ba2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a72c32c022e2d1cebdcbefa2fc0810ed6a0c7be253660f8ad5ea9c521ee826b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100680837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b4080e2629487fd86346ead8e8e820c05cb893949b1970238bd1ea0e4cc8ae`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:45:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:46:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844d0dd6bf6aa5959f603bad64a331fca5cda171d344450ca89c77e67410ac3`  
		Last Modified: Mon, 26 Jul 2021 22:11:07 GMT  
		Size: 7.8 MB (7769926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e2a2dd7363ebee0e3b7e3d44204409298c305ea2a5f38345f68c7b769033b`  
		Last Modified: Mon, 26 Jul 2021 22:11:06 GMT  
		Size: 3.6 MB (3624037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaacada9b3485ee466ed24e835156869e37b446a2fe7a324d2f9349b81b4d0e`  
		Last Modified: Mon, 26 Jul 2021 22:11:30 GMT  
		Size: 60.7 MB (60718930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dee7b6f04c4f83196ef597f3f808046a2dd9027ef167d781f8e63e8863dd65b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89389160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a657cdf3fbed62a72c2fe65d674734ce4b12fbee60d88edce235c8aa2e5a041f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:18:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:19:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0761e0b1ad0205162c66dfa83bf91ca0344921eca2bdd1d64b0970a5c75f0c`  
		Last Modified: Tue, 27 Jul 2021 01:42:27 GMT  
		Size: 6.8 MB (6767075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c226da21dd821a4b4f19689b2131f6e34d29095f42b4046f2eb48cf954e0076`  
		Last Modified: Tue, 27 Jul 2021 01:42:24 GMT  
		Size: 3.1 MB (3103731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305b0cc7ca4c4e47790a52a092d4cc7774810f9fee0f20387a45833bc8740475`  
		Last Modified: Tue, 27 Jul 2021 01:43:20 GMT  
		Size: 55.5 MB (55454116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:19b36271f8dc3c3e32d2efe26aee8d1196a466b9e9daa03445d90e2db344a923
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99176541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88006fc39d950f9ac4bcaac8419a7dcf84b7b72b94bfecdf46a55135c344309f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:10:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:10:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:10:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b8ef0ef6610d6e720afe76a3df03bf2afed7f16cc8b12dab2279c75b1c408`  
		Last Modified: Tue, 31 Aug 2021 02:19:41 GMT  
		Size: 7.6 MB (7636852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a226690073506846a68b797c6c96615eec776aefa661831f4abff3715172704`  
		Last Modified: Tue, 31 Aug 2021 02:19:40 GMT  
		Size: 3.6 MB (3600358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d5c6943027b3d6294ec2bbad85003c7584f70a77a2b64b363ee36bbf30920b`  
		Last Modified: Tue, 31 Aug 2021 02:20:04 GMT  
		Size: 60.8 MB (60766232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3c557088facf8e21f8cb162d5da3b29b0b4d22b7978c6e5330f1abcf4069d200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115856069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81f3ab03184adf9e5ddbbaaf4424797d4ab33a9a2a2acc21b05608758876dbd`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:09:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:11:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f198532bfc08536f5ad0c1f1242b55d34d7aac9ce9dc059a6109c2d7e20b7`  
		Last Modified: Tue, 27 Jul 2021 04:23:58 GMT  
		Size: 8.7 MB (8722787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8f157ddc9f96bd79c6823da12b4c54366d23b79691f3d8f39665ef321ff86e`  
		Last Modified: Tue, 27 Jul 2021 04:23:57 GMT  
		Size: 4.5 MB (4456512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a51a75aca451f998a1dcf27f7a8ece4fb2c2aaf4f7a09896e4664873136d52d`  
		Last Modified: Tue, 27 Jul 2021 04:24:25 GMT  
		Size: 69.4 MB (69386343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:87aef79db204a762d5f40f658ce076db36ab3efc621aa006c6405230ae43653a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98117720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b46e24901559406cd7200c4359b8f96650d7eb96bb6cd9a829fc4b415f1ad1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748dba3041b2bd31a240176639b763492a369d59b429da56c854b823820b27b3`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 7.4 MB (7428812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e0c13c39c1426302723ee65c5c58538ee64cf9d25b9629ac690cedd2a7169b`  
		Last Modified: Tue, 31 Aug 2021 02:45:59 GMT  
		Size: 3.5 MB (3542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80abe2f24b0566481303d246a8e9996957224b079b7ff282fae87f647409e82c`  
		Last Modified: Tue, 31 Aug 2021 02:46:16 GMT  
		Size: 60.0 MB (60019295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:hirsute`

```console
$ docker pull buildpack-deps@sha256:0763bfd59ca79835896bb02e6be807329761ba61f5cb9e6f3292f07d7f7242cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:hirsute` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:91e9acc792f026674dd45f446df640319265b7262c1005bde38528222773d568
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248920500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe66bef49b8843238f7319eab8d5305a356c059489e901289f25b7ea66d4e34c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:55:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:58:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9939f009cb8ebf9ee9b4f6b6f99c0a7ca437c96b046a6345f065cbfcc3dde`  
		Last Modified: Mon, 26 Jul 2021 22:13:53 GMT  
		Size: 43.5 MB (43540366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111c706438d96ec9682736266bade1a4ac6bc3b0a5c98d469c32eddc94a5acbc`  
		Last Modified: Mon, 26 Jul 2021 22:14:30 GMT  
		Size: 164.4 MB (164449942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:786b965a9d6a8aa7384f2db07ae95fa6fb61ce55efe86186d39ffca8a2ed1056
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208923584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f552a257abc3da22a3250ecfc6d93dec61196503231879dba0c59f3b55dea58b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:32 GMT
ADD file:76353e48968f6c84802b150e577cc7fb1bc50985e78e1b499ecd8debfe50d8e5 in / 
# Mon, 26 Jul 2021 22:52:33 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:681a32f1cee4135c0497939e80766271e03a995a197d8293224e8f6bd470bfdd`  
		Last Modified: Mon, 26 Jul 2021 22:57:17 GMT  
		Size: 26.9 MB (26857313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d081ccdbe67f74ab6dab322dc6e8e84a9b56cb1909518f7d199a8fc8936d`  
		Last Modified: Tue, 27 Jul 2021 01:47:35 GMT  
		Size: 4.9 MB (4858897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb191db7ef79ad38fdcde76e18b9267b765696ecf8c500929ef80b649f800`  
		Last Modified: Tue, 27 Jul 2021 01:47:34 GMT  
		Size: 3.1 MB (3138386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b923df82160d2d4eea0012b206b82fae9ca16efd703aacc1069a7bb396b558`  
		Last Modified: Tue, 27 Jul 2021 01:48:15 GMT  
		Size: 40.0 MB (39956131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81972472b3986b3a6bbc0402e59a3d8f113ad7e7069d8918c442e57619255ef6`  
		Last Modified: Tue, 27 Jul 2021 01:49:48 GMT  
		Size: 134.1 MB (134112857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7e5f6e0a00dda48a76aa17bdd9632efad49c2d5e958de1da097c4ba901fcab89
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239569400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd905178021460f6c7f78fa90eceb02ac097094f0e7b4fa0619328671c28a7f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:53 GMT
ADD file:93dcfc1791d96861438a84bfd38f5c0520353febfcc59bde5510c9e85eab2cf8 in / 
# Tue, 31 Aug 2021 01:40:54 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:11:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4fbd1b15195364f20d4b603e346a2b5c64ae93e9de90f5c1bd82a61e92851632`  
		Last Modified: Tue, 31 Aug 2021 01:42:57 GMT  
		Size: 30.2 MB (30162874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54fbc3de08027791a7280c6d2d7f821165cc126fd0e08c6cba66c1d6fc122`  
		Last Modified: Tue, 31 Aug 2021 02:20:51 GMT  
		Size: 5.4 MB (5401544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7180cc8ab79571bbc48658748543060674d12cbbdf7683a598d89f6086677`  
		Last Modified: Tue, 31 Aug 2021 02:20:50 GMT  
		Size: 3.6 MB (3638240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826a66d619e21f0b3656bcd20cb8925d105fc0e444b4a72eb69d81408ecf67ed`  
		Last Modified: Tue, 31 Aug 2021 02:21:10 GMT  
		Size: 43.5 MB (43525534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0590f0535def702f02a4c077e4c3fe732c276f278986df7dc19c8a7c463603`  
		Last Modified: Tue, 31 Aug 2021 02:21:45 GMT  
		Size: 156.8 MB (156841208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e912d8844618c3e84df88afdb02d2fcc5ed1713afcb23c067a3e0d469ab40951
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.2 MB (268194289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428d43eec21252ab8aa929510a3955ba8fa3a1e59f0f8d49cbf487fc2abf9cd`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:18 GMT
ADD file:42c46f2fd1479c7d309139946c738ffe5c5379a9561b96a8d7511bdb0090481e in / 
# Mon, 26 Jul 2021 23:13:21 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:38:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:47:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:50f10986101895abb3160c75977e8e8eb7b79e82f78fa9dd1883692b644e4675`  
		Last Modified: Mon, 26 Jul 2021 23:16:36 GMT  
		Size: 37.4 MB (37352998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72f19678043711c11465b507df75ce318af4bd2b392f685ca3841dbba055aa`  
		Last Modified: Tue, 27 Jul 2021 04:26:44 GMT  
		Size: 6.1 MB (6133314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a982650c2954b338afda90c5ba86d7603861d62a22b2e3800362985c59823f`  
		Last Modified: Tue, 27 Jul 2021 04:26:43 GMT  
		Size: 4.5 MB (4523551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4da86ef0de66c418b38e81b81a9690c0e7b660053a2b63e8a7b090c8ffdd23`  
		Last Modified: Tue, 27 Jul 2021 04:27:06 GMT  
		Size: 49.5 MB (49482660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df05ea742cc84cf005f5b1fbce3aa2099c7974bbd0654675d0c0ff8c7dbab40f`  
		Last Modified: Tue, 27 Jul 2021 04:27:48 GMT  
		Size: 170.7 MB (170701766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ac52edf6a4ea4ab1f8ee0096caf69ad869cac3a58b760bee7eb927b04a48d6a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.9 MB (257914485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8b02dfe5db83585a676ecaa8de2d87d02ca0e88a0eb635baf0a58f8a5a54119`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:17:33 GMT
ADD file:c9125fcbdad41a027e81c7fc0616e4698eefb4bf591e9c215748c44001492a71 in / 
# Tue, 31 Aug 2021 01:17:35 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:03:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de98d6361415ec89b2135480af53817e96bf60ae2c78c53dad37c447f0f7b040`  
		Last Modified: Tue, 31 Aug 2021 01:33:15 GMT  
		Size: 27.1 MB (27143365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225134e3c31562a8c1d476ee61f8672ab2a39bc9f6dd1aa9d2334027bacf22c0`  
		Last Modified: Tue, 31 Aug 2021 02:44:14 GMT  
		Size: 4.9 MB (4945167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ca77fa5925540bdc2a4cf61c8acfdf7fc0d169793ae57fd6e0b7a6465022d`  
		Last Modified: Tue, 31 Aug 2021 02:44:11 GMT  
		Size: 3.2 MB (3177763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98a854c5e99476d386d6334136c9b5839b261270f40552a56a5557336599fcd`  
		Last Modified: Tue, 31 Aug 2021 02:46:12 GMT  
		Size: 40.3 MB (40329103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c567f920ef8255eb4f50d24bf8b4329ffc4253128705dc547c32723ea2c15bec`  
		Last Modified: Tue, 31 Aug 2021 02:51:50 GMT  
		Size: 182.3 MB (182319087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:16cbc9689a2459ec88062d9374e59c88dd2d38965300fa2f3d8afa87b6141c1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241418909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b8f027f78486d0ae43707e9e3128407eb00ebf6a230cfd375abfca1a96e8690`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:38 GMT
ADD file:ba5c2c420b69d0c125e25122344e156fa468282be3e91af99f6941eb676f308d in / 
# Tue, 31 Aug 2021 01:42:41 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e7ad6541ebda77ecfec574e1268bb944ba28f14ca69dab7bad1d63702975176`  
		Last Modified: Tue, 31 Aug 2021 01:44:29 GMT  
		Size: 32.5 MB (32491578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66e7ecd9588795e7cf09605e17fa940cd2b5566b310df2b484b60ba5faee036`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 5.8 MB (5802191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36acc9b914fe8f7ad986a1869bcd54799c01524d5a43634c1cff6407f77d9a14`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 4.2 MB (4185117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceeae36ed176d953e43f3ac748df4f3d272212947102e33987f59a8cecb55002`  
		Last Modified: Tue, 31 Aug 2021 02:47:06 GMT  
		Size: 47.4 MB (47400028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beaf975b1e5ae8c6fbc46716b09e0482ee34d077a5e324a7cb39c58d7d7e096`  
		Last Modified: Tue, 31 Aug 2021 02:47:32 GMT  
		Size: 151.5 MB (151539995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:hirsute-curl`

```console
$ docker pull buildpack-deps@sha256:3a72acc16fe1512414241dee6ddcb2a633d22a9b56c8f3047b71fa90a6a8b98f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:hirsute-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:87e3c232b29e67193cb8e3a360f59ef5bd082bac752150ac2e8f3dfd8dab5d67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40930192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0edd837b914a819d7989e4d055fee59b4f440b93324d3251e9e278f6af6ae9a1`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a130bec7346768f9e8fb6ac3803a47561327abb05a55c28428690c9fb241360d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34854596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:951f0804064fd4937066c5d9915e51e7a80326b9dffb2c8211540cc7ed1b4b71`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:32 GMT
ADD file:76353e48968f6c84802b150e577cc7fb1bc50985e78e1b499ecd8debfe50d8e5 in / 
# Mon, 26 Jul 2021 22:52:33 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:681a32f1cee4135c0497939e80766271e03a995a197d8293224e8f6bd470bfdd`  
		Last Modified: Mon, 26 Jul 2021 22:57:17 GMT  
		Size: 26.9 MB (26857313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d081ccdbe67f74ab6dab322dc6e8e84a9b56cb1909518f7d199a8fc8936d`  
		Last Modified: Tue, 27 Jul 2021 01:47:35 GMT  
		Size: 4.9 MB (4858897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb191db7ef79ad38fdcde76e18b9267b765696ecf8c500929ef80b649f800`  
		Last Modified: Tue, 27 Jul 2021 01:47:34 GMT  
		Size: 3.1 MB (3138386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1be6a6a353e2c9182de84c02a356036c8dde9815bb83505c0c329d064a55a6db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39202658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a37e4fd97a4962d1b26f3ab8d4d4b3037cf0f744a21cd18626183658d36514b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:53 GMT
ADD file:93dcfc1791d96861438a84bfd38f5c0520353febfcc59bde5510c9e85eab2cf8 in / 
# Tue, 31 Aug 2021 01:40:54 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:11:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4fbd1b15195364f20d4b603e346a2b5c64ae93e9de90f5c1bd82a61e92851632`  
		Last Modified: Tue, 31 Aug 2021 01:42:57 GMT  
		Size: 30.2 MB (30162874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54fbc3de08027791a7280c6d2d7f821165cc126fd0e08c6cba66c1d6fc122`  
		Last Modified: Tue, 31 Aug 2021 02:20:51 GMT  
		Size: 5.4 MB (5401544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7180cc8ab79571bbc48658748543060674d12cbbdf7683a598d89f6086677`  
		Last Modified: Tue, 31 Aug 2021 02:20:50 GMT  
		Size: 3.6 MB (3638240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0d986d60b7c68efa0428ba53ce2fca6f2363653c7ff5b21a2f8137d5f6d82650
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48009863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceb6d2da938e4f3e8ce68f5a01892235875704d7e88689eee9deac09bac85051`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:18 GMT
ADD file:42c46f2fd1479c7d309139946c738ffe5c5379a9561b96a8d7511bdb0090481e in / 
# Mon, 26 Jul 2021 23:13:21 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:50f10986101895abb3160c75977e8e8eb7b79e82f78fa9dd1883692b644e4675`  
		Last Modified: Mon, 26 Jul 2021 23:16:36 GMT  
		Size: 37.4 MB (37352998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72f19678043711c11465b507df75ce318af4bd2b392f685ca3841dbba055aa`  
		Last Modified: Tue, 27 Jul 2021 04:26:44 GMT  
		Size: 6.1 MB (6133314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a982650c2954b338afda90c5ba86d7603861d62a22b2e3800362985c59823f`  
		Last Modified: Tue, 27 Jul 2021 04:26:43 GMT  
		Size: 4.5 MB (4523551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:64c1efaa41585b95c9ae764b82ee6479920b3d19ee810a1fd0dc22c8a73f687c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35266295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1affb32245af279b11f5c62e61f3660f196c615fed09a9a21d3a0e5c8fa2a41b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:17:33 GMT
ADD file:c9125fcbdad41a027e81c7fc0616e4698eefb4bf591e9c215748c44001492a71 in / 
# Tue, 31 Aug 2021 01:17:35 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:03:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:de98d6361415ec89b2135480af53817e96bf60ae2c78c53dad37c447f0f7b040`  
		Last Modified: Tue, 31 Aug 2021 01:33:15 GMT  
		Size: 27.1 MB (27143365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225134e3c31562a8c1d476ee61f8672ab2a39bc9f6dd1aa9d2334027bacf22c0`  
		Last Modified: Tue, 31 Aug 2021 02:44:14 GMT  
		Size: 4.9 MB (4945167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ca77fa5925540bdc2a4cf61c8acfdf7fc0d169793ae57fd6e0b7a6465022d`  
		Last Modified: Tue, 31 Aug 2021 02:44:11 GMT  
		Size: 3.2 MB (3177763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a3a6241c11d52798f69cd608769182ec132e3c3557678a5b7d53de38c8cd7495
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42478886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c486f889ee86ee0e24365015f7d20301cd102b59e96a42c55b86db311ca2572`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:38 GMT
ADD file:ba5c2c420b69d0c125e25122344e156fa468282be3e91af99f6941eb676f308d in / 
# Tue, 31 Aug 2021 01:42:41 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2e7ad6541ebda77ecfec574e1268bb944ba28f14ca69dab7bad1d63702975176`  
		Last Modified: Tue, 31 Aug 2021 01:44:29 GMT  
		Size: 32.5 MB (32491578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66e7ecd9588795e7cf09605e17fa940cd2b5566b310df2b484b60ba5faee036`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 5.8 MB (5802191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36acc9b914fe8f7ad986a1869bcd54799c01524d5a43634c1cff6407f77d9a14`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 4.2 MB (4185117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:hirsute-scm`

```console
$ docker pull buildpack-deps@sha256:3fb49365cba4d74083cb480597e51047a6f356345efc6538476b62d078215bfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:hirsute-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:03c440ab93f47f6f25a8234febc88184480f28020791200b902ad758cc4fc7fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84470558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:823cef2ec1834c9343ac135b8763c224793328b28dd2afae1dad1a2da3016cac`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:55:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9939f009cb8ebf9ee9b4f6b6f99c0a7ca437c96b046a6345f065cbfcc3dde`  
		Last Modified: Mon, 26 Jul 2021 22:13:53 GMT  
		Size: 43.5 MB (43540366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6fcc5afd47847c2e97114df73dfbdb7cb98b3dba59c9d5e0460f5353e0ab2cd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74810727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12dc9111323484a0279e67f569d4cb21203c02f93aa3dcaa657dcc5ac889e26f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:32 GMT
ADD file:76353e48968f6c84802b150e577cc7fb1bc50985e78e1b499ecd8debfe50d8e5 in / 
# Mon, 26 Jul 2021 22:52:33 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:681a32f1cee4135c0497939e80766271e03a995a197d8293224e8f6bd470bfdd`  
		Last Modified: Mon, 26 Jul 2021 22:57:17 GMT  
		Size: 26.9 MB (26857313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d081ccdbe67f74ab6dab322dc6e8e84a9b56cb1909518f7d199a8fc8936d`  
		Last Modified: Tue, 27 Jul 2021 01:47:35 GMT  
		Size: 4.9 MB (4858897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb191db7ef79ad38fdcde76e18b9267b765696ecf8c500929ef80b649f800`  
		Last Modified: Tue, 27 Jul 2021 01:47:34 GMT  
		Size: 3.1 MB (3138386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b923df82160d2d4eea0012b206b82fae9ca16efd703aacc1069a7bb396b558`  
		Last Modified: Tue, 27 Jul 2021 01:48:15 GMT  
		Size: 40.0 MB (39956131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a0e40d34528ab940355ef0e5c6e5a4331f9bb512e5e3104310ea9db74dc73d59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82728192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca32f751faa503b8fea9beef96876f4dbec6142b5dce0a0f3112fd89eb7c213c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:53 GMT
ADD file:93dcfc1791d96861438a84bfd38f5c0520353febfcc59bde5510c9e85eab2cf8 in / 
# Tue, 31 Aug 2021 01:40:54 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:11:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4fbd1b15195364f20d4b603e346a2b5c64ae93e9de90f5c1bd82a61e92851632`  
		Last Modified: Tue, 31 Aug 2021 01:42:57 GMT  
		Size: 30.2 MB (30162874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54fbc3de08027791a7280c6d2d7f821165cc126fd0e08c6cba66c1d6fc122`  
		Last Modified: Tue, 31 Aug 2021 02:20:51 GMT  
		Size: 5.4 MB (5401544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7180cc8ab79571bbc48658748543060674d12cbbdf7683a598d89f6086677`  
		Last Modified: Tue, 31 Aug 2021 02:20:50 GMT  
		Size: 3.6 MB (3638240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826a66d619e21f0b3656bcd20cb8925d105fc0e444b4a72eb69d81408ecf67ed`  
		Last Modified: Tue, 31 Aug 2021 02:21:10 GMT  
		Size: 43.5 MB (43525534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f27c67b36f263760a8087131c54011ace3bd5d7db22c6529665d6abadf899e03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97492523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8b571049a41e25671a9c46d043cc1d74fe7567e153df521e45039f369392ac`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:18 GMT
ADD file:42c46f2fd1479c7d309139946c738ffe5c5379a9561b96a8d7511bdb0090481e in / 
# Mon, 26 Jul 2021 23:13:21 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:38:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:50f10986101895abb3160c75977e8e8eb7b79e82f78fa9dd1883692b644e4675`  
		Last Modified: Mon, 26 Jul 2021 23:16:36 GMT  
		Size: 37.4 MB (37352998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72f19678043711c11465b507df75ce318af4bd2b392f685ca3841dbba055aa`  
		Last Modified: Tue, 27 Jul 2021 04:26:44 GMT  
		Size: 6.1 MB (6133314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a982650c2954b338afda90c5ba86d7603861d62a22b2e3800362985c59823f`  
		Last Modified: Tue, 27 Jul 2021 04:26:43 GMT  
		Size: 4.5 MB (4523551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4da86ef0de66c418b38e81b81a9690c0e7b660053a2b63e8a7b090c8ffdd23`  
		Last Modified: Tue, 27 Jul 2021 04:27:06 GMT  
		Size: 49.5 MB (49482660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:92d46888b25701d05c84398baa31995dd2f2f9cece8d00a6d36ae0b98b41ed12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75595398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a3029ed135684d6a7d55a4aa6663061bf0bddaaac730e68a265ebb4392da89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:17:33 GMT
ADD file:c9125fcbdad41a027e81c7fc0616e4698eefb4bf591e9c215748c44001492a71 in / 
# Tue, 31 Aug 2021 01:17:35 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:03:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de98d6361415ec89b2135480af53817e96bf60ae2c78c53dad37c447f0f7b040`  
		Last Modified: Tue, 31 Aug 2021 01:33:15 GMT  
		Size: 27.1 MB (27143365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225134e3c31562a8c1d476ee61f8672ab2a39bc9f6dd1aa9d2334027bacf22c0`  
		Last Modified: Tue, 31 Aug 2021 02:44:14 GMT  
		Size: 4.9 MB (4945167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ca77fa5925540bdc2a4cf61c8acfdf7fc0d169793ae57fd6e0b7a6465022d`  
		Last Modified: Tue, 31 Aug 2021 02:44:11 GMT  
		Size: 3.2 MB (3177763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98a854c5e99476d386d6334136c9b5839b261270f40552a56a5557336599fcd`  
		Last Modified: Tue, 31 Aug 2021 02:46:12 GMT  
		Size: 40.3 MB (40329103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:946ba36daa4e4c0d9d38cda5253c2dfd87343e5523921f9a8f70978f0698ae7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89878914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e2cfd6247f86f57d874973213ecadf290768b88929aad3faf6c98c3ffda491`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:38 GMT
ADD file:ba5c2c420b69d0c125e25122344e156fa468282be3e91af99f6941eb676f308d in / 
# Tue, 31 Aug 2021 01:42:41 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e7ad6541ebda77ecfec574e1268bb944ba28f14ca69dab7bad1d63702975176`  
		Last Modified: Tue, 31 Aug 2021 01:44:29 GMT  
		Size: 32.5 MB (32491578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66e7ecd9588795e7cf09605e17fa940cd2b5566b310df2b484b60ba5faee036`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 5.8 MB (5802191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36acc9b914fe8f7ad986a1869bcd54799c01524d5a43634c1cff6407f77d9a14`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 4.2 MB (4185117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceeae36ed176d953e43f3ac748df4f3d272212947102e33987f59a8cecb55002`  
		Last Modified: Tue, 31 Aug 2021 02:47:06 GMT  
		Size: 47.4 MB (47400028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:impish`

```console
$ docker pull buildpack-deps@sha256:c7231b3b249de0235336e685852ad6cb611a1c60e593056efb47bb34e3090328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f1fbd344d391628950235e7ebbc2e73a07ec866504c8a8cf07eb080c0424ea23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.0 MB (241014503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29c1f84f1b4abbb17e66779835d3e04817d65d23dac76136a79263e383606b5e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:01 GMT
ADD file:aad4137373f37cc2272f1632b0fa50a91b4c0c878ca72ae8de8fee51ffa2f392 in / 
# Mon, 26 Jul 2021 21:22:02 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:59:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:02:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c8d2949e37d3f87c8d42e502aebe8d287cc56bd1f5846a5265a2124c60cb49c`  
		Last Modified: Mon, 26 Jul 2021 21:24:04 GMT  
		Size: 31.5 MB (31519889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad149f781f55b2a85f0e013b5220678d294bfdc9a113255a07b8fd871224219`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.7 MB (3692251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11936e1d3aa1eb439ea9dac0215a97aa74b71b1eabeed3965b276ff2c836d5e`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.6 MB (3552048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8ee9b3c3bd20f022701661feb52a5704b01f803876f6ebed7ce76763e8308e`  
		Last Modified: Mon, 26 Jul 2021 22:15:03 GMT  
		Size: 37.9 MB (37878472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0aa8dd8688cfc9a43656760d3e978006c45b87ca791b9167139138d70a1b24`  
		Last Modified: Mon, 26 Jul 2021 22:15:39 GMT  
		Size: 164.4 MB (164371843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5928a111b753c3ea702c899aa1dadf079dbfebd238622fe69088e94070f72bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.2 MB (208201657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99da5a03dde9bc7c4517e415d7d5005cf746dd8520e1cc643bfa0671a3071b31`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:54 GMT
ADD file:7c7c93de372cabbc1cbc45bb3618b626ecd538c81cdb8a09c63b397ac79615ca in / 
# Mon, 26 Jul 2021 22:52:55 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:29:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:31:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa3fdc2705d50f3ad184e38a8ae9a54c70a75ef26a8f2036c5cc36454c57b49a`  
		Last Modified: Mon, 26 Jul 2021 22:57:52 GMT  
		Size: 26.9 MB (26876142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05927c7769ed8e7aa2c01453e69c9f65172154a601b0218204df2a1c260a6`  
		Last Modified: Tue, 27 Jul 2021 01:50:05 GMT  
		Size: 3.4 MB (3438752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c89b675bf7d9d2c4ea66630864775dc5879d8e56b1c77d25f08550fd9f882b`  
		Last Modified: Tue, 27 Jul 2021 01:50:04 GMT  
		Size: 3.7 MB (3742290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebac5e3a405d40889f25f311860e0142aaa8172e0dc5fe0de50562f4f0c3a13`  
		Last Modified: Tue, 27 Jul 2021 01:50:46 GMT  
		Size: 40.1 MB (40055381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0958d8b812ecd19d60e605cda443527872d489da05c24b268b265ad90455c7a`  
		Last Modified: Tue, 27 Jul 2021 01:52:18 GMT  
		Size: 134.1 MB (134089092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9fba45e42da203add658a83d947b8063b6e3e8821e9d87f2735a0e7c94861c62
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.5 MB (399490006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d91834fc28eab00910a8bc6ab02bf69640dc79fd4c237189ec0b270e505a452`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:02 GMT
ADD file:ed3a8c55fbedc627dd5d33aecf52df10becbd9bd492f7c3f4f0a710b15629618 in / 
# Tue, 31 Aug 2021 01:41:03 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:13:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:14:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:835dcfefc46e2b5551a40002ffed802b6b70970071e61e3f9dce0dd0404c2a12`  
		Last Modified: Tue, 31 Aug 2021 01:43:19 GMT  
		Size: 29.0 MB (29033527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76d237fe2a405ec5c0175da7117764a3725e495a5280fa68824281d0209f48`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.7 MB (3677477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972cd7eb9f3f8f76c354e0777c1e299b4979c519af36ee25c5a4b5176d14c93b`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.5 MB (3533509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f0c095fc735f206fea57d94ba168122a4d321e4718f54f2db7b3f7c503ed6`  
		Last Modified: Tue, 31 Aug 2021 02:22:17 GMT  
		Size: 38.1 MB (38076803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feef883879fbaff65f9ee52b7386798fbbe6f94a0b6031c782a0345fbb93d11`  
		Last Modified: Tue, 31 Aug 2021 02:23:17 GMT  
		Size: 325.2 MB (325168690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:026f6496bf6d4bafc2b039e06e34dde5dde8d61220141f114a7305ce9e8e2ca3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258293115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c20ecec8e3efdf1ba1eb0ccb7ca993541ac9081c97fa86d026a768ca4c722e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:33 GMT
ADD file:5419572ba3a583506859cb346c0715939486d87fcc143e308557a18a73bb92b2 in / 
# Mon, 26 Jul 2021 23:13:37 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:49:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:50:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:52:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:05:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:415d912bb08e4b766d9582ddc3d0e3c55a978420909d0ce62488cfc6ddcd065d`  
		Last Modified: Mon, 26 Jul 2021 23:17:00 GMT  
		Size: 37.2 MB (37160030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03ededf19de330d97ae5f2cd78f381456f81c19eb46ff80cebace0dbe476eac`  
		Last Modified: Tue, 27 Jul 2021 04:28:02 GMT  
		Size: 4.1 MB (4095072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ec3f753c3934e1f67de00b1cde7c52b2558b372872daab551be31f8ee74787`  
		Last Modified: Tue, 27 Jul 2021 04:28:01 GMT  
		Size: 4.2 MB (4241926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946929704f815af80a61ae55d86531279d22d2292a2f74bf22ed5819c842bb88`  
		Last Modified: Tue, 27 Jul 2021 04:28:22 GMT  
		Size: 42.3 MB (42289669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0c649aac611e54d363fe1b342ef3f246007e65e9ed1524344fb03a95842bd7`  
		Last Modified: Tue, 27 Jul 2021 04:29:05 GMT  
		Size: 170.5 MB (170506418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:e8938656e5921a5d321c930f895539216d4881311214c803e2643503210f917c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.4 MB (267418888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cccfa4b5ab59d8bd311ab4a7f824737ab812260d9622df726a8bf3f0eecd481`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:19:36 GMT
ADD file:84d3daa77b3c4590ccb1b2c1bdfa7b2ea2629a8e289c7e0df33678a72ef40f4c in / 
# Tue, 31 Aug 2021 01:19:38 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:16:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:20:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:26:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2027d80189558886be09b6f8194607cd27258802c79f3c3f228e92404c40c304`  
		Last Modified: Tue, 31 Aug 2021 01:35:47 GMT  
		Size: 27.2 MB (27192169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccb43db8246e726e33f90f4887b26c5c6e5c0eb9b7c4fd223c18539a9963369`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 3.5 MB (3483280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a66489e611edd2a918d67c7aa380888b297b1b1170487f8cf4d412010e9da74`  
		Last Modified: Tue, 31 Aug 2021 02:53:00 GMT  
		Size: 3.8 MB (3803155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2a8d532c190bc5429a7b1a5b15e55c1c120cd8fd520ce5adcdeacadde8c6cb`  
		Last Modified: Tue, 31 Aug 2021 02:55:01 GMT  
		Size: 40.7 MB (40741042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fcfc294837d6a343623ab80428c480526c29b2bb2550c72deb28922f97489f`  
		Last Modified: Tue, 31 Aug 2021 03:00:51 GMT  
		Size: 192.2 MB (192199242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2813c9e36e8aa79b52e8baaa49202e6b8118da28adf2c05c0474ee676685cc4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.4 MB (370398338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c30fa68204d8cf8bba78b5f70b8a1b3fe9b5adefe038d919dc178471b101048`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:54 GMT
ADD file:4748ab039bb7c33cbda2bba944346ecf2e0e6238971d842acc53ec7e8c77df92 in / 
# Tue, 31 Aug 2021 01:42:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:39:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:39:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2abd65908848180c8f2b1a3f2a6493d9c7c22253fc30bc557fce0bbf12327e7`  
		Last Modified: Tue, 31 Aug 2021 01:44:45 GMT  
		Size: 31.3 MB (31308069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f61cb11476011700fc2feeb76881a7eeceb9638e97fa4c33603d64dab544155`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3950090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7802bd74770db74806622bc0f14aa9cc4666241c5b47c5aee05c1b85aa17ebe5`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3962603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e8b1ada6b39a4ab9001051926a2b823d061ce3d31ae907a24efa8fa9961ec`  
		Last Modified: Tue, 31 Aug 2021 02:47:54 GMT  
		Size: 38.9 MB (38858118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62018211b9b26fc8460e4b465948a6eecc369f5b26a1014a1453ed9a8ac2ed7c`  
		Last Modified: Tue, 31 Aug 2021 02:48:36 GMT  
		Size: 292.3 MB (292319458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:e7b8414d525774e5b4628a305abdae6ff90e2fc7b84fedaf62402035b5456292
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c8382f9699ecc7686190ed3ba75041ec06511c7ae5be650adba6abe1a2d1e4a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38764188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f9bb8a11c0d1b625f74b36eed098e3671e1079814f7535e6fa39d4773adb19`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:01 GMT
ADD file:aad4137373f37cc2272f1632b0fa50a91b4c0c878ca72ae8de8fee51ffa2f392 in / 
# Mon, 26 Jul 2021 21:22:02 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:59:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6c8d2949e37d3f87c8d42e502aebe8d287cc56bd1f5846a5265a2124c60cb49c`  
		Last Modified: Mon, 26 Jul 2021 21:24:04 GMT  
		Size: 31.5 MB (31519889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad149f781f55b2a85f0e013b5220678d294bfdc9a113255a07b8fd871224219`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.7 MB (3692251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11936e1d3aa1eb439ea9dac0215a97aa74b71b1eabeed3965b276ff2c836d5e`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.6 MB (3552048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:14cb8487c3b5aea4627a0dd934cbc37283b95eb342ad6ccc08e89753ade64ae9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34057184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f2e381f6175d4348fc21d1d747335f18ba51395951d01822be790604501efd9`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:54 GMT
ADD file:7c7c93de372cabbc1cbc45bb3618b626ecd538c81cdb8a09c63b397ac79615ca in / 
# Mon, 26 Jul 2021 22:52:55 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fa3fdc2705d50f3ad184e38a8ae9a54c70a75ef26a8f2036c5cc36454c57b49a`  
		Last Modified: Mon, 26 Jul 2021 22:57:52 GMT  
		Size: 26.9 MB (26876142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05927c7769ed8e7aa2c01453e69c9f65172154a601b0218204df2a1c260a6`  
		Last Modified: Tue, 27 Jul 2021 01:50:05 GMT  
		Size: 3.4 MB (3438752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c89b675bf7d9d2c4ea66630864775dc5879d8e56b1c77d25f08550fd9f882b`  
		Last Modified: Tue, 27 Jul 2021 01:50:04 GMT  
		Size: 3.7 MB (3742290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a443fd6e3736e490f466797038af04904d36fc0129968f8a26a2d0c0f5411654
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36244513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651cadc9706f04ce4ca19d0656ea6e725e8b0099e4f8ac8a95e0c9db590029d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:02 GMT
ADD file:ed3a8c55fbedc627dd5d33aecf52df10becbd9bd492f7c3f4f0a710b15629618 in / 
# Tue, 31 Aug 2021 01:41:03 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:13:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:835dcfefc46e2b5551a40002ffed802b6b70970071e61e3f9dce0dd0404c2a12`  
		Last Modified: Tue, 31 Aug 2021 01:43:19 GMT  
		Size: 29.0 MB (29033527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76d237fe2a405ec5c0175da7117764a3725e495a5280fa68824281d0209f48`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.7 MB (3677477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972cd7eb9f3f8f76c354e0777c1e299b4979c519af36ee25c5a4b5176d14c93b`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.5 MB (3533509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fb1ae578b0181287cdee49a1ddf90688b5634cddd1742a265064aeb8ca520596
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45497028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b814659ec88c950bcc0e38be82a3b5cbca6e6929da1fe08971ca5efa510f66`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:33 GMT
ADD file:5419572ba3a583506859cb346c0715939486d87fcc143e308557a18a73bb92b2 in / 
# Mon, 26 Jul 2021 23:13:37 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:49:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:50:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:415d912bb08e4b766d9582ddc3d0e3c55a978420909d0ce62488cfc6ddcd065d`  
		Last Modified: Mon, 26 Jul 2021 23:17:00 GMT  
		Size: 37.2 MB (37160030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03ededf19de330d97ae5f2cd78f381456f81c19eb46ff80cebace0dbe476eac`  
		Last Modified: Tue, 27 Jul 2021 04:28:02 GMT  
		Size: 4.1 MB (4095072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ec3f753c3934e1f67de00b1cde7c52b2558b372872daab551be31f8ee74787`  
		Last Modified: Tue, 27 Jul 2021 04:28:01 GMT  
		Size: 4.2 MB (4241926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:97bd04e7cd9db63b4fdfd2f347aa020ccedf795d142138f5bc2fbd99b3405f27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34478604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221e715de9dc218092a332bbdf4433b434c800e4703c3f3ab14ad8b5106fbae8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:19:36 GMT
ADD file:84d3daa77b3c4590ccb1b2c1bdfa7b2ea2629a8e289c7e0df33678a72ef40f4c in / 
# Tue, 31 Aug 2021 01:19:38 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:16:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2027d80189558886be09b6f8194607cd27258802c79f3c3f228e92404c40c304`  
		Last Modified: Tue, 31 Aug 2021 01:35:47 GMT  
		Size: 27.2 MB (27192169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccb43db8246e726e33f90f4887b26c5c6e5c0eb9b7c4fd223c18539a9963369`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 3.5 MB (3483280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a66489e611edd2a918d67c7aa380888b297b1b1170487f8cf4d412010e9da74`  
		Last Modified: Tue, 31 Aug 2021 02:53:00 GMT  
		Size: 3.8 MB (3803155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b3f1c9e13e18f3a6e5662bf31762ed9c77414c91bab87c7de91de6a71e1935e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39220762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cc85733e213410e8138f3ac19e6603d3c39f436a8584a4f0df250ce43cb4d2b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:54 GMT
ADD file:4748ab039bb7c33cbda2bba944346ecf2e0e6238971d842acc53ec7e8c77df92 in / 
# Tue, 31 Aug 2021 01:42:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:39:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2abd65908848180c8f2b1a3f2a6493d9c7c22253fc30bc557fce0bbf12327e7`  
		Last Modified: Tue, 31 Aug 2021 01:44:45 GMT  
		Size: 31.3 MB (31308069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f61cb11476011700fc2feeb76881a7eeceb9638e97fa4c33603d64dab544155`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3950090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7802bd74770db74806622bc0f14aa9cc4666241c5b47c5aee05c1b85aa17ebe5`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3962603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:impish-scm`

```console
$ docker pull buildpack-deps@sha256:b741ca3cf6c93c9c8a833e446bf46c9b00bc74364aceab9ae0552f81563244f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1568944d072c74d3848ea3b159daa499efb19b8ca24a27be213e3e6706358db2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76642660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99660b61d6e2e864495950c7bade0adea9062dd182f11d88cc8c4554a8e4c3e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:01 GMT
ADD file:aad4137373f37cc2272f1632b0fa50a91b4c0c878ca72ae8de8fee51ffa2f392 in / 
# Mon, 26 Jul 2021 21:22:02 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:59:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c8d2949e37d3f87c8d42e502aebe8d287cc56bd1f5846a5265a2124c60cb49c`  
		Last Modified: Mon, 26 Jul 2021 21:24:04 GMT  
		Size: 31.5 MB (31519889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad149f781f55b2a85f0e013b5220678d294bfdc9a113255a07b8fd871224219`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.7 MB (3692251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11936e1d3aa1eb439ea9dac0215a97aa74b71b1eabeed3965b276ff2c836d5e`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.6 MB (3552048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8ee9b3c3bd20f022701661feb52a5704b01f803876f6ebed7ce76763e8308e`  
		Last Modified: Mon, 26 Jul 2021 22:15:03 GMT  
		Size: 37.9 MB (37878472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:af9428118519e17bc6c573f6e9c0997f45932bd2ccd1de24b26ca842ff185561
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74112565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f107b16cd8f0186dee68e0dc6d339ebdf055d86f1a61044e769517f2b951da30`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:54 GMT
ADD file:7c7c93de372cabbc1cbc45bb3618b626ecd538c81cdb8a09c63b397ac79615ca in / 
# Mon, 26 Jul 2021 22:52:55 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:29:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa3fdc2705d50f3ad184e38a8ae9a54c70a75ef26a8f2036c5cc36454c57b49a`  
		Last Modified: Mon, 26 Jul 2021 22:57:52 GMT  
		Size: 26.9 MB (26876142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05927c7769ed8e7aa2c01453e69c9f65172154a601b0218204df2a1c260a6`  
		Last Modified: Tue, 27 Jul 2021 01:50:05 GMT  
		Size: 3.4 MB (3438752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c89b675bf7d9d2c4ea66630864775dc5879d8e56b1c77d25f08550fd9f882b`  
		Last Modified: Tue, 27 Jul 2021 01:50:04 GMT  
		Size: 3.7 MB (3742290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebac5e3a405d40889f25f311860e0142aaa8172e0dc5fe0de50562f4f0c3a13`  
		Last Modified: Tue, 27 Jul 2021 01:50:46 GMT  
		Size: 40.1 MB (40055381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9b14a5032f9cecabfdd36fdd1f4cf36fe9e77c69c67df42361a09c52ab0056ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3ed19e94cacde52671ebc1c2fc041af08a623bce8a636b1f779768b6f239f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:02 GMT
ADD file:ed3a8c55fbedc627dd5d33aecf52df10becbd9bd492f7c3f4f0a710b15629618 in / 
# Tue, 31 Aug 2021 01:41:03 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:13:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:835dcfefc46e2b5551a40002ffed802b6b70970071e61e3f9dce0dd0404c2a12`  
		Last Modified: Tue, 31 Aug 2021 01:43:19 GMT  
		Size: 29.0 MB (29033527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76d237fe2a405ec5c0175da7117764a3725e495a5280fa68824281d0209f48`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.7 MB (3677477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972cd7eb9f3f8f76c354e0777c1e299b4979c519af36ee25c5a4b5176d14c93b`  
		Last Modified: Tue, 31 Aug 2021 02:21:58 GMT  
		Size: 3.5 MB (3533509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964f0c095fc735f206fea57d94ba168122a4d321e4718f54f2db7b3f7c503ed6`  
		Last Modified: Tue, 31 Aug 2021 02:22:17 GMT  
		Size: 38.1 MB (38076803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1465a3eb205a891ac7628435a12af70e11d4d65c5154790ac85cf87d9fff0815
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87786697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12eea146d6a5af6407383e3d75078ee099d3f782c5a9277e03fea2051086cfa`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:33 GMT
ADD file:5419572ba3a583506859cb346c0715939486d87fcc143e308557a18a73bb92b2 in / 
# Mon, 26 Jul 2021 23:13:37 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:49:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:50:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:52:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:415d912bb08e4b766d9582ddc3d0e3c55a978420909d0ce62488cfc6ddcd065d`  
		Last Modified: Mon, 26 Jul 2021 23:17:00 GMT  
		Size: 37.2 MB (37160030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03ededf19de330d97ae5f2cd78f381456f81c19eb46ff80cebace0dbe476eac`  
		Last Modified: Tue, 27 Jul 2021 04:28:02 GMT  
		Size: 4.1 MB (4095072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ec3f753c3934e1f67de00b1cde7c52b2558b372872daab551be31f8ee74787`  
		Last Modified: Tue, 27 Jul 2021 04:28:01 GMT  
		Size: 4.2 MB (4241926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946929704f815af80a61ae55d86531279d22d2292a2f74bf22ed5819c842bb88`  
		Last Modified: Tue, 27 Jul 2021 04:28:22 GMT  
		Size: 42.3 MB (42289669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:614636c66a9fe0c5bdf74d262aea3147673d5e6029e0be438a16320cde474ad5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75219646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df26d2ad97a6b07536755961bac409c36c72d1d41a9afaa589a2659cd1e18050`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:19:36 GMT
ADD file:84d3daa77b3c4590ccb1b2c1bdfa7b2ea2629a8e289c7e0df33678a72ef40f4c in / 
# Tue, 31 Aug 2021 01:19:38 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:16:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:20:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2027d80189558886be09b6f8194607cd27258802c79f3c3f228e92404c40c304`  
		Last Modified: Tue, 31 Aug 2021 01:35:47 GMT  
		Size: 27.2 MB (27192169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccb43db8246e726e33f90f4887b26c5c6e5c0eb9b7c4fd223c18539a9963369`  
		Last Modified: Tue, 31 Aug 2021 02:53:01 GMT  
		Size: 3.5 MB (3483280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a66489e611edd2a918d67c7aa380888b297b1b1170487f8cf4d412010e9da74`  
		Last Modified: Tue, 31 Aug 2021 02:53:00 GMT  
		Size: 3.8 MB (3803155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2a8d532c190bc5429a7b1a5b15e55c1c120cd8fd520ce5adcdeacadde8c6cb`  
		Last Modified: Tue, 31 Aug 2021 02:55:01 GMT  
		Size: 40.7 MB (40741042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:182a5862cbeafa138059b2c711748f5fb7b509f7a52ed4488b483b78a2736457
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.1 MB (78078880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd61715f5db10dc5a7fd9b64563d7002600c850a3a00b72c4217f99b4d3dac1f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:54 GMT
ADD file:4748ab039bb7c33cbda2bba944346ecf2e0e6238971d842acc53ec7e8c77df92 in / 
# Tue, 31 Aug 2021 01:42:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:39:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:39:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2abd65908848180c8f2b1a3f2a6493d9c7c22253fc30bc557fce0bbf12327e7`  
		Last Modified: Tue, 31 Aug 2021 01:44:45 GMT  
		Size: 31.3 MB (31308069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f61cb11476011700fc2feeb76881a7eeceb9638e97fa4c33603d64dab544155`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3950090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7802bd74770db74806622bc0f14aa9cc4666241c5b47c5aee05c1b85aa17ebe5`  
		Last Modified: Tue, 31 Aug 2021 02:47:40 GMT  
		Size: 4.0 MB (3962603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e8b1ada6b39a4ab9001051926a2b823d061ce3d31ae907a24efa8fa9961ec`  
		Last Modified: Tue, 31 Aug 2021 02:47:54 GMT  
		Size: 38.9 MB (38858118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:f84b3ee2dd5104bbb1d77aae6a898d8f1e2a7fa0af22f175b7550ec17ba09df1
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

### `buildpack-deps:latest` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cafaa221feb7c182ed3c3f83f0086da57bc7156c30159366155c5897a86d915b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (321951029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe8fece98de2233a5a26a59d08ff969b8b55b7fbc1a1c6e7ceb6b22ec659b884`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf565088aae3ef2159885f29853bce88eb16082b0c98fcacd08fc9008c84b9`  
		Last Modified: Tue, 17 Aug 2021 09:29:09 GMT  
		Size: 5.2 MB (5153283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c0dd0dc0d3d367cc5b85f86d8881afb658e8eb341a86daf3835c2f14159ac`  
		Last Modified: Tue, 17 Aug 2021 09:29:10 GMT  
		Size: 10.9 MB (10871829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf06daf65610482c638dcc63479a8281e667e37f7842219d66f2dedf63718f4`  
		Last Modified: Tue, 17 Aug 2021 09:29:34 GMT  
		Size: 54.6 MB (54565734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942374d5c11438b68e78d44b36c9eac8fe0a2570c33681d7263b0f3f069c06b9`  
		Last Modified: Tue, 17 Aug 2021 09:30:21 GMT  
		Size: 196.4 MB (196445179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b9c95648c1c4f6bc00721365da71edf685136b260eb2cc57266229470473ce2c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.0 MB (295049846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c41fc84b081c31c9c20ab9f272e38b3482520d7acbd98f04ae0efeaecc5abf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:18:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:21:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b0b6b82f848e8ef423a421d5d46194f7787ebf23e3dcc69fb177eb4dc49f6`  
		Last Modified: Tue, 17 Aug 2021 09:36:54 GMT  
		Size: 5.1 MB (5063684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02ecba39f2b03f1bc47ed6ba17c15a62b11e7eb2ae7397ba374851a864efc67`  
		Last Modified: Tue, 17 Aug 2021 09:36:55 GMT  
		Size: 10.6 MB (10570968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f083cd711c027bf75e496fb0a9b4e8e2ac1a102c5fc0d01c3375757fc102a526`  
		Last Modified: Tue, 17 Aug 2021 09:37:46 GMT  
		Size: 52.3 MB (52319253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c87f1282078740238a813920e2dab455ea24e91c18b10b6e89bfc34d3dabe5`  
		Last Modified: Tue, 17 Aug 2021 09:39:41 GMT  
		Size: 174.6 MB (174643701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:20a100f794f73d9565aeb095033cbd7d03958c4f5cace47051a44b242b46e4e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282478824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648d40b55ba7c2d96aacdb0170baba32efd26ffb7e7e26cb74e8422a52c6fdce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:12:37 GMT
ADD file:579ac9b41923db9165f333faac1330f2924a14f90cab7605ffd66c1815249adf in / 
# Tue, 17 Aug 2021 02:12:38 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:20:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1ce31b8c318c8eac9eba15cdf329f397a64952ab575a09c167fc9ddc5a991a98`  
		Last Modified: Tue, 17 Aug 2021 02:28:44 GMT  
		Size: 50.1 MB (50118546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5a38f951962ad43cfef6137e6638004e3a3f066bb26e2c3b52489258a4b5c`  
		Last Modified: Tue, 17 Aug 2021 15:38:06 GMT  
		Size: 4.9 MB (4922570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a545de7dcb8f9fe8fd65b3b1f104abbb20cee600bc8602beef63ccc4f6259`  
		Last Modified: Tue, 17 Aug 2021 15:38:08 GMT  
		Size: 10.2 MB (10216795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0801bbb4cc34f3ceed00d5e57c23d39f3f1763075f34e2b90a80f078ae6d486a`  
		Last Modified: Tue, 17 Aug 2021 15:38:59 GMT  
		Size: 50.3 MB (50328392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3d7c49ff6810d965ef9be32d59d7da22bf3dd967c4d1f3b3414a7aed7b5ed9`  
		Last Modified: Tue, 17 Aug 2021 15:40:48 GMT  
		Size: 166.9 MB (166892521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c5716ed801cb5ff800dbe3f9364795dc7bbbb0bcea2c08b0b00a0a9def980c69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313622714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787980177678b9ae90f4b44fc98c5baf6b6e494714c2a083736d7ed49fed43db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:52:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:52:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495d06e79f81fe42766bacea59684f27db9d24960b6dd7efeea81f48820d0f6`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 5.1 MB (5142588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd18a2d3ce3a400515ed7a845aeb9d8cd17b023f1efe77ff81292bd63addcc0`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 10.9 MB (10872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfd3a44e1c9b9d3df6b60162d29469b5fe3aaddecba7bf2b122ced08e2a848`  
		Last Modified: Tue, 17 Aug 2021 08:01:25 GMT  
		Size: 54.7 MB (54670308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e87d255e4f38e1f000f523e71beef3ea90c78d187cbca6373c8bcdc15dab325`  
		Last Modified: Tue, 17 Aug 2021 08:02:07 GMT  
		Size: 189.3 MB (189336134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

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

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e56dff8e57c911a088985665f4838cb934b32307330794016163f6bc43f101c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301388823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0407593e24bc9c23a80aec36f20f500b78d2e8635f06aecd1e722db0bc94edf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:42:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:45:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d42212351d464cda967a0b9462fdbf31cf8b926ec739f94ca92a04924b59b44`  
		Last Modified: Tue, 17 Aug 2021 20:53:57 GMT  
		Size: 5.1 MB (5114876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f443b77bd62cad6049ac9b935c37714988629b9b90804c902ebf5d94db0947`  
		Last Modified: Tue, 17 Aug 2021 20:53:59 GMT  
		Size: 10.9 MB (10873298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f994e51a722336aa2b759033a359755271ce92b5d1948340ac2760bd28d90a8`  
		Last Modified: Tue, 17 Aug 2021 20:54:52 GMT  
		Size: 53.3 MB (53297838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb32760aefab4b67e850394277f734a5e65f8191fb6c3dd5e43b4c1577e4c61`  
		Last Modified: Tue, 17 Aug 2021 20:57:03 GMT  
		Size: 178.9 MB (178935476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3035d395cdd02846678666bf0e6fdbafe0fcc72f36134d4cc968c3fc48667386
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330493921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d3e26c8948f38abc9f03d8319b316eb0204deca02aa44662b8ef9338ec5ed0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 14:34:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:53:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f9b82c933b317ed127f45e6f56d6d7508514459e0ef09073b467d3dd8425e`  
		Last Modified: Tue, 17 Aug 2021 15:58:19 GMT  
		Size: 5.4 MB (5401864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a6114ee4fe00702ca86cd44f229643d9324c4b202ed6583f35d2eca848a4a`  
		Last Modified: Tue, 17 Aug 2021 15:58:18 GMT  
		Size: 11.6 MB (11626128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e91c7e9879fdf8ce8ef16f2ba105dac2bc4d76888c86b7b5c63973c05f7ed4`  
		Last Modified: Tue, 17 Aug 2021 16:00:07 GMT  
		Size: 58.8 MB (58849860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8542edff3433d9f519b8030bb7b7f200e5cec504915eda9435d627020680c`  
		Last Modified: Tue, 17 Aug 2021 16:04:00 GMT  
		Size: 195.8 MB (195800037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8b7e5e3f28327cce774548f9e1559535aacb731aa486537b0b1c5458c81caddf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295572826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:186802d3daef183bcf0a403c0ce38346f8c731d225920fe8893adc7c58b07151`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:32:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:32:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20bd918649e02578e4e6f19a2c873dbcc6da7009f7b4ee3088a3e2f594fe6e`  
		Last Modified: Tue, 17 Aug 2021 07:43:16 GMT  
		Size: 5.1 MB (5137099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e43baff5e6307dfe51df170140aa3c7c4b7a4cb3fb03b3a2255a8038c9542`  
		Last Modified: Tue, 17 Aug 2021 07:43:17 GMT  
		Size: 10.8 MB (10761504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163c4ba4cbac76aa2dccf627dc69a5f47c32176dc12e23d0bbbfaa6723a446`  
		Last Modified: Tue, 17 Aug 2021 07:43:35 GMT  
		Size: 54.1 MB (54050153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc89d77adebd4b8848cee8bc0ed80f335c59bbc0b93c29b608cef22175243fe`  
		Last Modified: Tue, 17 Aug 2021 07:44:05 GMT  
		Size: 172.4 MB (172430038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:410405a7cb1b238dfef3c9c3f84a26187296e876b92117fa25bed3a015dd7c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable` - linux; amd64

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

### `buildpack-deps:oldoldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c5429a40f146bf912c705c832cbc25389f3d2161675a42ce9e472082875b03df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309139494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:764861d75f807b284332aa3fa8c966915b39d39bee1b8d8f7254843d50630b01`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:00:50 GMT
ADD file:77054e1fc1091d0e0800f856514f36121a7b447fd1e2df32e6c8ff77e6136c66 in / 
# Tue, 17 Aug 2021 02:00:51 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:31:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:34:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfc6a97ccb61e1bee683ec639f55514bc40b09ef15dcd73c928632c03b3df06c`  
		Last Modified: Tue, 17 Aug 2021 02:18:40 GMT  
		Size: 44.1 MB (44091900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20f6698538a8926450e2bf8d1e9e1f5630637ea61c2b25c184a6a10a108b3e4`  
		Last Modified: Tue, 17 Aug 2021 09:46:08 GMT  
		Size: 10.4 MB (10350685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e83002ce3ccf92cb337a353e881e214497f7e55c7a28f556743242710dbd1a2`  
		Last Modified: Tue, 17 Aug 2021 09:46:04 GMT  
		Size: 4.2 MB (4161501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189296784b99bb4cb5b5de65a61b6597c48637dee4490557ff3e564713b772c3`  
		Last Modified: Tue, 17 Aug 2021 09:46:52 GMT  
		Size: 48.0 MB (47983610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec91ec6f66e8da219762222b74940c02cf181770578d198d2f2575e5efea404`  
		Last Modified: Tue, 17 Aug 2021 09:49:01 GMT  
		Size: 202.6 MB (202551798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

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

### `buildpack-deps:oldoldstable` - linux; arm64 variant v8

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

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:730dd341c80f904d29a15532a89ac80632e9ec3ca37fb49b5a42598754088a9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332745158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afd95a9c0c53c01589fa6e35930e9b20d5c53bddf47bf357d81da909585990bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:05:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aca3d286261da95e058ae37c67e002a572b7dfc1dd7fe13d83060357489bfb`  
		Last Modified: Tue, 17 Aug 2021 02:13:06 GMT  
		Size: 11.4 MB (11353003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d22bbd8aeb7ef47c0fb18407f27411bd8008e1189b79f7c7c3dd1a6adfb7`  
		Last Modified: Tue, 17 Aug 2021 02:13:04 GMT  
		Size: 4.6 MB (4565010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f484f8f178f4bf3f3ec40912975a9e55159419f752b4683fcf11d9317be62c1e`  
		Last Modified: Tue, 17 Aug 2021 02:13:36 GMT  
		Size: 51.3 MB (51265260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686652807b46ef0616820485447143dc2d8fe496a532ae72c2cb0b508e67be60`  
		Last Modified: Tue, 17 Aug 2021 02:14:31 GMT  
		Size: 219.5 MB (219464665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:d02b7f64bfb73fd7bbef2ff4089d5b0a2835e8d81f40ce73e43f8f7fa7d2ca5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f97bd030bd9ca71861a61c9d6070bfa74a81b6f58afc51240259c4bf2e018f68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61018259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c9a62b63fb33454b389e17aea5f5abc09826bb499e30b9143971b9e6467a0b8`
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

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b9f641884fb639f0ddbf2004df2833d07b4df4eab88314b274fe24df4f908ef5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58604086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:901a010af7c0fd8d20a8ef29dadb26b7b9037aa7c3cba9aeb1814d3da18b96f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:00:50 GMT
ADD file:77054e1fc1091d0e0800f856514f36121a7b447fd1e2df32e6c8ff77e6136c66 in / 
# Tue, 17 Aug 2021 02:00:51 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bfc6a97ccb61e1bee683ec639f55514bc40b09ef15dcd73c928632c03b3df06c`  
		Last Modified: Tue, 17 Aug 2021 02:18:40 GMT  
		Size: 44.1 MB (44091900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20f6698538a8926450e2bf8d1e9e1f5630637ea61c2b25c184a6a10a108b3e4`  
		Last Modified: Tue, 17 Aug 2021 09:46:08 GMT  
		Size: 10.4 MB (10350685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e83002ce3ccf92cb337a353e881e214497f7e55c7a28f556743242710dbd1a2`  
		Last Modified: Tue, 17 Aug 2021 09:46:04 GMT  
		Size: 4.2 MB (4161501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f76ce59ad7abdbc8ff07ab0f91412a36027e076f2d87267e839c08e1493af6e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55992627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769c4c3f2e05b3ea5a1f34faae69d5935d3b3bf25b0502b3f51f66d9afab054f`
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

### `buildpack-deps:oldoldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a05e8a73f3ab8eaf3dde75a4f631ace100a433103b2934a0d1fb2aeecbde4e46
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57489982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f8de4cd39074ec0ba6be25bdc437074bc992a7d3e0218fd6957a741c90d203`
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

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:56da13ff13e95aaa610c01385585460016336f54817bf884dfb21e5a284f638a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62015233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d43094d7b883081dbd61e1705ac3e4c9e7e1f5efa1482eee7c698100937a53c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aca3d286261da95e058ae37c67e002a572b7dfc1dd7fe13d83060357489bfb`  
		Last Modified: Tue, 17 Aug 2021 02:13:06 GMT  
		Size: 11.4 MB (11353003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d22bbd8aeb7ef47c0fb18407f27411bd8008e1189b79f7c7c3dd1a6adfb7`  
		Last Modified: Tue, 17 Aug 2021 02:13:04 GMT  
		Size: 4.6 MB (4565010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:c44057c71fee67ac90a7d7de5c568a63909426c17c35d98a45163d43e7cb1ed4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c8cf20dfaed873ec2b57d437fd3dad180e5c25e3b5bcc2d71a9efa4f898f5a15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110779810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f4c42bb45b3d4146db1ca241675e7bc775392475e17e01f5a7ee3ee52a745a`
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

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cb17d66b3425c45df325e2afb076b919e45c5619b389d0d2199904827621f8fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106587696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a7559b36b89cca1b4c88a0013a833598818219be141088a68a2f242d0b5c764`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:00:50 GMT
ADD file:77054e1fc1091d0e0800f856514f36121a7b447fd1e2df32e6c8ff77e6136c66 in / 
# Tue, 17 Aug 2021 02:00:51 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:31:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfc6a97ccb61e1bee683ec639f55514bc40b09ef15dcd73c928632c03b3df06c`  
		Last Modified: Tue, 17 Aug 2021 02:18:40 GMT  
		Size: 44.1 MB (44091900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20f6698538a8926450e2bf8d1e9e1f5630637ea61c2b25c184a6a10a108b3e4`  
		Last Modified: Tue, 17 Aug 2021 09:46:08 GMT  
		Size: 10.4 MB (10350685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e83002ce3ccf92cb337a353e881e214497f7e55c7a28f556743242710dbd1a2`  
		Last Modified: Tue, 17 Aug 2021 09:46:04 GMT  
		Size: 4.2 MB (4161501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189296784b99bb4cb5b5de65a61b6597c48637dee4490557ff3e564713b772c3`  
		Last Modified: Tue, 17 Aug 2021 09:46:52 GMT  
		Size: 48.0 MB (47983610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b0d81bf2020711fddfc13427a5ddf6ff1622419cf1d7f0f7819d24c593843d3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102118784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecab1bcf19c083b34655482d0155cf67c9644e906e5b82ba0c7c75974937896`
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

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6f14f0285f97a25eb7caf7f31213bd1a506cfc18fb9f33146f2ba7e789369811
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105227228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5c63c662f33a6ebdeb59d7cbe0566b0c0ce06d5f2e8671067e1655c48a8075`
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

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a118e684aa2e428350e3fae74c09246820e7a5d41a92d1679f1f4139a06b633a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113280493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e61a364c0adae3b9b246c7e2afa1f6b0145b2424dc75da8e16f94a3701c7e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aca3d286261da95e058ae37c67e002a572b7dfc1dd7fe13d83060357489bfb`  
		Last Modified: Tue, 17 Aug 2021 02:13:06 GMT  
		Size: 11.4 MB (11353003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d22bbd8aeb7ef47c0fb18407f27411bd8008e1189b79f7c7c3dd1a6adfb7`  
		Last Modified: Tue, 17 Aug 2021 02:13:04 GMT  
		Size: 4.6 MB (4565010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f484f8f178f4bf3f3ec40912975a9e55159419f752b4683fcf11d9317be62c1e`  
		Last Modified: Tue, 17 Aug 2021 02:13:36 GMT  
		Size: 51.3 MB (51265260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:ad1d4fa28be6745ab3df67d99e62f5833dd59d4960ecbd707335306fa85ff442
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

### `buildpack-deps:oldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ff472a5ff4bd7253818dfb92e99eee39991da84764d17477d3fad07f06ab1141
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312501525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95271c703a8640d6bc8140abe60bf7dab2e0d95b99f10c284404dcc42e9fce73`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:21:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4099a935a96edef1e9378de34e314d07fb3aea1b7205774055a1fa44a3819f4`  
		Last Modified: Tue, 17 Aug 2021 09:30:37 GMT  
		Size: 7.8 MB (7833079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e2960d83651b1494b4da6c97686e79cc760aa90a75948eed56786726f86928`  
		Last Modified: Tue, 17 Aug 2021 09:30:38 GMT  
		Size: 10.0 MB (9997209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffd4e6385927b79e4d4daa2d00523e766502eed6dd1934e1eda583d348abd8b`  
		Last Modified: Tue, 17 Aug 2021 09:30:58 GMT  
		Size: 51.8 MB (51841042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce46ad6f244a871abfead80f28a613b68fba68e165467d817e09453b369252f`  
		Last Modified: Tue, 17 Aug 2021 09:31:38 GMT  
		Size: 192.4 MB (192393994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:364f2e1bd615a23683b10fdfdb92ae50c06489c895c1ff397dce0c8cc208c57c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286119589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15cdf2a53ae111b3303afe4ac8fbae51a121204bbf99d9e1da4b96b85a705d9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:56:17 GMT
ADD file:784cabdb8b1e35aff6dcfa7acb3c6da5d76ee575188460537a190bab6ef49655 in / 
# Tue, 17 Aug 2021 01:56:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:25:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce5dcedb6ed028586f61d36e8067567349cb049735f9b1fbeb748a005636b9d9`  
		Last Modified: Tue, 17 Aug 2021 02:11:57 GMT  
		Size: 48.2 MB (48153800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1036818934ab73ac9c3e731432ae2c2c576a342f8ac27c0de1654407945f2b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 7.4 MB (7376657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33acf22e716d76b46aa215be86d402b346c30583ac243161d878e673e2e55f3b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824ed8f5821cf4dcfd3bd99d56b7aa9c5eae5312be30686e88b07808d8c0cdc`  
		Last Modified: Tue, 17 Aug 2021 09:40:52 GMT  
		Size: 49.6 MB (49574573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e758f7a7e0da372de0f1611d7468674233f2987fcd71261075cd789d9e68c376`  
		Last Modified: Tue, 17 Aug 2021 09:42:43 GMT  
		Size: 171.3 MB (171327019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d9fa7ab94996efb32eaab7c8363d856078c4236005a258221b1bb956b0e35553
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278336342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfdda06dd06bb9126a7313b6e12f595b0f2c2e92f8f8999e5814c02e077a6e2c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:48 GMT
ADD file:335c38ff88b5e08b7ac0de8108215837affe91919978ea400e32196f7601b991 in / 
# Tue, 17 Aug 2021 02:13:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:21:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:21:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:22:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:24:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:978724337d55541757ceda31b51cc0dcbdb70d7d5bc63ebcc0aaceab90aa8acf`  
		Last Modified: Tue, 17 Aug 2021 02:30:16 GMT  
		Size: 45.9 MB (45917818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f0b0065a7e3b0a78d7b7e0691152e1474bfd7bc177bb8a2383c8b14b0c9dab`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 7.1 MB (7124489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6ed7bdd30c985279190b4c2a50b4257a03d5706663e8ec8c766f425014c39c`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 9.3 MB (9343798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54854fad8c30eacd3b5b5484549685dbf93460ecf31ea30835ec3aa3e3cfa49`  
		Last Modified: Tue, 17 Aug 2021 15:41:54 GMT  
		Size: 47.4 MB (47357324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c39822934191a8ed942f48d7d0005d1f051e099931a35baf8688726dc3ec632`  
		Last Modified: Tue, 17 Aug 2021 15:43:40 GMT  
		Size: 168.6 MB (168592913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:91996eae68b6eaf9ef2e8da9977f75957df26e91cce6e7ee57512071962c18bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (303045063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904acaa22971fd0fb987aab79cd5d55ad3052d4f940c4dd7d20511e547513a04`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:54:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:54:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0eab8670a99c796e5d1a5613581de4cf56c052c3ff83593ca70565c7c45683`  
		Last Modified: Tue, 17 Aug 2021 08:02:43 GMT  
		Size: 52.2 MB (52167867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510a11c58681da817539e7455b4ea1dec3b803bd34d93a7d261508fcdb4a6f74`  
		Last Modified: Tue, 17 Aug 2021 08:03:20 GMT  
		Size: 184.0 MB (183975288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8a5d000723d1d7e1dde9372d4466c86060fcc7d0a75d5f77505d838505df5697
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321916207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08baf0563c53b9fbc69d9dd212ee8b008f0c9955f963977ffa5509d397fd67df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:51 GMT
ADD file:98d4857c154cb75c011be69c57275c4a1304d441ddb03fe8388342bc0e2a9689 in / 
# Tue, 17 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:59:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:00:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:01:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17ec3e1e9f7b10e3075002c6dd4297be244b5386198d7a417a9d22302080b6f7`  
		Last Modified: Tue, 17 Aug 2021 01:50:25 GMT  
		Size: 51.2 MB (51207344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54b2adab88b38d8137579946b8da20be9bdb174381dc3e02340d5a786c41ac`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 8.0 MB (7998779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea932812b2c3a1292981a835c426875eb75f95cb82d925268ceca609a2f23315`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 10.3 MB (10340001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51f590108a6abf5786a02b71f872bd665de64cbee36555dd51fcf8df17b74a`  
		Last Modified: Tue, 17 Aug 2021 02:10:05 GMT  
		Size: 53.4 MB (53437804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ed94c24c31fc57f522ffc87f8d4d7bea22c7b1c41b056fcf497994d3568d1`  
		Last Modified: Tue, 17 Aug 2021 02:11:15 GMT  
		Size: 198.9 MB (198932279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2b0e48869fbf3f77ec60d613fe4f2451863692d821ca110ac445c46ef2314f9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297104024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b277e856e0dbfb86d7a235699dce3f54b041c07fa42b95e67bcbf8c9464bb75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:02 GMT
ADD file:a8c2c0d0623fc8523c52507da1bb3e33e40086f0387a0ec12df9480599a1799e in / 
# Tue, 17 Aug 2021 01:12:03 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:45:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:46:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:49:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e36b8e9dc7a490231e9a4577c7c920ea6252b0b035d31b18e0115e0743d5ca97`  
		Last Modified: Tue, 17 Aug 2021 01:21:04 GMT  
		Size: 49.1 MB (49079655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf1e19e8c366bbeed533597a718657c71c55ace29aedda5015330b7811605a`  
		Last Modified: Tue, 17 Aug 2021 20:57:20 GMT  
		Size: 7.3 MB (7252790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab553f775efe1ebe386c27726c3f1723f48e32fb8865b49e910c181e3cfab788`  
		Last Modified: Tue, 17 Aug 2021 20:57:21 GMT  
		Size: 10.0 MB (10016441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28044c83fd33e51894666e65c54e1691250d8298a8687b14d7a079df5afd69c`  
		Last Modified: Tue, 17 Aug 2021 20:58:09 GMT  
		Size: 50.8 MB (50843141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a254e959b3e0b79e2ecebd56f2318cd2299b7983a3afc46b2ccf4c7400d3cb`  
		Last Modified: Tue, 17 Aug 2021 21:00:16 GMT  
		Size: 179.9 MB (179911997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2e1857e66330a9c88bcd4c611ab4957d2748a322519d057ab23fe1bc854c6d81
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333925560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50fc7bc98fca33962c2d053a05d960cd2f3e563582e2a3ca49919b18a46d8b19`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:35 GMT
ADD file:cd847762c4d814b1302366ad14c10c4fc83be52d52ede8336744b1f0bf988112 in / 
# Tue, 17 Aug 2021 01:33:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:22:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4b39f6d7e8772c5450fb8b799577a194b8bdd1a2935d732d4836f0713e6518a`  
		Last Modified: Tue, 17 Aug 2021 01:47:16 GMT  
		Size: 54.2 MB (54182973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b2ff2b66aeb977708310cb04f7b6110efbc73ff8a538b6f003df129f2fb0f3`  
		Last Modified: Tue, 17 Aug 2021 16:04:35 GMT  
		Size: 8.3 MB (8272123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edeeefbd9326b5c8dbf6c5b3a60d602c1e0f2d0af22dc2cfc28842351dc6b95`  
		Last Modified: Tue, 17 Aug 2021 16:04:33 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350768736925f68aafac882b13a3e7593640560819c88b60d0f566ec1781de0b`  
		Last Modified: Tue, 17 Aug 2021 16:05:58 GMT  
		Size: 57.5 MB (57457638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59be0c0011a56689a0699ad31ad26e9a7da01ae88b4764884cf262f2cb31c28`  
		Last Modified: Tue, 17 Aug 2021 16:10:04 GMT  
		Size: 203.3 MB (203284992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:80d92f21c111dc9c416e40575b17808f5f13edb19cd80fb284baf097ac00d767
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294546507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1088c269f2788cf285d144ee0886437b648e27560a62606824856ada90dc66a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:25 GMT
ADD file:0443e797578f02bf4a9404844d217d992a5dafb634ae3a03ed9e181313f78d4c in / 
# Tue, 17 Aug 2021 01:49:33 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:34:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b14cfca9681354c01ba0c52718b98b1783ccc6a88170ff1b5d491a86f389ccee`  
		Last Modified: Tue, 17 Aug 2021 01:57:51 GMT  
		Size: 49.0 MB (49004330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398cc2dd69156863e1a916460d85ea681c1fea50e25611f3fa0bf634ecda0a97`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 7.4 MB (7400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc3c2fc42de3b04bcd5e6a2d4b4004ba2295b0580a1ae1d2e01ea1d65200a0`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 9.9 MB (9883198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723dbf1359b8c022bdec44c42d0fda155c8ca45da7152e885954f7c17d70c05c`  
		Last Modified: Tue, 17 Aug 2021 07:44:31 GMT  
		Size: 51.4 MB (51380299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0234edac00c22e8e9fac61c99ce359d2968b0d2eed6a0bc430c1312fcb980c`  
		Last Modified: Tue, 17 Aug 2021 07:45:00 GMT  
		Size: 176.9 MB (176877890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:362d5c697af8f484f7ae13c85deea3cab6b00f9ba746c57100d923e9f77084ad
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

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:497fe7d6785c18b508d94d41decc6f8f7747217ed3fa71e5fba86a1cf85c3739
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68266489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1136d707940b8ca41c39cf5bf8ef4e5c65cec971cceb3160138971badc108967`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4099a935a96edef1e9378de34e314d07fb3aea1b7205774055a1fa44a3819f4`  
		Last Modified: Tue, 17 Aug 2021 09:30:37 GMT  
		Size: 7.8 MB (7833079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e2960d83651b1494b4da6c97686e79cc760aa90a75948eed56786726f86928`  
		Last Modified: Tue, 17 Aug 2021 09:30:38 GMT  
		Size: 10.0 MB (9997209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:da5b8eb187b6b53bf095f163c217b3eecc10198c815c9a0c1f26628bb8c26334
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65217997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d44190dbb507ef58f05cf66da856e9c1aa332e05aa3bf37ae7ad4602e90a3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:56:17 GMT
ADD file:784cabdb8b1e35aff6dcfa7acb3c6da5d76ee575188460537a190bab6ef49655 in / 
# Tue, 17 Aug 2021 01:56:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ce5dcedb6ed028586f61d36e8067567349cb049735f9b1fbeb748a005636b9d9`  
		Last Modified: Tue, 17 Aug 2021 02:11:57 GMT  
		Size: 48.2 MB (48153800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1036818934ab73ac9c3e731432ae2c2c576a342f8ac27c0de1654407945f2b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 7.4 MB (7376657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33acf22e716d76b46aa215be86d402b346c30583ac243161d878e673e2e55f3b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:db039b572fd5a9af2d28931774fccafc924168089530272c19bbe8bbc5e2dd91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62386105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d071eaa7bc77231a9601b9803544237251f24da0051d72372ba6d6a08ddd550`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:48 GMT
ADD file:335c38ff88b5e08b7ac0de8108215837affe91919978ea400e32196f7601b991 in / 
# Tue, 17 Aug 2021 02:13:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:21:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:21:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:978724337d55541757ceda31b51cc0dcbdb70d7d5bc63ebcc0aaceab90aa8acf`  
		Last Modified: Tue, 17 Aug 2021 02:30:16 GMT  
		Size: 45.9 MB (45917818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f0b0065a7e3b0a78d7b7e0691152e1474bfd7bc177bb8a2383c8b14b0c9dab`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 7.1 MB (7124489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6ed7bdd30c985279190b4c2a50b4257a03d5706663e8ec8c766f425014c39c`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 9.3 MB (9343798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:32d342f1ccb22c5aab6bbac3708e207a49ee70e3d283dea19a81b8abdfac1ea0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66901908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12cc124d374de8b5eca7edb432d729a09f24f12ddb3bd30040f8f781c80bbffd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0f44fa0a78c1b024b7b57c7dfdaf67fd1d83e6a47c25ba6951db73d1b87367fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69546124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca2a445c5ff6e65a07e933e73aa21587acb1ac2b1a7d72c2c7f2a19b28473ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:51 GMT
ADD file:98d4857c154cb75c011be69c57275c4a1304d441ddb03fe8388342bc0e2a9689 in / 
# Tue, 17 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:59:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:17ec3e1e9f7b10e3075002c6dd4297be244b5386198d7a417a9d22302080b6f7`  
		Last Modified: Tue, 17 Aug 2021 01:50:25 GMT  
		Size: 51.2 MB (51207344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54b2adab88b38d8137579946b8da20be9bdb174381dc3e02340d5a786c41ac`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 8.0 MB (7998779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea932812b2c3a1292981a835c426875eb75f95cb82d925268ceca609a2f23315`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 10.3 MB (10340001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4c8071c6e8cb4d846d227e025984b053fad4a3dd2e703d7125cc81f7db73838d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66348886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f297322b38395246036055fe978a89876b94ff9397851939a20e4d360bc2243`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:02 GMT
ADD file:a8c2c0d0623fc8523c52507da1bb3e33e40086f0387a0ec12df9480599a1799e in / 
# Tue, 17 Aug 2021 01:12:03 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:45:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e36b8e9dc7a490231e9a4577c7c920ea6252b0b035d31b18e0115e0743d5ca97`  
		Last Modified: Tue, 17 Aug 2021 01:21:04 GMT  
		Size: 49.1 MB (49079655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf1e19e8c366bbeed533597a718657c71c55ace29aedda5015330b7811605a`  
		Last Modified: Tue, 17 Aug 2021 20:57:20 GMT  
		Size: 7.3 MB (7252790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab553f775efe1ebe386c27726c3f1723f48e32fb8865b49e910c181e3cfab788`  
		Last Modified: Tue, 17 Aug 2021 20:57:21 GMT  
		Size: 10.0 MB (10016441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f0132bbc40fe6f19e70d6ed09d2468ac0f2aa7e9775e7513f35beb3ca3aa75c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73182930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c52f522da9b38f0d62f5476be6f4360207f575044814019f3f07de43154563d9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:35 GMT
ADD file:cd847762c4d814b1302366ad14c10c4fc83be52d52ede8336744b1f0bf988112 in / 
# Tue, 17 Aug 2021 01:33:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a4b39f6d7e8772c5450fb8b799577a194b8bdd1a2935d732d4836f0713e6518a`  
		Last Modified: Tue, 17 Aug 2021 01:47:16 GMT  
		Size: 54.2 MB (54182973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b2ff2b66aeb977708310cb04f7b6110efbc73ff8a538b6f003df129f2fb0f3`  
		Last Modified: Tue, 17 Aug 2021 16:04:35 GMT  
		Size: 8.3 MB (8272123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edeeefbd9326b5c8dbf6c5b3a60d602c1e0f2d0af22dc2cfc28842351dc6b95`  
		Last Modified: Tue, 17 Aug 2021 16:04:33 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d6f10cb7018413f6e061cee9cf7e810d23904e165779fdf4b8216569577e4d1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66288318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d2ff06a71ed154e37eba7dfe06067e8775954cd4c0746db42a3e636ad810039`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:25 GMT
ADD file:0443e797578f02bf4a9404844d217d992a5dafb634ae3a03ed9e181313f78d4c in / 
# Tue, 17 Aug 2021 01:49:33 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:34:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b14cfca9681354c01ba0c52718b98b1783ccc6a88170ff1b5d491a86f389ccee`  
		Last Modified: Tue, 17 Aug 2021 01:57:51 GMT  
		Size: 49.0 MB (49004330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398cc2dd69156863e1a916460d85ea681c1fea50e25611f3fa0bf634ecda0a97`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 7.4 MB (7400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc3c2fc42de3b04bcd5e6a2d4b4004ba2295b0580a1ae1d2e01ea1d65200a0`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 9.9 MB (9883198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:222c0ca0bba33fec8b59689bc4c25b5213eb0757a28d7f8ef3fe6572327ae4e6
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

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5f0efe6cb5460b8e4c226ac7b8800efd073be90c013db2cecc723fafe67f5a94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120107531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba2bc828a3e5dbc792e59263153ca7d43e8eaea225ac12335765983dae56b210`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:21:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4099a935a96edef1e9378de34e314d07fb3aea1b7205774055a1fa44a3819f4`  
		Last Modified: Tue, 17 Aug 2021 09:30:37 GMT  
		Size: 7.8 MB (7833079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e2960d83651b1494b4da6c97686e79cc760aa90a75948eed56786726f86928`  
		Last Modified: Tue, 17 Aug 2021 09:30:38 GMT  
		Size: 10.0 MB (9997209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffd4e6385927b79e4d4daa2d00523e766502eed6dd1934e1eda583d348abd8b`  
		Last Modified: Tue, 17 Aug 2021 09:30:58 GMT  
		Size: 51.8 MB (51841042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:31841421c87e0d139b3dd546eef3887a00ac38e6a3cd6021e1cb94390646347c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114792570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f63086e65411b3f81d2b2d5de7844c8af328a16f5177a6a77beece3cdee972b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:56:17 GMT
ADD file:784cabdb8b1e35aff6dcfa7acb3c6da5d76ee575188460537a190bab6ef49655 in / 
# Tue, 17 Aug 2021 01:56:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce5dcedb6ed028586f61d36e8067567349cb049735f9b1fbeb748a005636b9d9`  
		Last Modified: Tue, 17 Aug 2021 02:11:57 GMT  
		Size: 48.2 MB (48153800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1036818934ab73ac9c3e731432ae2c2c576a342f8ac27c0de1654407945f2b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 7.4 MB (7376657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33acf22e716d76b46aa215be86d402b346c30583ac243161d878e673e2e55f3b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824ed8f5821cf4dcfd3bd99d56b7aa9c5eae5312be30686e88b07808d8c0cdc`  
		Last Modified: Tue, 17 Aug 2021 09:40:52 GMT  
		Size: 49.6 MB (49574573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:be696c95b2e45c5098978d1443ea5388283dc86a32693296f1ccde7af6276cfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109743429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae06312e8b3ee525f6a2780c2ca3676bbfb804f21eb366f50128fa9ba2a2d0b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:48 GMT
ADD file:335c38ff88b5e08b7ac0de8108215837affe91919978ea400e32196f7601b991 in / 
# Tue, 17 Aug 2021 02:13:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:21:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:21:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:22:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:978724337d55541757ceda31b51cc0dcbdb70d7d5bc63ebcc0aaceab90aa8acf`  
		Last Modified: Tue, 17 Aug 2021 02:30:16 GMT  
		Size: 45.9 MB (45917818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f0b0065a7e3b0a78d7b7e0691152e1474bfd7bc177bb8a2383c8b14b0c9dab`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 7.1 MB (7124489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6ed7bdd30c985279190b4c2a50b4257a03d5706663e8ec8c766f425014c39c`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 9.3 MB (9343798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54854fad8c30eacd3b5b5484549685dbf93460ecf31ea30835ec3aa3e3cfa49`  
		Last Modified: Tue, 17 Aug 2021 15:41:54 GMT  
		Size: 47.4 MB (47357324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f205f4ce2ab7ca9500880d60a78bdbfc28690cb36152742749166702d5c614ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119069775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be45f7fa2e70d1185fbc4913782c90d5e841037e8a39892d75443ec7e2284882`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:54:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0eab8670a99c796e5d1a5613581de4cf56c052c3ff83593ca70565c7c45683`  
		Last Modified: Tue, 17 Aug 2021 08:02:43 GMT  
		Size: 52.2 MB (52167867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b93315610788a1790a30e09d35f401e86e379b24ac307d2f5034f6563b506d83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122983928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae3516212cddb6fe0af927d0804199bcd75b7f211eeca85b15c17500ea4bdeb2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:51 GMT
ADD file:98d4857c154cb75c011be69c57275c4a1304d441ddb03fe8388342bc0e2a9689 in / 
# Tue, 17 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:59:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:00:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17ec3e1e9f7b10e3075002c6dd4297be244b5386198d7a417a9d22302080b6f7`  
		Last Modified: Tue, 17 Aug 2021 01:50:25 GMT  
		Size: 51.2 MB (51207344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54b2adab88b38d8137579946b8da20be9bdb174381dc3e02340d5a786c41ac`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 8.0 MB (7998779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea932812b2c3a1292981a835c426875eb75f95cb82d925268ceca609a2f23315`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 10.3 MB (10340001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51f590108a6abf5786a02b71f872bd665de64cbee36555dd51fcf8df17b74a`  
		Last Modified: Tue, 17 Aug 2021 02:10:05 GMT  
		Size: 53.4 MB (53437804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:cdd5f0a255e2b203fda9f9da748b29d1cbd1c436a3fab250c00d98a766f0811a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117192027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b8420dbc34754e42504603d5492904047f7b20448d055a240048862336a2e9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:02 GMT
ADD file:a8c2c0d0623fc8523c52507da1bb3e33e40086f0387a0ec12df9480599a1799e in / 
# Tue, 17 Aug 2021 01:12:03 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:45:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:46:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e36b8e9dc7a490231e9a4577c7c920ea6252b0b035d31b18e0115e0743d5ca97`  
		Last Modified: Tue, 17 Aug 2021 01:21:04 GMT  
		Size: 49.1 MB (49079655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf1e19e8c366bbeed533597a718657c71c55ace29aedda5015330b7811605a`  
		Last Modified: Tue, 17 Aug 2021 20:57:20 GMT  
		Size: 7.3 MB (7252790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab553f775efe1ebe386c27726c3f1723f48e32fb8865b49e910c181e3cfab788`  
		Last Modified: Tue, 17 Aug 2021 20:57:21 GMT  
		Size: 10.0 MB (10016441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28044c83fd33e51894666e65c54e1691250d8298a8687b14d7a079df5afd69c`  
		Last Modified: Tue, 17 Aug 2021 20:58:09 GMT  
		Size: 50.8 MB (50843141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:986a9620f9dde7ab2ba404bf95257d683551ad4cdb24c380d99d6742723a2faf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130640568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60fea57c4f4e9377c6d9ebfba03667f4f5c98dbf30cd02020d8ed9da9e950dd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:35 GMT
ADD file:cd847762c4d814b1302366ad14c10c4fc83be52d52ede8336744b1f0bf988112 in / 
# Tue, 17 Aug 2021 01:33:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4b39f6d7e8772c5450fb8b799577a194b8bdd1a2935d732d4836f0713e6518a`  
		Last Modified: Tue, 17 Aug 2021 01:47:16 GMT  
		Size: 54.2 MB (54182973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b2ff2b66aeb977708310cb04f7b6110efbc73ff8a538b6f003df129f2fb0f3`  
		Last Modified: Tue, 17 Aug 2021 16:04:35 GMT  
		Size: 8.3 MB (8272123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edeeefbd9326b5c8dbf6c5b3a60d602c1e0f2d0af22dc2cfc28842351dc6b95`  
		Last Modified: Tue, 17 Aug 2021 16:04:33 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350768736925f68aafac882b13a3e7593640560819c88b60d0f566ec1781de0b`  
		Last Modified: Tue, 17 Aug 2021 16:05:58 GMT  
		Size: 57.5 MB (57457638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bd5e99eae2c75ab38c62bb8c506df389296ceef68663a6cf77c3c9574b582396
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117668617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd52a53fd4d502b1e8e07b671196e14bac22b39fc9ff3c5f64b4092d60e97af6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:25 GMT
ADD file:0443e797578f02bf4a9404844d217d992a5dafb634ae3a03ed9e181313f78d4c in / 
# Tue, 17 Aug 2021 01:49:33 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:34:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b14cfca9681354c01ba0c52718b98b1783ccc6a88170ff1b5d491a86f389ccee`  
		Last Modified: Tue, 17 Aug 2021 01:57:51 GMT  
		Size: 49.0 MB (49004330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398cc2dd69156863e1a916460d85ea681c1fea50e25611f3fa0bf634ecda0a97`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 7.4 MB (7400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc3c2fc42de3b04bcd5e6a2d4b4004ba2295b0580a1ae1d2e01ea1d65200a0`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 9.9 MB (9883198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723dbf1359b8c022bdec44c42d0fda155c8ca45da7152e885954f7c17d70c05c`  
		Last Modified: Tue, 17 Aug 2021 07:44:31 GMT  
		Size: 51.4 MB (51380299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:7c9700c28be70bfd3bae7ec1bca0be928e089a0dabeac1547d9d01821dc1137e
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
$ docker pull buildpack-deps@sha256:fcf696e81fbb39515e31895fbeedb08b0bf07e1bc8bfac1094b1f4adfebad8e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125505850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f8c023a59a00085d55f58463800a73350f5a479bc85bd8fec65c6d63c59b9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf565088aae3ef2159885f29853bce88eb16082b0c98fcacd08fc9008c84b9`  
		Last Modified: Tue, 17 Aug 2021 09:29:09 GMT  
		Size: 5.2 MB (5153283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c0dd0dc0d3d367cc5b85f86d8881afb658e8eb341a86daf3835c2f14159ac`  
		Last Modified: Tue, 17 Aug 2021 09:29:10 GMT  
		Size: 10.9 MB (10871829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf06daf65610482c638dcc63479a8281e667e37f7842219d66f2dedf63718f4`  
		Last Modified: Tue, 17 Aug 2021 09:29:34 GMT  
		Size: 54.6 MB (54565734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f4f9aaf82aa16a66de2601280af242b6eed140501fdefc27dbddaee1a2abd04d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120406145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7f7ffa4516f21995c9d82c55032542d253b9c19f3e8a3c7a5a351e3f28904bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:18:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b0b6b82f848e8ef423a421d5d46194f7787ebf23e3dcc69fb177eb4dc49f6`  
		Last Modified: Tue, 17 Aug 2021 09:36:54 GMT  
		Size: 5.1 MB (5063684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02ecba39f2b03f1bc47ed6ba17c15a62b11e7eb2ae7397ba374851a864efc67`  
		Last Modified: Tue, 17 Aug 2021 09:36:55 GMT  
		Size: 10.6 MB (10570968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f083cd711c027bf75e496fb0a9b4e8e2ac1a102c5fc0d01c3375757fc102a526`  
		Last Modified: Tue, 17 Aug 2021 09:37:46 GMT  
		Size: 52.3 MB (52319253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:952205bc7cddbbfb9fa8d02a6b6359b25693f6c583577f30ae38f6fc953128d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115586303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67953dbcbb8bcfebe0afc9db6d95f9f661b8a7f422c688642a536fd858e9d5a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:12:37 GMT
ADD file:579ac9b41923db9165f333faac1330f2924a14f90cab7605ffd66c1815249adf in / 
# Tue, 17 Aug 2021 02:12:38 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1ce31b8c318c8eac9eba15cdf329f397a64952ab575a09c167fc9ddc5a991a98`  
		Last Modified: Tue, 17 Aug 2021 02:28:44 GMT  
		Size: 50.1 MB (50118546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5a38f951962ad43cfef6137e6638004e3a3f066bb26e2c3b52489258a4b5c`  
		Last Modified: Tue, 17 Aug 2021 15:38:06 GMT  
		Size: 4.9 MB (4922570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a545de7dcb8f9fe8fd65b3b1f104abbb20cee600bc8602beef63ccc4f6259`  
		Last Modified: Tue, 17 Aug 2021 15:38:08 GMT  
		Size: 10.2 MB (10216795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0801bbb4cc34f3ceed00d5e57c23d39f3f1763075f34e2b90a80f078ae6d486a`  
		Last Modified: Tue, 17 Aug 2021 15:38:59 GMT  
		Size: 50.3 MB (50328392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7466552e59983c946898f07f77837b743f3b156ff789fc751ee98a02a9add3b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124286580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d51b8f3ab483064d973aecc62a3b04b730815b474f7f9793cd107f3f79f6dad2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:52:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:52:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495d06e79f81fe42766bacea59684f27db9d24960b6dd7efeea81f48820d0f6`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 5.1 MB (5142588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd18a2d3ce3a400515ed7a845aeb9d8cd17b023f1efe77ff81292bd63addcc0`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 10.9 MB (10872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfd3a44e1c9b9d3df6b60162d29469b5fe3aaddecba7bf2b122ced08e2a848`  
		Last Modified: Tue, 17 Aug 2021 08:01:25 GMT  
		Size: 54.7 MB (54670308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:00be0f57bc7e719a20f1fa7c7544e0df9c6853fb707efac9b901c65b6c06ba5a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128372373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca098a2a0c1d25e4bb10cde9432093d0aa17de51005d3952d00ec8f1d6b262b2`
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

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:03f5904c242d11766ad5bf5183be9e7630b9e37d9670519c71a54b93a9c4d095
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122453347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63db1c68912deb8496753716857c5912bdf02ca2a4bad7229ef3b7bdeab044a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:42:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d42212351d464cda967a0b9462fdbf31cf8b926ec739f94ca92a04924b59b44`  
		Last Modified: Tue, 17 Aug 2021 20:53:57 GMT  
		Size: 5.1 MB (5114876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f443b77bd62cad6049ac9b935c37714988629b9b90804c902ebf5d94db0947`  
		Last Modified: Tue, 17 Aug 2021 20:53:59 GMT  
		Size: 10.9 MB (10873298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f994e51a722336aa2b759033a359755271ce92b5d1948340ac2760bd28d90a8`  
		Last Modified: Tue, 17 Aug 2021 20:54:52 GMT  
		Size: 53.3 MB (53297838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fcbc2251bc93c2efb3d7fba801d28ae0f31bcd293b3ba7c7a232d9dd37ba5578
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134693884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d90068795b93d0a5374de038dbf136ba1114dd082e28d5b649c0406f044c8fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 14:34:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f9b82c933b317ed127f45e6f56d6d7508514459e0ef09073b467d3dd8425e`  
		Last Modified: Tue, 17 Aug 2021 15:58:19 GMT  
		Size: 5.4 MB (5401864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a6114ee4fe00702ca86cd44f229643d9324c4b202ed6583f35d2eca848a4a`  
		Last Modified: Tue, 17 Aug 2021 15:58:18 GMT  
		Size: 11.6 MB (11626128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e91c7e9879fdf8ce8ef16f2ba105dac2bc4d76888c86b7b5c63973c05f7ed4`  
		Last Modified: Tue, 17 Aug 2021 16:00:07 GMT  
		Size: 58.8 MB (58849860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5bae3f8d99ee48e52b19e9cd49f9ecfd1154979fb8ab49ec52a4f4d74ba5cdae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123142788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8878de09ccb0b4cf42119e9df2aaefcfc61cbfc3ce818b2f70133e76585d8413`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:32:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:32:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20bd918649e02578e4e6f19a2c873dbcc6da7009f7b4ee3088a3e2f594fe6e`  
		Last Modified: Tue, 17 Aug 2021 07:43:16 GMT  
		Size: 5.1 MB (5137099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e43baff5e6307dfe51df170140aa3c7c4b7a4cb3fb03b3a2255a8038c9542`  
		Last Modified: Tue, 17 Aug 2021 07:43:17 GMT  
		Size: 10.8 MB (10761504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163c4ba4cbac76aa2dccf627dc69a5f47c32176dc12e23d0bbbfaa6723a446`  
		Last Modified: Tue, 17 Aug 2021 07:43:35 GMT  
		Size: 54.1 MB (54050153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:e4cfe790617d2ffabc8a963300bbb2f38bba6c162ac644150f7c4b3f17ca5556
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9164c1de3ee959d94d9a02a9b9fc381d9920f63439a879416e11babcb20c201c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.9 MB (323887742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47dd1f6893fa5d12feded97d9a2eaee1d1451d93d7941dd8cbf829d9cf976cd1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:06 GMT
ADD file:3052ec53a19fa26baad5d50e4d2867be2cc386ae62195d8dbb9d90d0b904c464 in / 
# Tue, 17 Aug 2021 01:25:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:24:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6952a6bd46e0eaa2c0e7e851a45f288b3dc080472a9249e48c74b3fb7551fcc`  
		Last Modified: Tue, 17 Aug 2021 01:31:55 GMT  
		Size: 54.9 MB (54930846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ac09fd3cc15f0b26d3a8005c31390d5de204431a0355ffc55e60a6a8f3b25`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 5.2 MB (5171335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e5aaa7713c8cc3d2dd4d36732e1aac9d876c81ddc49221a0d413f2d4f7dcb1`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 10.9 MB (10872817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11986d12d3ac34fc246feb151c1fbc9cdf5db866e53edb07c12fcda5e91e187a`  
		Last Modified: Tue, 17 Aug 2021 09:32:14 GMT  
		Size: 55.5 MB (55453832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f5ea41d022ec1a5a36111aa96cf323591a2da89a14eaff8b4a7daf934e07db`  
		Last Modified: Tue, 17 Aug 2021 09:32:59 GMT  
		Size: 197.5 MB (197458912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:698f3ba6ac57420b4376d98d74a3565525e5508f17abb7d81a864084630f893d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.7 MB (296739431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe4db913c27b633c7fceef07d6d7ed9cedd47c78761439492de9ccfc7b0c93be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:59:08 GMT
ADD file:f9ad3ec0db7a58cdae9cae8207122785d2b8c116c5bb4d47d46f530bda897397 in / 
# Tue, 17 Aug 2021 01:59:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:26:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:27:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:29:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f84c96ba3e58d3cff4f87a969dd91565bb9be34588bf76d1a5a253c40ee1139`  
		Last Modified: Tue, 17 Aug 2021 02:16:06 GMT  
		Size: 52.5 MB (52493950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97b83ef80c1b594046817ebd2be34eaa8faee56f4463a801453d7757341208b`  
		Last Modified: Tue, 17 Aug 2021 09:42:59 GMT  
		Size: 5.1 MB (5075615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c50a77e6ef78b9b162607f1afc018b1b92ec1874e815ace7ce3c948fe8c8ea`  
		Last Modified: Tue, 17 Aug 2021 09:43:02 GMT  
		Size: 10.6 MB (10572088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c2bac917a1fcd804dd397408311320a680c743c2e90437422491a062c16b37`  
		Last Modified: Tue, 17 Aug 2021 09:43:52 GMT  
		Size: 53.2 MB (53162948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3bfc85a26073067cb5d47404e861e10a9b16acbeaf9a46bf6f5ff7e4c76f26`  
		Last Modified: Tue, 17 Aug 2021 09:45:50 GMT  
		Size: 175.4 MB (175434830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b3d4233d2c38ac382c41432382339368b97b4091dd57b816568d20a38f83339c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.2 MB (284204177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0cdedcbc9c431bec8e9a11931577f0827e9460fe4221c57dd5b6ba4b477b7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:17:03 GMT
ADD file:75b6eb36a0ba8612cac405c278e0b6859f0857f284d7f2da3bc8ad6f4596cb7d in / 
# Tue, 17 Aug 2021 02:17:04 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:25:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:25:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:26:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:27:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86a6508bfdcb208b57a6ef5ca954ff178d89a14ca7c65b27bcd68df01e915895`  
		Last Modified: Tue, 17 Aug 2021 02:34:04 GMT  
		Size: 50.1 MB (50148031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894d51adc3dd9d078687cb2de22546210c7c13da66ac22c2e59180e6c194ddb`  
		Last Modified: Tue, 17 Aug 2021 15:43:55 GMT  
		Size: 4.9 MB (4937133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c61d960a4bb6b195a3e18c7e848519224d78371f6f147c8385202bcdab4023`  
		Last Modified: Tue, 17 Aug 2021 15:43:57 GMT  
		Size: 10.2 MB (10217512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cacd13952822a4eee5f0a451c9ca9324612dfe962c2c8f6c1e5ad8ec953c3c`  
		Last Modified: Tue, 17 Aug 2021 15:44:48 GMT  
		Size: 51.1 MB (51113693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98862062e57fe52710d4ffb6c0843dda047d1266229ba48b659752bc45f51895`  
		Last Modified: Tue, 17 Aug 2021 15:46:36 GMT  
		Size: 167.8 MB (167787808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7030b40a4d93866530c63b0070c4fb19df9d4b2d8e9c45fa08a148cbf4b68697
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.5 MB (315489595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8b77487ed2389e4f72c688d728194d97cb3bf6cf78144f4983b358713225cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:32 GMT
ADD file:2eb550b4dc61105505c60437af91d7300fc5596834bfce84a75b260663bf4f42 in / 
# Tue, 17 Aug 2021 01:47:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:55:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:55:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:55:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:56:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c8e1604d5b38112a190afe29ac6b4d1c501651ae9e68b6eaa49788ae64f145d`  
		Last Modified: Tue, 17 Aug 2021 01:56:14 GMT  
		Size: 53.6 MB (53625965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4b3d12f8e0cac2ab78286575b8f56d2cadedcafd68908cc60821856f5e360`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 5.2 MB (5160051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb41ce34a000fbba6dafcb340db9d0b7f64a8efd27ff966f77978ddd2c567439`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 10.9 MB (10873429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7ff3790681e7d2217b96a8b89bdf6b99ab28fa3c7c0da0c88118fa977a7ce9`  
		Last Modified: Tue, 17 Aug 2021 08:03:58 GMT  
		Size: 55.4 MB (55414468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168df4c59e132a8a240d09c437b400a3c05962347006f90a438bd329f995729`  
		Last Modified: Tue, 17 Aug 2021 08:04:37 GMT  
		Size: 190.4 MB (190415682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:97d4fde8a2be765cae7f2ab60ba592c97c8fa2e0a9d5c68af477246aa4d62768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329396504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5acf4b10d41b0fe38a7f0365df036214514ac503b45b8d91bb5d5f72329683e6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:42 GMT
ADD file:8d9eb4b2afc4eb0058f4080c5f0eedf0ddef323f1cc5a0403658254d191f117e in / 
# Tue, 17 Aug 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:02:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:03:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:79e62a40ce7bfbbe436e33c1da1c5661386b9674fe81402fdbfbb42a5b84998b`  
		Last Modified: Tue, 17 Aug 2021 01:52:55 GMT  
		Size: 56.0 MB (55967475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3391f9add930caab1f7ad8d326db740aab914960a3522b2baea8f34b06d23`  
		Last Modified: Tue, 17 Aug 2021 02:11:30 GMT  
		Size: 5.3 MB (5301763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c1c03bbd7c2f8c23dd8b5a8bae89de98d00fe400f6f7c89140aed7a78c6aa7`  
		Last Modified: Tue, 17 Aug 2021 02:11:31 GMT  
		Size: 11.3 MB (11250490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71047ae47f0ad2d0279c1731200ffbae15c68839f662197eb53927e89f4a346a`  
		Last Modified: Tue, 17 Aug 2021 02:11:56 GMT  
		Size: 56.7 MB (56684792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2118c03028a270167b86bbfa714238fc20ce6fcba7db2de02928657dbbcdb9`  
		Last Modified: Tue, 17 Aug 2021 02:12:48 GMT  
		Size: 200.2 MB (200191984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3afe0eb83a1d2b02654ced38fce91c3113deefaf57a2eb0c344eeca8c167f5fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (302974399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8334ddfd22e4126eab61b74efdbc14fd1220498aefd2fbc6852cbd759cfd112`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:13:43 GMT
ADD file:a77aad2a2ac623e0a0640ce1caa07dc2982875f5e01f2baec92d08795be4ad93 in / 
# Tue, 17 Aug 2021 01:13:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:51:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:53:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e190daae609fdf78d1dc3b15955b491e5dba465be6fc9a8a7ffc7a7039ffccd6`  
		Last Modified: Tue, 17 Aug 2021 01:23:46 GMT  
		Size: 53.2 MB (53198954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86d281139f06d0443f660a40811f7a489e4a83c078e49d5b8f57195e98409cf`  
		Last Modified: Tue, 17 Aug 2021 21:00:30 GMT  
		Size: 5.1 MB (5131004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99713d0cdbd7eef9bc879aca6d384c6712d27d4af1616629bada8c72f448a620`  
		Last Modified: Tue, 17 Aug 2021 21:00:33 GMT  
		Size: 10.9 MB (10873555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa119cf8ddcc3e8e9ab5ccb513faee61d808d3ca9cfb4d4ef9d68386a6848f`  
		Last Modified: Tue, 17 Aug 2021 21:01:23 GMT  
		Size: 54.3 MB (54264071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614453a7d63e2b291eae511f2a53543b63f728d3d16e35342663dd17bb00e1a6`  
		Last Modified: Tue, 17 Aug 2021 21:03:30 GMT  
		Size: 179.5 MB (179506815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c3bd218a847687d723b4ea74f3d272c6c3d821c14455f89aa40519ac92162367
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332737468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f34fe1147300f860a425db5f0166a3f5469ec71225b0edab829490bf30faca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:35:46 GMT
ADD file:3bdf0f06854c7b6578701900c267a6a5a712e84cc267d519df82eb28d568221c in / 
# Tue, 17 Aug 2021 01:35:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:24:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:26:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:54:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d596d5bddf4c6763b1156eb07675e21eb75a9b5bc9e5629b035d92244696d704`  
		Last Modified: Tue, 17 Aug 2021 01:52:09 GMT  
		Size: 58.9 MB (58855169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3055c003e2e867f5f7baa6505d799eff17441266441133ae556e40de99b75429`  
		Last Modified: Tue, 17 Aug 2021 16:10:29 GMT  
		Size: 5.4 MB (5421863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a281bbbade77271f6acd86003d63e414b000f703adebe3ff4c838ab7244b2c`  
		Last Modified: Tue, 17 Aug 2021 16:10:31 GMT  
		Size: 11.6 MB (11626757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d86af2c2f0d04abf574423e9d1d5c3771093d278c3c65bcb999fee07604f643`  
		Last Modified: Tue, 17 Aug 2021 16:12:29 GMT  
		Size: 59.9 MB (59883318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815763adc68353307c31a3ba0dce4b537a40f61b31cf42e0e050874ee170db45`  
		Last Modified: Tue, 17 Aug 2021 16:15:04 GMT  
		Size: 197.0 MB (196950361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:791e251bc4cb264f5035b6d51f0de093de65a9b68e2c02d3887b5dd55bf589c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329744362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5900075fa959e9c06925c33138e367fe67bbfcbfe99d3e4d8d0751e575a1429`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:57 GMT
ADD file:17c3a69ac6b2ac905f0d9d5d8d828215848c91b6aca208c63e3c8c6c3c28ac20 in / 
# Tue, 17 Aug 2021 01:45:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:29:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:33:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:43:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03abe71e39e08cd630ff168b11929dc5c3c5111cfb3d81f5a8183f7ba7162fab`  
		Last Modified: Tue, 17 Aug 2021 02:01:48 GMT  
		Size: 50.4 MB (50437771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e3ddf2aa723d9dc92fc071b3cc373219cd68de4072a024dc13965f2156705`  
		Last Modified: Tue, 17 Aug 2021 03:07:39 GMT  
		Size: 5.0 MB (4984859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbcb287940d650490755774d53a8edf26fba9558538160b4f649b66979ee4d`  
		Last Modified: Tue, 17 Aug 2021 03:07:43 GMT  
		Size: 10.3 MB (10293904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecda3ed528238bab9bf59ea2bc04887f931df81d6afd6768a21f6cb99a711637`  
		Last Modified: Tue, 17 Aug 2021 03:09:51 GMT  
		Size: 51.4 MB (51387224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3175c8a8bbf446d59b78ab670863174b7a4426d3ff03cafcf314f6c0449c4f05`  
		Last Modified: Tue, 17 Aug 2021 03:15:44 GMT  
		Size: 212.6 MB (212640604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:00c27d2eaa6c65a4cabff2ccc774ff8415fdc24e95cacf11fd8a9158729549b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.2 MB (297230778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f8588692cd0ecb96393420b73e8864acb9011c076ff04727891cc6ca741813f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:51:06 GMT
ADD file:ab809bd14c40234cf29151f2485ed39a9fa31f67c202abe6bf8546f5899aa52f in / 
# Tue, 17 Aug 2021 01:51:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:37:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:39:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6758b3369d7c595105d273788911a60f3cbd8b26d39dea406c75de4d1da4a084`  
		Last Modified: Tue, 17 Aug 2021 01:59:02 GMT  
		Size: 53.2 MB (53226590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee5f5767e372ec2c62434ed4325aa1b14846b20d736bdb81e1861163803d98`  
		Last Modified: Tue, 17 Aug 2021 07:45:09 GMT  
		Size: 5.2 MB (5152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1daed3fa6142f9fe36fd70a1e631c71aa839f077885d60cb4e7fb21210dacc`  
		Last Modified: Tue, 17 Aug 2021 07:45:10 GMT  
		Size: 10.8 MB (10763976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52078ebb293da4fc08dd7b04c3124715e75d72e8d33e91bcdaf326bcad28bdb`  
		Last Modified: Tue, 17 Aug 2021 07:45:26 GMT  
		Size: 54.7 MB (54724881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095155f9776442484b7b68f12906c0078739fa9a10717a8b4caf8bae637f75ba`  
		Last Modified: Tue, 17 Aug 2021 07:45:54 GMT  
		Size: 173.4 MB (173362475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:9024dbabe7a1da375a2ea36118557b2f0f3c1c7a7eeddae64d719108a78539a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5d6bc794b03974feb0bca10638255c61d229c30482c16488bf76bd19de3866c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70974998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b61c222380eee70d755288337c14d488c6aaa25dcd184ed039dbaef3fabab8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:06 GMT
ADD file:3052ec53a19fa26baad5d50e4d2867be2cc386ae62195d8dbb9d90d0b904c464 in / 
# Tue, 17 Aug 2021 01:25:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a6952a6bd46e0eaa2c0e7e851a45f288b3dc080472a9249e48c74b3fb7551fcc`  
		Last Modified: Tue, 17 Aug 2021 01:31:55 GMT  
		Size: 54.9 MB (54930846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ac09fd3cc15f0b26d3a8005c31390d5de204431a0355ffc55e60a6a8f3b25`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 5.2 MB (5171335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e5aaa7713c8cc3d2dd4d36732e1aac9d876c81ddc49221a0d413f2d4f7dcb1`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 10.9 MB (10872817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3d791feb2549b4b03c2e48bcb7d5deb42f1a8752dda92091267f9867edfb81c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68141653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebd6ddbec1219266e98b1930904201cf38f080dc8ab6427e0c39b6fdb448051e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:59:08 GMT
ADD file:f9ad3ec0db7a58cdae9cae8207122785d2b8c116c5bb4d47d46f530bda897397 in / 
# Tue, 17 Aug 2021 01:59:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:26:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8f84c96ba3e58d3cff4f87a969dd91565bb9be34588bf76d1a5a253c40ee1139`  
		Last Modified: Tue, 17 Aug 2021 02:16:06 GMT  
		Size: 52.5 MB (52493950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97b83ef80c1b594046817ebd2be34eaa8faee56f4463a801453d7757341208b`  
		Last Modified: Tue, 17 Aug 2021 09:42:59 GMT  
		Size: 5.1 MB (5075615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c50a77e6ef78b9b162607f1afc018b1b92ec1874e815ace7ce3c948fe8c8ea`  
		Last Modified: Tue, 17 Aug 2021 09:43:02 GMT  
		Size: 10.6 MB (10572088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:145f85437ade6ab27652a447c637dcc1efd6d627d69571e89a9a30de68e9ca31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65302676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfd861564ad7af9f83d87f0b53feb3deea7080ddbfaed0678f2fc99c2b942ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:17:03 GMT
ADD file:75b6eb36a0ba8612cac405c278e0b6859f0857f284d7f2da3bc8ad6f4596cb7d in / 
# Tue, 17 Aug 2021 02:17:04 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:25:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:25:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:86a6508bfdcb208b57a6ef5ca954ff178d89a14ca7c65b27bcd68df01e915895`  
		Last Modified: Tue, 17 Aug 2021 02:34:04 GMT  
		Size: 50.1 MB (50148031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894d51adc3dd9d078687cb2de22546210c7c13da66ac22c2e59180e6c194ddb`  
		Last Modified: Tue, 17 Aug 2021 15:43:55 GMT  
		Size: 4.9 MB (4937133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c61d960a4bb6b195a3e18c7e848519224d78371f6f147c8385202bcdab4023`  
		Last Modified: Tue, 17 Aug 2021 15:43:57 GMT  
		Size: 10.2 MB (10217512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:95d6d67d8406fecd07f2ca47fb1c181429f99d8aa0fc2ea109f9f7e7ce9e9a1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69659445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da9d49ec2b2035e68d98fe9d85208d455692b9c1c6a998f4e214216593a3973`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:32 GMT
ADD file:2eb550b4dc61105505c60437af91d7300fc5596834bfce84a75b260663bf4f42 in / 
# Tue, 17 Aug 2021 01:47:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:55:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:55:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0c8e1604d5b38112a190afe29ac6b4d1c501651ae9e68b6eaa49788ae64f145d`  
		Last Modified: Tue, 17 Aug 2021 01:56:14 GMT  
		Size: 53.6 MB (53625965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4b3d12f8e0cac2ab78286575b8f56d2cadedcafd68908cc60821856f5e360`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 5.2 MB (5160051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb41ce34a000fbba6dafcb340db9d0b7f64a8efd27ff966f77978ddd2c567439`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 10.9 MB (10873429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1fff776b370dd15d9693f26b99eb5780cdcdb3bb8e65edd38597f03b4e64d758
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72519728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddda0428d54281258d8a03082810ed4c348538dc58305c7e6a3471f26fe2df0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:42 GMT
ADD file:8d9eb4b2afc4eb0058f4080c5f0eedf0ddef323f1cc5a0403658254d191f117e in / 
# Tue, 17 Aug 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:02:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:79e62a40ce7bfbbe436e33c1da1c5661386b9674fe81402fdbfbb42a5b84998b`  
		Last Modified: Tue, 17 Aug 2021 01:52:55 GMT  
		Size: 56.0 MB (55967475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3391f9add930caab1f7ad8d326db740aab914960a3522b2baea8f34b06d23`  
		Last Modified: Tue, 17 Aug 2021 02:11:30 GMT  
		Size: 5.3 MB (5301763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c1c03bbd7c2f8c23dd8b5a8bae89de98d00fe400f6f7c89140aed7a78c6aa7`  
		Last Modified: Tue, 17 Aug 2021 02:11:31 GMT  
		Size: 11.3 MB (11250490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:98d7bad65228d9092b100017daa4d05eac8019a3dbe623a4adefe8f9373977f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69203513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a36a3cbc335f2339b81ecd932608bf269d960941ef345fb150a652c913e776be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:13:43 GMT
ADD file:a77aad2a2ac623e0a0640ce1caa07dc2982875f5e01f2baec92d08795be4ad93 in / 
# Tue, 17 Aug 2021 01:13:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e190daae609fdf78d1dc3b15955b491e5dba465be6fc9a8a7ffc7a7039ffccd6`  
		Last Modified: Tue, 17 Aug 2021 01:23:46 GMT  
		Size: 53.2 MB (53198954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86d281139f06d0443f660a40811f7a489e4a83c078e49d5b8f57195e98409cf`  
		Last Modified: Tue, 17 Aug 2021 21:00:30 GMT  
		Size: 5.1 MB (5131004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99713d0cdbd7eef9bc879aca6d384c6712d27d4af1616629bada8c72f448a620`  
		Last Modified: Tue, 17 Aug 2021 21:00:33 GMT  
		Size: 10.9 MB (10873555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4f884fa29acd285b5b2771d8cc4bce5275b8afc32f27f4bd75703664d0fc3a10
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75903789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f518063b21791802c1bda67dbdbcc4e0499960cdc1d888f032263ba4920d1e48`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:35:46 GMT
ADD file:3bdf0f06854c7b6578701900c267a6a5a712e84cc267d519df82eb28d568221c in / 
# Tue, 17 Aug 2021 01:35:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:24:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:26:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d596d5bddf4c6763b1156eb07675e21eb75a9b5bc9e5629b035d92244696d704`  
		Last Modified: Tue, 17 Aug 2021 01:52:09 GMT  
		Size: 58.9 MB (58855169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3055c003e2e867f5f7baa6505d799eff17441266441133ae556e40de99b75429`  
		Last Modified: Tue, 17 Aug 2021 16:10:29 GMT  
		Size: 5.4 MB (5421863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a281bbbade77271f6acd86003d63e414b000f703adebe3ff4c838ab7244b2c`  
		Last Modified: Tue, 17 Aug 2021 16:10:31 GMT  
		Size: 11.6 MB (11626757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ea1ea7eb3f215c84403554672c91c22945344400c673d6f1522fd607ee45c612
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65716534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7bd69c97313ca7d402f43854f393547d6854ae7a3b046c650dadf00adab219`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:57 GMT
ADD file:17c3a69ac6b2ac905f0d9d5d8d828215848c91b6aca208c63e3c8c6c3c28ac20 in / 
# Tue, 17 Aug 2021 01:45:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:29:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:03abe71e39e08cd630ff168b11929dc5c3c5111cfb3d81f5a8183f7ba7162fab`  
		Last Modified: Tue, 17 Aug 2021 02:01:48 GMT  
		Size: 50.4 MB (50437771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e3ddf2aa723d9dc92fc071b3cc373219cd68de4072a024dc13965f2156705`  
		Last Modified: Tue, 17 Aug 2021 03:07:39 GMT  
		Size: 5.0 MB (4984859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbcb287940d650490755774d53a8edf26fba9558538160b4f649b66979ee4d`  
		Last Modified: Tue, 17 Aug 2021 03:07:43 GMT  
		Size: 10.3 MB (10293904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fab97181f913819d52d80648d12308e39e2b6edf93eed0dd25b6269b1e975638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69143422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b34924373ab74ba0650cd2931dacfef322ec14458f9202a4078c99c5f43650a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:51:06 GMT
ADD file:ab809bd14c40234cf29151f2485ed39a9fa31f67c202abe6bf8546f5899aa52f in / 
# Tue, 17 Aug 2021 01:51:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:37:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6758b3369d7c595105d273788911a60f3cbd8b26d39dea406c75de4d1da4a084`  
		Last Modified: Tue, 17 Aug 2021 01:59:02 GMT  
		Size: 53.2 MB (53226590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee5f5767e372ec2c62434ed4325aa1b14846b20d736bdb81e1861163803d98`  
		Last Modified: Tue, 17 Aug 2021 07:45:09 GMT  
		Size: 5.2 MB (5152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1daed3fa6142f9fe36fd70a1e631c71aa839f077885d60cb4e7fb21210dacc`  
		Last Modified: Tue, 17 Aug 2021 07:45:10 GMT  
		Size: 10.8 MB (10763976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:fc2b7d4525cb2656724b5da8e1e3a32b60ed1578e93a940fc4f9c1ed52bcb907
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4ce0505fd2f716a12637bce8cb2ea04b1f403f5bc10c794f0e11ee9e9ccd677d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126428830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d233be97a8804fc816ed0a4d036f84b04e91f53dab70bf7cbbfb72d15d81f11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:06 GMT
ADD file:3052ec53a19fa26baad5d50e4d2867be2cc386ae62195d8dbb9d90d0b904c464 in / 
# Tue, 17 Aug 2021 01:25:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6952a6bd46e0eaa2c0e7e851a45f288b3dc080472a9249e48c74b3fb7551fcc`  
		Last Modified: Tue, 17 Aug 2021 01:31:55 GMT  
		Size: 54.9 MB (54930846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ac09fd3cc15f0b26d3a8005c31390d5de204431a0355ffc55e60a6a8f3b25`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 5.2 MB (5171335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e5aaa7713c8cc3d2dd4d36732e1aac9d876c81ddc49221a0d413f2d4f7dcb1`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 10.9 MB (10872817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11986d12d3ac34fc246feb151c1fbc9cdf5db866e53edb07c12fcda5e91e187a`  
		Last Modified: Tue, 17 Aug 2021 09:32:14 GMT  
		Size: 55.5 MB (55453832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fc195efcaabeee27dd247ca281492315d995b9c123f7b6c168f62205c525c681
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121304601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ff593b6ceaeb3e7dfb6e363517c76c7d27441894855740c03e86f759bb782b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:59:08 GMT
ADD file:f9ad3ec0db7a58cdae9cae8207122785d2b8c116c5bb4d47d46f530bda897397 in / 
# Tue, 17 Aug 2021 01:59:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:26:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:27:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f84c96ba3e58d3cff4f87a969dd91565bb9be34588bf76d1a5a253c40ee1139`  
		Last Modified: Tue, 17 Aug 2021 02:16:06 GMT  
		Size: 52.5 MB (52493950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97b83ef80c1b594046817ebd2be34eaa8faee56f4463a801453d7757341208b`  
		Last Modified: Tue, 17 Aug 2021 09:42:59 GMT  
		Size: 5.1 MB (5075615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c50a77e6ef78b9b162607f1afc018b1b92ec1874e815ace7ce3c948fe8c8ea`  
		Last Modified: Tue, 17 Aug 2021 09:43:02 GMT  
		Size: 10.6 MB (10572088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c2bac917a1fcd804dd397408311320a680c743c2e90437422491a062c16b37`  
		Last Modified: Tue, 17 Aug 2021 09:43:52 GMT  
		Size: 53.2 MB (53162948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:614f5e84242acb4f77da6c4f20e61e8935fa7023f4de2f109e253786245f81aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116416369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67104fbe683be478e692224d7dbbf566952954f8cd25ca554a571e912d140d67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:17:03 GMT
ADD file:75b6eb36a0ba8612cac405c278e0b6859f0857f284d7f2da3bc8ad6f4596cb7d in / 
# Tue, 17 Aug 2021 02:17:04 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:25:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:25:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:26:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86a6508bfdcb208b57a6ef5ca954ff178d89a14ca7c65b27bcd68df01e915895`  
		Last Modified: Tue, 17 Aug 2021 02:34:04 GMT  
		Size: 50.1 MB (50148031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894d51adc3dd9d078687cb2de22546210c7c13da66ac22c2e59180e6c194ddb`  
		Last Modified: Tue, 17 Aug 2021 15:43:55 GMT  
		Size: 4.9 MB (4937133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c61d960a4bb6b195a3e18c7e848519224d78371f6f147c8385202bcdab4023`  
		Last Modified: Tue, 17 Aug 2021 15:43:57 GMT  
		Size: 10.2 MB (10217512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cacd13952822a4eee5f0a451c9ca9324612dfe962c2c8f6c1e5ad8ec953c3c`  
		Last Modified: Tue, 17 Aug 2021 15:44:48 GMT  
		Size: 51.1 MB (51113693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37bee1487624fd84c180d6b30ee44482d1ae1d363ae4312e0ae72e29742d84e8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125073913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3efdbbeaeb82295134826aa702e6298a62dd1936103e9b1f058056bf4a1721af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:32 GMT
ADD file:2eb550b4dc61105505c60437af91d7300fc5596834bfce84a75b260663bf4f42 in / 
# Tue, 17 Aug 2021 01:47:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:55:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:55:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:55:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c8e1604d5b38112a190afe29ac6b4d1c501651ae9e68b6eaa49788ae64f145d`  
		Last Modified: Tue, 17 Aug 2021 01:56:14 GMT  
		Size: 53.6 MB (53625965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4b3d12f8e0cac2ab78286575b8f56d2cadedcafd68908cc60821856f5e360`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 5.2 MB (5160051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb41ce34a000fbba6dafcb340db9d0b7f64a8efd27ff966f77978ddd2c567439`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 10.9 MB (10873429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7ff3790681e7d2217b96a8b89bdf6b99ab28fa3c7c0da0c88118fa977a7ce9`  
		Last Modified: Tue, 17 Aug 2021 08:03:58 GMT  
		Size: 55.4 MB (55414468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:04e0650bc727dd18f73c095ef5f35e238acfdbc963764c86f55dbd57a2817916
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129204520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3ac461708875960f1d5e7c484c1b60c5867b04bbdbb89494195e2999ae5c74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:42 GMT
ADD file:8d9eb4b2afc4eb0058f4080c5f0eedf0ddef323f1cc5a0403658254d191f117e in / 
# Tue, 17 Aug 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:02:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:79e62a40ce7bfbbe436e33c1da1c5661386b9674fe81402fdbfbb42a5b84998b`  
		Last Modified: Tue, 17 Aug 2021 01:52:55 GMT  
		Size: 56.0 MB (55967475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3391f9add930caab1f7ad8d326db740aab914960a3522b2baea8f34b06d23`  
		Last Modified: Tue, 17 Aug 2021 02:11:30 GMT  
		Size: 5.3 MB (5301763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c1c03bbd7c2f8c23dd8b5a8bae89de98d00fe400f6f7c89140aed7a78c6aa7`  
		Last Modified: Tue, 17 Aug 2021 02:11:31 GMT  
		Size: 11.3 MB (11250490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71047ae47f0ad2d0279c1731200ffbae15c68839f662197eb53927e89f4a346a`  
		Last Modified: Tue, 17 Aug 2021 02:11:56 GMT  
		Size: 56.7 MB (56684792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c1f36d5b0b0dcee92a157a00014bb120bf3e0526c31c561fddf31d9be0c0b241
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123467584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a236cbbfbe37dcf11589dcef6062492f943e44179a009ba1665e0fcb1a4e1af7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:13:43 GMT
ADD file:a77aad2a2ac623e0a0640ce1caa07dc2982875f5e01f2baec92d08795be4ad93 in / 
# Tue, 17 Aug 2021 01:13:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:51:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e190daae609fdf78d1dc3b15955b491e5dba465be6fc9a8a7ffc7a7039ffccd6`  
		Last Modified: Tue, 17 Aug 2021 01:23:46 GMT  
		Size: 53.2 MB (53198954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86d281139f06d0443f660a40811f7a489e4a83c078e49d5b8f57195e98409cf`  
		Last Modified: Tue, 17 Aug 2021 21:00:30 GMT  
		Size: 5.1 MB (5131004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99713d0cdbd7eef9bc879aca6d384c6712d27d4af1616629bada8c72f448a620`  
		Last Modified: Tue, 17 Aug 2021 21:00:33 GMT  
		Size: 10.9 MB (10873555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa119cf8ddcc3e8e9ab5ccb513faee61d808d3ca9cfb4d4ef9d68386a6848f`  
		Last Modified: Tue, 17 Aug 2021 21:01:23 GMT  
		Size: 54.3 MB (54264071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bdaf74ed5eb85a64320a1879fd8cb3fbc0b25ac5c31d2c487285f9490290ee94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135787107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2446242db75bbe280501c39a5d487742a2b9189f01a6865da572325bd1a7a878`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:35:46 GMT
ADD file:3bdf0f06854c7b6578701900c267a6a5a712e84cc267d519df82eb28d568221c in / 
# Tue, 17 Aug 2021 01:35:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:24:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:26:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d596d5bddf4c6763b1156eb07675e21eb75a9b5bc9e5629b035d92244696d704`  
		Last Modified: Tue, 17 Aug 2021 01:52:09 GMT  
		Size: 58.9 MB (58855169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3055c003e2e867f5f7baa6505d799eff17441266441133ae556e40de99b75429`  
		Last Modified: Tue, 17 Aug 2021 16:10:29 GMT  
		Size: 5.4 MB (5421863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a281bbbade77271f6acd86003d63e414b000f703adebe3ff4c838ab7244b2c`  
		Last Modified: Tue, 17 Aug 2021 16:10:31 GMT  
		Size: 11.6 MB (11626757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d86af2c2f0d04abf574423e9d1d5c3771093d278c3c65bcb999fee07604f643`  
		Last Modified: Tue, 17 Aug 2021 16:12:29 GMT  
		Size: 59.9 MB (59883318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8105fd441cbd36f7bde58e34b24e9329d34e31d2c7e2592edbd60d5ac0d77efd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117103758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27c68b1a73365a21c15885cd64ba01cc9fbb3f9160c6787ce5b37cdaa3cb6a9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:57 GMT
ADD file:17c3a69ac6b2ac905f0d9d5d8d828215848c91b6aca208c63e3c8c6c3c28ac20 in / 
# Tue, 17 Aug 2021 01:45:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:29:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:33:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03abe71e39e08cd630ff168b11929dc5c3c5111cfb3d81f5a8183f7ba7162fab`  
		Last Modified: Tue, 17 Aug 2021 02:01:48 GMT  
		Size: 50.4 MB (50437771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e3ddf2aa723d9dc92fc071b3cc373219cd68de4072a024dc13965f2156705`  
		Last Modified: Tue, 17 Aug 2021 03:07:39 GMT  
		Size: 5.0 MB (4984859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbcb287940d650490755774d53a8edf26fba9558538160b4f649b66979ee4d`  
		Last Modified: Tue, 17 Aug 2021 03:07:43 GMT  
		Size: 10.3 MB (10293904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecda3ed528238bab9bf59ea2bc04887f931df81d6afd6768a21f6cb99a711637`  
		Last Modified: Tue, 17 Aug 2021 03:09:51 GMT  
		Size: 51.4 MB (51387224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:508193ae57b397427a2d0c356c071845bd3d17f174589d82e138df64ec7e90bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123868303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7f4f7bd222e4b52b7b76ccd1407623917c762cf5daa6d1d6646c1c65968e00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:51:06 GMT
ADD file:ab809bd14c40234cf29151f2485ed39a9fa31f67c202abe6bf8546f5899aa52f in / 
# Tue, 17 Aug 2021 01:51:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:37:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6758b3369d7c595105d273788911a60f3cbd8b26d39dea406c75de4d1da4a084`  
		Last Modified: Tue, 17 Aug 2021 01:59:02 GMT  
		Size: 53.2 MB (53226590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee5f5767e372ec2c62434ed4325aa1b14846b20d736bdb81e1861163803d98`  
		Last Modified: Tue, 17 Aug 2021 07:45:09 GMT  
		Size: 5.2 MB (5152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1daed3fa6142f9fe36fd70a1e631c71aa839f077885d60cb4e7fb21210dacc`  
		Last Modified: Tue, 17 Aug 2021 07:45:10 GMT  
		Size: 10.8 MB (10763976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52078ebb293da4fc08dd7b04c3124715e75d72e8d33e91bcdaf326bcad28bdb`  
		Last Modified: Tue, 17 Aug 2021 07:45:26 GMT  
		Size: 54.7 MB (54724881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:f84b3ee2dd5104bbb1d77aae6a898d8f1e2a7fa0af22f175b7550ec17ba09df1
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

### `buildpack-deps:stable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cafaa221feb7c182ed3c3f83f0086da57bc7156c30159366155c5897a86d915b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (321951029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe8fece98de2233a5a26a59d08ff969b8b55b7fbc1a1c6e7ceb6b22ec659b884`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf565088aae3ef2159885f29853bce88eb16082b0c98fcacd08fc9008c84b9`  
		Last Modified: Tue, 17 Aug 2021 09:29:09 GMT  
		Size: 5.2 MB (5153283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c0dd0dc0d3d367cc5b85f86d8881afb658e8eb341a86daf3835c2f14159ac`  
		Last Modified: Tue, 17 Aug 2021 09:29:10 GMT  
		Size: 10.9 MB (10871829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf06daf65610482c638dcc63479a8281e667e37f7842219d66f2dedf63718f4`  
		Last Modified: Tue, 17 Aug 2021 09:29:34 GMT  
		Size: 54.6 MB (54565734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942374d5c11438b68e78d44b36c9eac8fe0a2570c33681d7263b0f3f069c06b9`  
		Last Modified: Tue, 17 Aug 2021 09:30:21 GMT  
		Size: 196.4 MB (196445179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b9c95648c1c4f6bc00721365da71edf685136b260eb2cc57266229470473ce2c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.0 MB (295049846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c41fc84b081c31c9c20ab9f272e38b3482520d7acbd98f04ae0efeaecc5abf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:18:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:21:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b0b6b82f848e8ef423a421d5d46194f7787ebf23e3dcc69fb177eb4dc49f6`  
		Last Modified: Tue, 17 Aug 2021 09:36:54 GMT  
		Size: 5.1 MB (5063684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02ecba39f2b03f1bc47ed6ba17c15a62b11e7eb2ae7397ba374851a864efc67`  
		Last Modified: Tue, 17 Aug 2021 09:36:55 GMT  
		Size: 10.6 MB (10570968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f083cd711c027bf75e496fb0a9b4e8e2ac1a102c5fc0d01c3375757fc102a526`  
		Last Modified: Tue, 17 Aug 2021 09:37:46 GMT  
		Size: 52.3 MB (52319253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c87f1282078740238a813920e2dab455ea24e91c18b10b6e89bfc34d3dabe5`  
		Last Modified: Tue, 17 Aug 2021 09:39:41 GMT  
		Size: 174.6 MB (174643701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:20a100f794f73d9565aeb095033cbd7d03958c4f5cace47051a44b242b46e4e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282478824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648d40b55ba7c2d96aacdb0170baba32efd26ffb7e7e26cb74e8422a52c6fdce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:12:37 GMT
ADD file:579ac9b41923db9165f333faac1330f2924a14f90cab7605ffd66c1815249adf in / 
# Tue, 17 Aug 2021 02:12:38 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:20:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1ce31b8c318c8eac9eba15cdf329f397a64952ab575a09c167fc9ddc5a991a98`  
		Last Modified: Tue, 17 Aug 2021 02:28:44 GMT  
		Size: 50.1 MB (50118546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5a38f951962ad43cfef6137e6638004e3a3f066bb26e2c3b52489258a4b5c`  
		Last Modified: Tue, 17 Aug 2021 15:38:06 GMT  
		Size: 4.9 MB (4922570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a545de7dcb8f9fe8fd65b3b1f104abbb20cee600bc8602beef63ccc4f6259`  
		Last Modified: Tue, 17 Aug 2021 15:38:08 GMT  
		Size: 10.2 MB (10216795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0801bbb4cc34f3ceed00d5e57c23d39f3f1763075f34e2b90a80f078ae6d486a`  
		Last Modified: Tue, 17 Aug 2021 15:38:59 GMT  
		Size: 50.3 MB (50328392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3d7c49ff6810d965ef9be32d59d7da22bf3dd967c4d1f3b3414a7aed7b5ed9`  
		Last Modified: Tue, 17 Aug 2021 15:40:48 GMT  
		Size: 166.9 MB (166892521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c5716ed801cb5ff800dbe3f9364795dc7bbbb0bcea2c08b0b00a0a9def980c69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313622714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787980177678b9ae90f4b44fc98c5baf6b6e494714c2a083736d7ed49fed43db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:52:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:52:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495d06e79f81fe42766bacea59684f27db9d24960b6dd7efeea81f48820d0f6`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 5.1 MB (5142588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd18a2d3ce3a400515ed7a845aeb9d8cd17b023f1efe77ff81292bd63addcc0`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 10.9 MB (10872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfd3a44e1c9b9d3df6b60162d29469b5fe3aaddecba7bf2b122ced08e2a848`  
		Last Modified: Tue, 17 Aug 2021 08:01:25 GMT  
		Size: 54.7 MB (54670308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e87d255e4f38e1f000f523e71beef3ea90c78d187cbca6373c8bcdc15dab325`  
		Last Modified: Tue, 17 Aug 2021 08:02:07 GMT  
		Size: 189.3 MB (189336134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

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

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e56dff8e57c911a088985665f4838cb934b32307330794016163f6bc43f101c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301388823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0407593e24bc9c23a80aec36f20f500b78d2e8635f06aecd1e722db0bc94edf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:42:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:45:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d42212351d464cda967a0b9462fdbf31cf8b926ec739f94ca92a04924b59b44`  
		Last Modified: Tue, 17 Aug 2021 20:53:57 GMT  
		Size: 5.1 MB (5114876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f443b77bd62cad6049ac9b935c37714988629b9b90804c902ebf5d94db0947`  
		Last Modified: Tue, 17 Aug 2021 20:53:59 GMT  
		Size: 10.9 MB (10873298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f994e51a722336aa2b759033a359755271ce92b5d1948340ac2760bd28d90a8`  
		Last Modified: Tue, 17 Aug 2021 20:54:52 GMT  
		Size: 53.3 MB (53297838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb32760aefab4b67e850394277f734a5e65f8191fb6c3dd5e43b4c1577e4c61`  
		Last Modified: Tue, 17 Aug 2021 20:57:03 GMT  
		Size: 178.9 MB (178935476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3035d395cdd02846678666bf0e6fdbafe0fcc72f36134d4cc968c3fc48667386
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330493921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d3e26c8948f38abc9f03d8319b316eb0204deca02aa44662b8ef9338ec5ed0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 14:34:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:53:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f9b82c933b317ed127f45e6f56d6d7508514459e0ef09073b467d3dd8425e`  
		Last Modified: Tue, 17 Aug 2021 15:58:19 GMT  
		Size: 5.4 MB (5401864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a6114ee4fe00702ca86cd44f229643d9324c4b202ed6583f35d2eca848a4a`  
		Last Modified: Tue, 17 Aug 2021 15:58:18 GMT  
		Size: 11.6 MB (11626128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e91c7e9879fdf8ce8ef16f2ba105dac2bc4d76888c86b7b5c63973c05f7ed4`  
		Last Modified: Tue, 17 Aug 2021 16:00:07 GMT  
		Size: 58.8 MB (58849860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8542edff3433d9f519b8030bb7b7f200e5cec504915eda9435d627020680c`  
		Last Modified: Tue, 17 Aug 2021 16:04:00 GMT  
		Size: 195.8 MB (195800037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8b7e5e3f28327cce774548f9e1559535aacb731aa486537b0b1c5458c81caddf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295572826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:186802d3daef183bcf0a403c0ce38346f8c731d225920fe8893adc7c58b07151`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:32:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:32:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20bd918649e02578e4e6f19a2c873dbcc6da7009f7b4ee3088a3e2f594fe6e`  
		Last Modified: Tue, 17 Aug 2021 07:43:16 GMT  
		Size: 5.1 MB (5137099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e43baff5e6307dfe51df170140aa3c7c4b7a4cb3fb03b3a2255a8038c9542`  
		Last Modified: Tue, 17 Aug 2021 07:43:17 GMT  
		Size: 10.8 MB (10761504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163c4ba4cbac76aa2dccf627dc69a5f47c32176dc12e23d0bbbfaa6723a446`  
		Last Modified: Tue, 17 Aug 2021 07:43:35 GMT  
		Size: 54.1 MB (54050153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc89d77adebd4b8848cee8bc0ed80f335c59bbc0b93c29b608cef22175243fe`  
		Last Modified: Tue, 17 Aug 2021 07:44:05 GMT  
		Size: 172.4 MB (172430038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:fdd2452507132b7a4c6b432c32e159f15d955afa4258e5b8f64b7fdc7add487f
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

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f2aebefdccca99d265c8e84738ee9f99c36f4212ca051d43b4683798dfb42636
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70940116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6fe7405525d60b20905a08baa979b62312fdb03b9a48e235baebfc59977f2c2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf565088aae3ef2159885f29853bce88eb16082b0c98fcacd08fc9008c84b9`  
		Last Modified: Tue, 17 Aug 2021 09:29:09 GMT  
		Size: 5.2 MB (5153283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c0dd0dc0d3d367cc5b85f86d8881afb658e8eb341a86daf3835c2f14159ac`  
		Last Modified: Tue, 17 Aug 2021 09:29:10 GMT  
		Size: 10.9 MB (10871829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b2e1e86e8147e79ba83867e74aa1a9fa3b677f764ef0a9d7e3cae46c5ad2669d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68086892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c4086386b6b216789ae1d7d834ccfd24e3cae7f8d6d9f2d9dfa493924d3cc3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:18:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b0b6b82f848e8ef423a421d5d46194f7787ebf23e3dcc69fb177eb4dc49f6`  
		Last Modified: Tue, 17 Aug 2021 09:36:54 GMT  
		Size: 5.1 MB (5063684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02ecba39f2b03f1bc47ed6ba17c15a62b11e7eb2ae7397ba374851a864efc67`  
		Last Modified: Tue, 17 Aug 2021 09:36:55 GMT  
		Size: 10.6 MB (10570968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:65059ed8ae5f1dcdde3da0bb274969b7cca178755ccd40eee90ae54fde9e89fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65257911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c4021355832ed254e558058a0774730787867c0d43269189b5abea64f2fe0b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:12:37 GMT
ADD file:579ac9b41923db9165f333faac1330f2924a14f90cab7605ffd66c1815249adf in / 
# Tue, 17 Aug 2021 02:12:38 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1ce31b8c318c8eac9eba15cdf329f397a64952ab575a09c167fc9ddc5a991a98`  
		Last Modified: Tue, 17 Aug 2021 02:28:44 GMT  
		Size: 50.1 MB (50118546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5a38f951962ad43cfef6137e6638004e3a3f066bb26e2c3b52489258a4b5c`  
		Last Modified: Tue, 17 Aug 2021 15:38:06 GMT  
		Size: 4.9 MB (4922570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a545de7dcb8f9fe8fd65b3b1f104abbb20cee600bc8602beef63ccc4f6259`  
		Last Modified: Tue, 17 Aug 2021 15:38:08 GMT  
		Size: 10.2 MB (10216795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fe66fbc885d81fdafbe18713a6165c8028b9ed9939b65497ab53bdf98e963213
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69616272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48afe04239a66261d25a64f298c4fa2467895f8861bcf70bcc11a0248523fb5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:52:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:52:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495d06e79f81fe42766bacea59684f27db9d24960b6dd7efeea81f48820d0f6`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 5.1 MB (5142588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd18a2d3ce3a400515ed7a845aeb9d8cd17b023f1efe77ff81292bd63addcc0`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 10.9 MB (10872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e593b0b7e666a4ee388aec91360e9d8414ec6b6846bab3c97d2fad8f754445d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72456123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f08f2eeb7d00459ae8f10b008928c02a6c5ad7cbd65e4e0ab0ead6da5ba4b05c`
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

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5617c8a692ae2f2d66e61c9353dd8f51a5584d8d3bc9247c10af1c8ed8b9fa49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69155509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efea973f65ee025f05845863859e9962cff13e166db36866230ec2619834163e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d42212351d464cda967a0b9462fdbf31cf8b926ec739f94ca92a04924b59b44`  
		Last Modified: Tue, 17 Aug 2021 20:53:57 GMT  
		Size: 5.1 MB (5114876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f443b77bd62cad6049ac9b935c37714988629b9b90804c902ebf5d94db0947`  
		Last Modified: Tue, 17 Aug 2021 20:53:59 GMT  
		Size: 10.9 MB (10873298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7c55dd439b7bc0da37bc1d85c237a140966ff47444714b599ceb42724bb68232
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75844024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c6a017b4350c90fd80678152fdf7e17a772a4b8585ddad57bdb2cb34e56a59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f9b82c933b317ed127f45e6f56d6d7508514459e0ef09073b467d3dd8425e`  
		Last Modified: Tue, 17 Aug 2021 15:58:19 GMT  
		Size: 5.4 MB (5401864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a6114ee4fe00702ca86cd44f229643d9324c4b202ed6583f35d2eca848a4a`  
		Last Modified: Tue, 17 Aug 2021 15:58:18 GMT  
		Size: 11.6 MB (11626128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:86da00cec8807a6fca2c5dc68ebe2887651da5b291cee956ee1b61e0a2ec85d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69092635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1b1429c9e37360be6c7c7fb3e2850f6c59962e4669641fdc1cbb2dfe99a8241`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:32:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20bd918649e02578e4e6f19a2c873dbcc6da7009f7b4ee3088a3e2f594fe6e`  
		Last Modified: Tue, 17 Aug 2021 07:43:16 GMT  
		Size: 5.1 MB (5137099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e43baff5e6307dfe51df170140aa3c7c4b7a4cb3fb03b3a2255a8038c9542`  
		Last Modified: Tue, 17 Aug 2021 07:43:17 GMT  
		Size: 10.8 MB (10761504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:7c9700c28be70bfd3bae7ec1bca0be928e089a0dabeac1547d9d01821dc1137e
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

### `buildpack-deps:stable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fcf696e81fbb39515e31895fbeedb08b0bf07e1bc8bfac1094b1f4adfebad8e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125505850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f8c023a59a00085d55f58463800a73350f5a479bc85bd8fec65c6d63c59b9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:26 GMT
ADD file:a528c112b566e7f129178dadedfa421b0c5b870997c4628327967850e54b915c in / 
# Tue, 17 Aug 2021 01:23:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:19:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c25b3090c2685271afcffc2a4db73f15ab11a0124bfcde6085c934a4e6f4a51`  
		Last Modified: Tue, 17 Aug 2021 01:29:06 GMT  
		Size: 54.9 MB (54915004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf565088aae3ef2159885f29853bce88eb16082b0c98fcacd08fc9008c84b9`  
		Last Modified: Tue, 17 Aug 2021 09:29:09 GMT  
		Size: 5.2 MB (5153283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c0dd0dc0d3d367cc5b85f86d8881afb658e8eb341a86daf3835c2f14159ac`  
		Last Modified: Tue, 17 Aug 2021 09:29:10 GMT  
		Size: 10.9 MB (10871829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf06daf65610482c638dcc63479a8281e667e37f7842219d66f2dedf63718f4`  
		Last Modified: Tue, 17 Aug 2021 09:29:34 GMT  
		Size: 54.6 MB (54565734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f4f9aaf82aa16a66de2601280af242b6eed140501fdefc27dbddaee1a2abd04d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120406145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7f7ffa4516f21995c9d82c55032542d253b9c19f3e8a3c7a5a351e3f28904bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:14 GMT
ADD file:7a83f4345de2023aecfd9fd02a04f76c6dddfdfec51caee0a04f0ad7b2144029 in / 
# Tue, 17 Aug 2021 01:55:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:18:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:19:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb7926e14f672d57d0e93564148e3a6ec9f8c5d47c68edca8eb69b1dd5f5972f`  
		Last Modified: Tue, 17 Aug 2021 02:10:17 GMT  
		Size: 52.5 MB (52452240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b0b6b82f848e8ef423a421d5d46194f7787ebf23e3dcc69fb177eb4dc49f6`  
		Last Modified: Tue, 17 Aug 2021 09:36:54 GMT  
		Size: 5.1 MB (5063684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02ecba39f2b03f1bc47ed6ba17c15a62b11e7eb2ae7397ba374851a864efc67`  
		Last Modified: Tue, 17 Aug 2021 09:36:55 GMT  
		Size: 10.6 MB (10570968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f083cd711c027bf75e496fb0a9b4e8e2ac1a102c5fc0d01c3375757fc102a526`  
		Last Modified: Tue, 17 Aug 2021 09:37:46 GMT  
		Size: 52.3 MB (52319253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:952205bc7cddbbfb9fa8d02a6b6359b25693f6c583577f30ae38f6fc953128d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115586303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67953dbcbb8bcfebe0afc9db6d95f9f661b8a7f422c688642a536fd858e9d5a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:12:37 GMT
ADD file:579ac9b41923db9165f333faac1330f2924a14f90cab7605ffd66c1815249adf in / 
# Tue, 17 Aug 2021 02:12:38 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1ce31b8c318c8eac9eba15cdf329f397a64952ab575a09c167fc9ddc5a991a98`  
		Last Modified: Tue, 17 Aug 2021 02:28:44 GMT  
		Size: 50.1 MB (50118546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5a38f951962ad43cfef6137e6638004e3a3f066bb26e2c3b52489258a4b5c`  
		Last Modified: Tue, 17 Aug 2021 15:38:06 GMT  
		Size: 4.9 MB (4922570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a545de7dcb8f9fe8fd65b3b1f104abbb20cee600bc8602beef63ccc4f6259`  
		Last Modified: Tue, 17 Aug 2021 15:38:08 GMT  
		Size: 10.2 MB (10216795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0801bbb4cc34f3ceed00d5e57c23d39f3f1763075f34e2b90a80f078ae6d486a`  
		Last Modified: Tue, 17 Aug 2021 15:38:59 GMT  
		Size: 50.3 MB (50328392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7466552e59983c946898f07f77837b743f3b156ff789fc751ee98a02a9add3b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124286580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d51b8f3ab483064d973aecc62a3b04b730815b474f7f9793cd107f3f79f6dad2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:48 GMT
ADD file:1e52a0aa8f37622b3d0d73bddae98dd854cdd0b001fffe704eb833b2659413ec in / 
# Tue, 17 Aug 2021 01:45:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:52:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:52:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:52:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a5d73d4b7323ffb58a7d3baa48bf81bba71d259b96fbc5b838424f52d325a8a`  
		Last Modified: Tue, 17 Aug 2021 01:52:56 GMT  
		Size: 53.6 MB (53601013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495d06e79f81fe42766bacea59684f27db9d24960b6dd7efeea81f48820d0f6`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 5.1 MB (5142588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd18a2d3ce3a400515ed7a845aeb9d8cd17b023f1efe77ff81292bd63addcc0`  
		Last Modified: Tue, 17 Aug 2021 08:01:01 GMT  
		Size: 10.9 MB (10872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfd3a44e1c9b9d3df6b60162d29469b5fe3aaddecba7bf2b122ced08e2a848`  
		Last Modified: Tue, 17 Aug 2021 08:01:25 GMT  
		Size: 54.7 MB (54670308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:00be0f57bc7e719a20f1fa7c7544e0df9c6853fb707efac9b901c65b6c06ba5a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128372373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca098a2a0c1d25e4bb10cde9432093d0aa17de51005d3952d00ec8f1d6b262b2`
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

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:03f5904c242d11766ad5bf5183be9e7630b9e37d9670519c71a54b93a9c4d095
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122453347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63db1c68912deb8496753716857c5912bdf02ca2a4bad7229ef3b7bdeab044a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:07 GMT
ADD file:02211d64840f82348df6fadec1317a40ec119abf15381f1218e0b40b27073c32 in / 
# Tue, 17 Aug 2021 01:11:08 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:42:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10a39c0341c0177ba4782a91252884e299a2bdf04f77024e7d4275d957fdd83d`  
		Last Modified: Tue, 17 Aug 2021 01:19:35 GMT  
		Size: 53.2 MB (53167335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d42212351d464cda967a0b9462fdbf31cf8b926ec739f94ca92a04924b59b44`  
		Last Modified: Tue, 17 Aug 2021 20:53:57 GMT  
		Size: 5.1 MB (5114876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f443b77bd62cad6049ac9b935c37714988629b9b90804c902ebf5d94db0947`  
		Last Modified: Tue, 17 Aug 2021 20:53:59 GMT  
		Size: 10.9 MB (10873298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f994e51a722336aa2b759033a359755271ce92b5d1948340ac2760bd28d90a8`  
		Last Modified: Tue, 17 Aug 2021 20:54:52 GMT  
		Size: 53.3 MB (53297838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fcbc2251bc93c2efb3d7fba801d28ae0f31bcd293b3ba7c7a232d9dd37ba5578
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134693884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d90068795b93d0a5374de038dbf136ba1114dd082e28d5b649c0406f044c8fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:32:24 GMT
ADD file:99182c25a0a65904aac8094f31301f6c09a689865eacb67729ddd5f9d350068a in / 
# Tue, 17 Aug 2021 01:32:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 14:34:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81e441398542923e66b79e84b365735eb5092b8210bf61da038972187cb6883b`  
		Last Modified: Tue, 17 Aug 2021 01:44:58 GMT  
		Size: 58.8 MB (58816032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f9b82c933b317ed127f45e6f56d6d7508514459e0ef09073b467d3dd8425e`  
		Last Modified: Tue, 17 Aug 2021 15:58:19 GMT  
		Size: 5.4 MB (5401864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a6114ee4fe00702ca86cd44f229643d9324c4b202ed6583f35d2eca848a4a`  
		Last Modified: Tue, 17 Aug 2021 15:58:18 GMT  
		Size: 11.6 MB (11626128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e91c7e9879fdf8ce8ef16f2ba105dac2bc4d76888c86b7b5c63973c05f7ed4`  
		Last Modified: Tue, 17 Aug 2021 16:00:07 GMT  
		Size: 58.8 MB (58849860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5bae3f8d99ee48e52b19e9cd49f9ecfd1154979fb8ab49ec52a4f4d74ba5cdae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123142788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8878de09ccb0b4cf42119e9df2aaefcfc61cbfc3ce818b2f70133e76585d8413`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:31 GMT
ADD file:e474c3a08924b08926e175fe0a0a7e43dc15cae2e57293e15bff80c9a8f531f7 in / 
# Tue, 17 Aug 2021 01:48:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:32:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:32:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bd94e714496bf4e4164b0831f18dcd1d20351a4443b7a552c19b96d4e123f1f`  
		Last Modified: Tue, 17 Aug 2021 01:57:10 GMT  
		Size: 53.2 MB (53194032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c20bd918649e02578e4e6f19a2c873dbcc6da7009f7b4ee3088a3e2f594fe6e`  
		Last Modified: Tue, 17 Aug 2021 07:43:16 GMT  
		Size: 5.1 MB (5137099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e43baff5e6307dfe51df170140aa3c7c4b7a4cb3fb03b3a2255a8038c9542`  
		Last Modified: Tue, 17 Aug 2021 07:43:17 GMT  
		Size: 10.8 MB (10761504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163c4ba4cbac76aa2dccf627dc69a5f47c32176dc12e23d0bbbfaa6723a446`  
		Last Modified: Tue, 17 Aug 2021 07:43:35 GMT  
		Size: 54.1 MB (54050153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stretch`

```console
$ docker pull buildpack-deps@sha256:410405a7cb1b238dfef3c9c3f84a26187296e876b92117fa25bed3a015dd7c9e
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
$ docker pull buildpack-deps@sha256:c5429a40f146bf912c705c832cbc25389f3d2161675a42ce9e472082875b03df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309139494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:764861d75f807b284332aa3fa8c966915b39d39bee1b8d8f7254843d50630b01`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:00:50 GMT
ADD file:77054e1fc1091d0e0800f856514f36121a7b447fd1e2df32e6c8ff77e6136c66 in / 
# Tue, 17 Aug 2021 02:00:51 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:31:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:34:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfc6a97ccb61e1bee683ec639f55514bc40b09ef15dcd73c928632c03b3df06c`  
		Last Modified: Tue, 17 Aug 2021 02:18:40 GMT  
		Size: 44.1 MB (44091900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20f6698538a8926450e2bf8d1e9e1f5630637ea61c2b25c184a6a10a108b3e4`  
		Last Modified: Tue, 17 Aug 2021 09:46:08 GMT  
		Size: 10.4 MB (10350685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e83002ce3ccf92cb337a353e881e214497f7e55c7a28f556743242710dbd1a2`  
		Last Modified: Tue, 17 Aug 2021 09:46:04 GMT  
		Size: 4.2 MB (4161501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189296784b99bb4cb5b5de65a61b6597c48637dee4490557ff3e564713b772c3`  
		Last Modified: Tue, 17 Aug 2021 09:46:52 GMT  
		Size: 48.0 MB (47983610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec91ec6f66e8da219762222b74940c02cf181770578d198d2f2575e5efea404`  
		Last Modified: Tue, 17 Aug 2021 09:49:01 GMT  
		Size: 202.6 MB (202551798 bytes)  
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
$ docker pull buildpack-deps@sha256:730dd341c80f904d29a15532a89ac80632e9ec3ca37fb49b5a42598754088a9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332745158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afd95a9c0c53c01589fa6e35930e9b20d5c53bddf47bf357d81da909585990bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:05:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aca3d286261da95e058ae37c67e002a572b7dfc1dd7fe13d83060357489bfb`  
		Last Modified: Tue, 17 Aug 2021 02:13:06 GMT  
		Size: 11.4 MB (11353003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d22bbd8aeb7ef47c0fb18407f27411bd8008e1189b79f7c7c3dd1a6adfb7`  
		Last Modified: Tue, 17 Aug 2021 02:13:04 GMT  
		Size: 4.6 MB (4565010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f484f8f178f4bf3f3ec40912975a9e55159419f752b4683fcf11d9317be62c1e`  
		Last Modified: Tue, 17 Aug 2021 02:13:36 GMT  
		Size: 51.3 MB (51265260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686652807b46ef0616820485447143dc2d8fe496a532ae72c2cb0b508e67be60`  
		Last Modified: Tue, 17 Aug 2021 02:14:31 GMT  
		Size: 219.5 MB (219464665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stretch-curl`

```console
$ docker pull buildpack-deps@sha256:d02b7f64bfb73fd7bbef2ff4089d5b0a2835e8d81f40ce73e43f8f7fa7d2ca5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f97bd030bd9ca71861a61c9d6070bfa74a81b6f58afc51240259c4bf2e018f68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61018259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c9a62b63fb33454b389e17aea5f5abc09826bb499e30b9143971b9e6467a0b8`
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

### `buildpack-deps:stretch-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b9f641884fb639f0ddbf2004df2833d07b4df4eab88314b274fe24df4f908ef5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58604086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:901a010af7c0fd8d20a8ef29dadb26b7b9037aa7c3cba9aeb1814d3da18b96f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:00:50 GMT
ADD file:77054e1fc1091d0e0800f856514f36121a7b447fd1e2df32e6c8ff77e6136c66 in / 
# Tue, 17 Aug 2021 02:00:51 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bfc6a97ccb61e1bee683ec639f55514bc40b09ef15dcd73c928632c03b3df06c`  
		Last Modified: Tue, 17 Aug 2021 02:18:40 GMT  
		Size: 44.1 MB (44091900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20f6698538a8926450e2bf8d1e9e1f5630637ea61c2b25c184a6a10a108b3e4`  
		Last Modified: Tue, 17 Aug 2021 09:46:08 GMT  
		Size: 10.4 MB (10350685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e83002ce3ccf92cb337a353e881e214497f7e55c7a28f556743242710dbd1a2`  
		Last Modified: Tue, 17 Aug 2021 09:46:04 GMT  
		Size: 4.2 MB (4161501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f76ce59ad7abdbc8ff07ab0f91412a36027e076f2d87267e839c08e1493af6e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55992627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769c4c3f2e05b3ea5a1f34faae69d5935d3b3bf25b0502b3f51f66d9afab054f`
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

### `buildpack-deps:stretch-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a05e8a73f3ab8eaf3dde75a4f631ace100a433103b2934a0d1fb2aeecbde4e46
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57489982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f8de4cd39074ec0ba6be25bdc437074bc992a7d3e0218fd6957a741c90d203`
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

### `buildpack-deps:stretch-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:56da13ff13e95aaa610c01385585460016336f54817bf884dfb21e5a284f638a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62015233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d43094d7b883081dbd61e1705ac3e4c9e7e1f5efa1482eee7c698100937a53c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aca3d286261da95e058ae37c67e002a572b7dfc1dd7fe13d83060357489bfb`  
		Last Modified: Tue, 17 Aug 2021 02:13:06 GMT  
		Size: 11.4 MB (11353003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d22bbd8aeb7ef47c0fb18407f27411bd8008e1189b79f7c7c3dd1a6adfb7`  
		Last Modified: Tue, 17 Aug 2021 02:13:04 GMT  
		Size: 4.6 MB (4565010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:c44057c71fee67ac90a7d7de5c568a63909426c17c35d98a45163d43e7cb1ed4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c8cf20dfaed873ec2b57d437fd3dad180e5c25e3b5bcc2d71a9efa4f898f5a15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110779810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f4c42bb45b3d4146db1ca241675e7bc775392475e17e01f5a7ee3ee52a745a`
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

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cb17d66b3425c45df325e2afb076b919e45c5619b389d0d2199904827621f8fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106587696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a7559b36b89cca1b4c88a0013a833598818219be141088a68a2f242d0b5c764`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:00:50 GMT
ADD file:77054e1fc1091d0e0800f856514f36121a7b447fd1e2df32e6c8ff77e6136c66 in / 
# Tue, 17 Aug 2021 02:00:51 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:31:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfc6a97ccb61e1bee683ec639f55514bc40b09ef15dcd73c928632c03b3df06c`  
		Last Modified: Tue, 17 Aug 2021 02:18:40 GMT  
		Size: 44.1 MB (44091900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20f6698538a8926450e2bf8d1e9e1f5630637ea61c2b25c184a6a10a108b3e4`  
		Last Modified: Tue, 17 Aug 2021 09:46:08 GMT  
		Size: 10.4 MB (10350685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e83002ce3ccf92cb337a353e881e214497f7e55c7a28f556743242710dbd1a2`  
		Last Modified: Tue, 17 Aug 2021 09:46:04 GMT  
		Size: 4.2 MB (4161501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189296784b99bb4cb5b5de65a61b6597c48637dee4490557ff3e564713b772c3`  
		Last Modified: Tue, 17 Aug 2021 09:46:52 GMT  
		Size: 48.0 MB (47983610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b0d81bf2020711fddfc13427a5ddf6ff1622419cf1d7f0f7819d24c593843d3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102118784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecab1bcf19c083b34655482d0155cf67c9644e906e5b82ba0c7c75974937896`
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

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6f14f0285f97a25eb7caf7f31213bd1a506cfc18fb9f33146f2ba7e789369811
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105227228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5c63c662f33a6ebdeb59d7cbe0566b0c0ce06d5f2e8671067e1655c48a8075`
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

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a118e684aa2e428350e3fae74c09246820e7a5d41a92d1679f1f4139a06b633a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113280493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e61a364c0adae3b9b246c7e2afa1f6b0145b2424dc75da8e16f94a3701c7e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aca3d286261da95e058ae37c67e002a572b7dfc1dd7fe13d83060357489bfb`  
		Last Modified: Tue, 17 Aug 2021 02:13:06 GMT  
		Size: 11.4 MB (11353003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d22bbd8aeb7ef47c0fb18407f27411bd8008e1189b79f7c7c3dd1a6adfb7`  
		Last Modified: Tue, 17 Aug 2021 02:13:04 GMT  
		Size: 4.6 MB (4565010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f484f8f178f4bf3f3ec40912975a9e55159419f752b4683fcf11d9317be62c1e`  
		Last Modified: Tue, 17 Aug 2021 02:13:36 GMT  
		Size: 51.3 MB (51265260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:e4cfe790617d2ffabc8a963300bbb2f38bba6c162ac644150f7c4b3f17ca5556
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9164c1de3ee959d94d9a02a9b9fc381d9920f63439a879416e11babcb20c201c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.9 MB (323887742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47dd1f6893fa5d12feded97d9a2eaee1d1451d93d7941dd8cbf829d9cf976cd1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:06 GMT
ADD file:3052ec53a19fa26baad5d50e4d2867be2cc386ae62195d8dbb9d90d0b904c464 in / 
# Tue, 17 Aug 2021 01:25:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:24:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6952a6bd46e0eaa2c0e7e851a45f288b3dc080472a9249e48c74b3fb7551fcc`  
		Last Modified: Tue, 17 Aug 2021 01:31:55 GMT  
		Size: 54.9 MB (54930846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ac09fd3cc15f0b26d3a8005c31390d5de204431a0355ffc55e60a6a8f3b25`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 5.2 MB (5171335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e5aaa7713c8cc3d2dd4d36732e1aac9d876c81ddc49221a0d413f2d4f7dcb1`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 10.9 MB (10872817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11986d12d3ac34fc246feb151c1fbc9cdf5db866e53edb07c12fcda5e91e187a`  
		Last Modified: Tue, 17 Aug 2021 09:32:14 GMT  
		Size: 55.5 MB (55453832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f5ea41d022ec1a5a36111aa96cf323591a2da89a14eaff8b4a7daf934e07db`  
		Last Modified: Tue, 17 Aug 2021 09:32:59 GMT  
		Size: 197.5 MB (197458912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:698f3ba6ac57420b4376d98d74a3565525e5508f17abb7d81a864084630f893d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.7 MB (296739431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe4db913c27b633c7fceef07d6d7ed9cedd47c78761439492de9ccfc7b0c93be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:59:08 GMT
ADD file:f9ad3ec0db7a58cdae9cae8207122785d2b8c116c5bb4d47d46f530bda897397 in / 
# Tue, 17 Aug 2021 01:59:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:26:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:27:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:29:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f84c96ba3e58d3cff4f87a969dd91565bb9be34588bf76d1a5a253c40ee1139`  
		Last Modified: Tue, 17 Aug 2021 02:16:06 GMT  
		Size: 52.5 MB (52493950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97b83ef80c1b594046817ebd2be34eaa8faee56f4463a801453d7757341208b`  
		Last Modified: Tue, 17 Aug 2021 09:42:59 GMT  
		Size: 5.1 MB (5075615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c50a77e6ef78b9b162607f1afc018b1b92ec1874e815ace7ce3c948fe8c8ea`  
		Last Modified: Tue, 17 Aug 2021 09:43:02 GMT  
		Size: 10.6 MB (10572088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c2bac917a1fcd804dd397408311320a680c743c2e90437422491a062c16b37`  
		Last Modified: Tue, 17 Aug 2021 09:43:52 GMT  
		Size: 53.2 MB (53162948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3bfc85a26073067cb5d47404e861e10a9b16acbeaf9a46bf6f5ff7e4c76f26`  
		Last Modified: Tue, 17 Aug 2021 09:45:50 GMT  
		Size: 175.4 MB (175434830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b3d4233d2c38ac382c41432382339368b97b4091dd57b816568d20a38f83339c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.2 MB (284204177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0cdedcbc9c431bec8e9a11931577f0827e9460fe4221c57dd5b6ba4b477b7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:17:03 GMT
ADD file:75b6eb36a0ba8612cac405c278e0b6859f0857f284d7f2da3bc8ad6f4596cb7d in / 
# Tue, 17 Aug 2021 02:17:04 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:25:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:25:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:26:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:27:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86a6508bfdcb208b57a6ef5ca954ff178d89a14ca7c65b27bcd68df01e915895`  
		Last Modified: Tue, 17 Aug 2021 02:34:04 GMT  
		Size: 50.1 MB (50148031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894d51adc3dd9d078687cb2de22546210c7c13da66ac22c2e59180e6c194ddb`  
		Last Modified: Tue, 17 Aug 2021 15:43:55 GMT  
		Size: 4.9 MB (4937133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c61d960a4bb6b195a3e18c7e848519224d78371f6f147c8385202bcdab4023`  
		Last Modified: Tue, 17 Aug 2021 15:43:57 GMT  
		Size: 10.2 MB (10217512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cacd13952822a4eee5f0a451c9ca9324612dfe962c2c8f6c1e5ad8ec953c3c`  
		Last Modified: Tue, 17 Aug 2021 15:44:48 GMT  
		Size: 51.1 MB (51113693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98862062e57fe52710d4ffb6c0843dda047d1266229ba48b659752bc45f51895`  
		Last Modified: Tue, 17 Aug 2021 15:46:36 GMT  
		Size: 167.8 MB (167787808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7030b40a4d93866530c63b0070c4fb19df9d4b2d8e9c45fa08a148cbf4b68697
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.5 MB (315489595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8b77487ed2389e4f72c688d728194d97cb3bf6cf78144f4983b358713225cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:32 GMT
ADD file:2eb550b4dc61105505c60437af91d7300fc5596834bfce84a75b260663bf4f42 in / 
# Tue, 17 Aug 2021 01:47:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:55:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:55:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:55:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:56:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c8e1604d5b38112a190afe29ac6b4d1c501651ae9e68b6eaa49788ae64f145d`  
		Last Modified: Tue, 17 Aug 2021 01:56:14 GMT  
		Size: 53.6 MB (53625965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4b3d12f8e0cac2ab78286575b8f56d2cadedcafd68908cc60821856f5e360`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 5.2 MB (5160051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb41ce34a000fbba6dafcb340db9d0b7f64a8efd27ff966f77978ddd2c567439`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 10.9 MB (10873429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7ff3790681e7d2217b96a8b89bdf6b99ab28fa3c7c0da0c88118fa977a7ce9`  
		Last Modified: Tue, 17 Aug 2021 08:03:58 GMT  
		Size: 55.4 MB (55414468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168df4c59e132a8a240d09c437b400a3c05962347006f90a438bd329f995729`  
		Last Modified: Tue, 17 Aug 2021 08:04:37 GMT  
		Size: 190.4 MB (190415682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:97d4fde8a2be765cae7f2ab60ba592c97c8fa2e0a9d5c68af477246aa4d62768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329396504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5acf4b10d41b0fe38a7f0365df036214514ac503b45b8d91bb5d5f72329683e6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:42 GMT
ADD file:8d9eb4b2afc4eb0058f4080c5f0eedf0ddef323f1cc5a0403658254d191f117e in / 
# Tue, 17 Aug 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:02:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:03:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:79e62a40ce7bfbbe436e33c1da1c5661386b9674fe81402fdbfbb42a5b84998b`  
		Last Modified: Tue, 17 Aug 2021 01:52:55 GMT  
		Size: 56.0 MB (55967475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3391f9add930caab1f7ad8d326db740aab914960a3522b2baea8f34b06d23`  
		Last Modified: Tue, 17 Aug 2021 02:11:30 GMT  
		Size: 5.3 MB (5301763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c1c03bbd7c2f8c23dd8b5a8bae89de98d00fe400f6f7c89140aed7a78c6aa7`  
		Last Modified: Tue, 17 Aug 2021 02:11:31 GMT  
		Size: 11.3 MB (11250490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71047ae47f0ad2d0279c1731200ffbae15c68839f662197eb53927e89f4a346a`  
		Last Modified: Tue, 17 Aug 2021 02:11:56 GMT  
		Size: 56.7 MB (56684792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2118c03028a270167b86bbfa714238fc20ce6fcba7db2de02928657dbbcdb9`  
		Last Modified: Tue, 17 Aug 2021 02:12:48 GMT  
		Size: 200.2 MB (200191984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3afe0eb83a1d2b02654ced38fce91c3113deefaf57a2eb0c344eeca8c167f5fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (302974399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8334ddfd22e4126eab61b74efdbc14fd1220498aefd2fbc6852cbd759cfd112`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:13:43 GMT
ADD file:a77aad2a2ac623e0a0640ce1caa07dc2982875f5e01f2baec92d08795be4ad93 in / 
# Tue, 17 Aug 2021 01:13:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:51:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:53:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e190daae609fdf78d1dc3b15955b491e5dba465be6fc9a8a7ffc7a7039ffccd6`  
		Last Modified: Tue, 17 Aug 2021 01:23:46 GMT  
		Size: 53.2 MB (53198954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86d281139f06d0443f660a40811f7a489e4a83c078e49d5b8f57195e98409cf`  
		Last Modified: Tue, 17 Aug 2021 21:00:30 GMT  
		Size: 5.1 MB (5131004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99713d0cdbd7eef9bc879aca6d384c6712d27d4af1616629bada8c72f448a620`  
		Last Modified: Tue, 17 Aug 2021 21:00:33 GMT  
		Size: 10.9 MB (10873555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa119cf8ddcc3e8e9ab5ccb513faee61d808d3ca9cfb4d4ef9d68386a6848f`  
		Last Modified: Tue, 17 Aug 2021 21:01:23 GMT  
		Size: 54.3 MB (54264071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614453a7d63e2b291eae511f2a53543b63f728d3d16e35342663dd17bb00e1a6`  
		Last Modified: Tue, 17 Aug 2021 21:03:30 GMT  
		Size: 179.5 MB (179506815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c3bd218a847687d723b4ea74f3d272c6c3d821c14455f89aa40519ac92162367
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332737468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f34fe1147300f860a425db5f0166a3f5469ec71225b0edab829490bf30faca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:35:46 GMT
ADD file:3bdf0f06854c7b6578701900c267a6a5a712e84cc267d519df82eb28d568221c in / 
# Tue, 17 Aug 2021 01:35:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:24:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:26:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:54:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d596d5bddf4c6763b1156eb07675e21eb75a9b5bc9e5629b035d92244696d704`  
		Last Modified: Tue, 17 Aug 2021 01:52:09 GMT  
		Size: 58.9 MB (58855169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3055c003e2e867f5f7baa6505d799eff17441266441133ae556e40de99b75429`  
		Last Modified: Tue, 17 Aug 2021 16:10:29 GMT  
		Size: 5.4 MB (5421863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a281bbbade77271f6acd86003d63e414b000f703adebe3ff4c838ab7244b2c`  
		Last Modified: Tue, 17 Aug 2021 16:10:31 GMT  
		Size: 11.6 MB (11626757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d86af2c2f0d04abf574423e9d1d5c3771093d278c3c65bcb999fee07604f643`  
		Last Modified: Tue, 17 Aug 2021 16:12:29 GMT  
		Size: 59.9 MB (59883318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815763adc68353307c31a3ba0dce4b537a40f61b31cf42e0e050874ee170db45`  
		Last Modified: Tue, 17 Aug 2021 16:15:04 GMT  
		Size: 197.0 MB (196950361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:791e251bc4cb264f5035b6d51f0de093de65a9b68e2c02d3887b5dd55bf589c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329744362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5900075fa959e9c06925c33138e367fe67bbfcbfe99d3e4d8d0751e575a1429`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:57 GMT
ADD file:17c3a69ac6b2ac905f0d9d5d8d828215848c91b6aca208c63e3c8c6c3c28ac20 in / 
# Tue, 17 Aug 2021 01:45:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:29:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:33:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:43:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03abe71e39e08cd630ff168b11929dc5c3c5111cfb3d81f5a8183f7ba7162fab`  
		Last Modified: Tue, 17 Aug 2021 02:01:48 GMT  
		Size: 50.4 MB (50437771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e3ddf2aa723d9dc92fc071b3cc373219cd68de4072a024dc13965f2156705`  
		Last Modified: Tue, 17 Aug 2021 03:07:39 GMT  
		Size: 5.0 MB (4984859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbcb287940d650490755774d53a8edf26fba9558538160b4f649b66979ee4d`  
		Last Modified: Tue, 17 Aug 2021 03:07:43 GMT  
		Size: 10.3 MB (10293904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecda3ed528238bab9bf59ea2bc04887f931df81d6afd6768a21f6cb99a711637`  
		Last Modified: Tue, 17 Aug 2021 03:09:51 GMT  
		Size: 51.4 MB (51387224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3175c8a8bbf446d59b78ab670863174b7a4426d3ff03cafcf314f6c0449c4f05`  
		Last Modified: Tue, 17 Aug 2021 03:15:44 GMT  
		Size: 212.6 MB (212640604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:00c27d2eaa6c65a4cabff2ccc774ff8415fdc24e95cacf11fd8a9158729549b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.2 MB (297230778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f8588692cd0ecb96393420b73e8864acb9011c076ff04727891cc6ca741813f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:51:06 GMT
ADD file:ab809bd14c40234cf29151f2485ed39a9fa31f67c202abe6bf8546f5899aa52f in / 
# Tue, 17 Aug 2021 01:51:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:37:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:39:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6758b3369d7c595105d273788911a60f3cbd8b26d39dea406c75de4d1da4a084`  
		Last Modified: Tue, 17 Aug 2021 01:59:02 GMT  
		Size: 53.2 MB (53226590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee5f5767e372ec2c62434ed4325aa1b14846b20d736bdb81e1861163803d98`  
		Last Modified: Tue, 17 Aug 2021 07:45:09 GMT  
		Size: 5.2 MB (5152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1daed3fa6142f9fe36fd70a1e631c71aa839f077885d60cb4e7fb21210dacc`  
		Last Modified: Tue, 17 Aug 2021 07:45:10 GMT  
		Size: 10.8 MB (10763976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52078ebb293da4fc08dd7b04c3124715e75d72e8d33e91bcdaf326bcad28bdb`  
		Last Modified: Tue, 17 Aug 2021 07:45:26 GMT  
		Size: 54.7 MB (54724881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095155f9776442484b7b68f12906c0078739fa9a10717a8b4caf8bae637f75ba`  
		Last Modified: Tue, 17 Aug 2021 07:45:54 GMT  
		Size: 173.4 MB (173362475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:9024dbabe7a1da375a2ea36118557b2f0f3c1c7a7eeddae64d719108a78539a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5d6bc794b03974feb0bca10638255c61d229c30482c16488bf76bd19de3866c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70974998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b61c222380eee70d755288337c14d488c6aaa25dcd184ed039dbaef3fabab8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:06 GMT
ADD file:3052ec53a19fa26baad5d50e4d2867be2cc386ae62195d8dbb9d90d0b904c464 in / 
# Tue, 17 Aug 2021 01:25:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a6952a6bd46e0eaa2c0e7e851a45f288b3dc080472a9249e48c74b3fb7551fcc`  
		Last Modified: Tue, 17 Aug 2021 01:31:55 GMT  
		Size: 54.9 MB (54930846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ac09fd3cc15f0b26d3a8005c31390d5de204431a0355ffc55e60a6a8f3b25`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 5.2 MB (5171335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e5aaa7713c8cc3d2dd4d36732e1aac9d876c81ddc49221a0d413f2d4f7dcb1`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 10.9 MB (10872817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3d791feb2549b4b03c2e48bcb7d5deb42f1a8752dda92091267f9867edfb81c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68141653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebd6ddbec1219266e98b1930904201cf38f080dc8ab6427e0c39b6fdb448051e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:59:08 GMT
ADD file:f9ad3ec0db7a58cdae9cae8207122785d2b8c116c5bb4d47d46f530bda897397 in / 
# Tue, 17 Aug 2021 01:59:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:26:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8f84c96ba3e58d3cff4f87a969dd91565bb9be34588bf76d1a5a253c40ee1139`  
		Last Modified: Tue, 17 Aug 2021 02:16:06 GMT  
		Size: 52.5 MB (52493950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97b83ef80c1b594046817ebd2be34eaa8faee56f4463a801453d7757341208b`  
		Last Modified: Tue, 17 Aug 2021 09:42:59 GMT  
		Size: 5.1 MB (5075615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c50a77e6ef78b9b162607f1afc018b1b92ec1874e815ace7ce3c948fe8c8ea`  
		Last Modified: Tue, 17 Aug 2021 09:43:02 GMT  
		Size: 10.6 MB (10572088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:145f85437ade6ab27652a447c637dcc1efd6d627d69571e89a9a30de68e9ca31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65302676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfd861564ad7af9f83d87f0b53feb3deea7080ddbfaed0678f2fc99c2b942ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:17:03 GMT
ADD file:75b6eb36a0ba8612cac405c278e0b6859f0857f284d7f2da3bc8ad6f4596cb7d in / 
# Tue, 17 Aug 2021 02:17:04 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:25:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:25:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:86a6508bfdcb208b57a6ef5ca954ff178d89a14ca7c65b27bcd68df01e915895`  
		Last Modified: Tue, 17 Aug 2021 02:34:04 GMT  
		Size: 50.1 MB (50148031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894d51adc3dd9d078687cb2de22546210c7c13da66ac22c2e59180e6c194ddb`  
		Last Modified: Tue, 17 Aug 2021 15:43:55 GMT  
		Size: 4.9 MB (4937133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c61d960a4bb6b195a3e18c7e848519224d78371f6f147c8385202bcdab4023`  
		Last Modified: Tue, 17 Aug 2021 15:43:57 GMT  
		Size: 10.2 MB (10217512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:95d6d67d8406fecd07f2ca47fb1c181429f99d8aa0fc2ea109f9f7e7ce9e9a1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69659445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da9d49ec2b2035e68d98fe9d85208d455692b9c1c6a998f4e214216593a3973`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:32 GMT
ADD file:2eb550b4dc61105505c60437af91d7300fc5596834bfce84a75b260663bf4f42 in / 
# Tue, 17 Aug 2021 01:47:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:55:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:55:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0c8e1604d5b38112a190afe29ac6b4d1c501651ae9e68b6eaa49788ae64f145d`  
		Last Modified: Tue, 17 Aug 2021 01:56:14 GMT  
		Size: 53.6 MB (53625965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4b3d12f8e0cac2ab78286575b8f56d2cadedcafd68908cc60821856f5e360`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 5.2 MB (5160051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb41ce34a000fbba6dafcb340db9d0b7f64a8efd27ff966f77978ddd2c567439`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 10.9 MB (10873429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1fff776b370dd15d9693f26b99eb5780cdcdb3bb8e65edd38597f03b4e64d758
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72519728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddda0428d54281258d8a03082810ed4c348538dc58305c7e6a3471f26fe2df0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:42 GMT
ADD file:8d9eb4b2afc4eb0058f4080c5f0eedf0ddef323f1cc5a0403658254d191f117e in / 
# Tue, 17 Aug 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:02:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:79e62a40ce7bfbbe436e33c1da1c5661386b9674fe81402fdbfbb42a5b84998b`  
		Last Modified: Tue, 17 Aug 2021 01:52:55 GMT  
		Size: 56.0 MB (55967475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3391f9add930caab1f7ad8d326db740aab914960a3522b2baea8f34b06d23`  
		Last Modified: Tue, 17 Aug 2021 02:11:30 GMT  
		Size: 5.3 MB (5301763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c1c03bbd7c2f8c23dd8b5a8bae89de98d00fe400f6f7c89140aed7a78c6aa7`  
		Last Modified: Tue, 17 Aug 2021 02:11:31 GMT  
		Size: 11.3 MB (11250490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:98d7bad65228d9092b100017daa4d05eac8019a3dbe623a4adefe8f9373977f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69203513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a36a3cbc335f2339b81ecd932608bf269d960941ef345fb150a652c913e776be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:13:43 GMT
ADD file:a77aad2a2ac623e0a0640ce1caa07dc2982875f5e01f2baec92d08795be4ad93 in / 
# Tue, 17 Aug 2021 01:13:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e190daae609fdf78d1dc3b15955b491e5dba465be6fc9a8a7ffc7a7039ffccd6`  
		Last Modified: Tue, 17 Aug 2021 01:23:46 GMT  
		Size: 53.2 MB (53198954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86d281139f06d0443f660a40811f7a489e4a83c078e49d5b8f57195e98409cf`  
		Last Modified: Tue, 17 Aug 2021 21:00:30 GMT  
		Size: 5.1 MB (5131004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99713d0cdbd7eef9bc879aca6d384c6712d27d4af1616629bada8c72f448a620`  
		Last Modified: Tue, 17 Aug 2021 21:00:33 GMT  
		Size: 10.9 MB (10873555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4f884fa29acd285b5b2771d8cc4bce5275b8afc32f27f4bd75703664d0fc3a10
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75903789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f518063b21791802c1bda67dbdbcc4e0499960cdc1d888f032263ba4920d1e48`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:35:46 GMT
ADD file:3bdf0f06854c7b6578701900c267a6a5a712e84cc267d519df82eb28d568221c in / 
# Tue, 17 Aug 2021 01:35:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:24:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:26:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d596d5bddf4c6763b1156eb07675e21eb75a9b5bc9e5629b035d92244696d704`  
		Last Modified: Tue, 17 Aug 2021 01:52:09 GMT  
		Size: 58.9 MB (58855169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3055c003e2e867f5f7baa6505d799eff17441266441133ae556e40de99b75429`  
		Last Modified: Tue, 17 Aug 2021 16:10:29 GMT  
		Size: 5.4 MB (5421863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a281bbbade77271f6acd86003d63e414b000f703adebe3ff4c838ab7244b2c`  
		Last Modified: Tue, 17 Aug 2021 16:10:31 GMT  
		Size: 11.6 MB (11626757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ea1ea7eb3f215c84403554672c91c22945344400c673d6f1522fd607ee45c612
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65716534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7bd69c97313ca7d402f43854f393547d6854ae7a3b046c650dadf00adab219`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:57 GMT
ADD file:17c3a69ac6b2ac905f0d9d5d8d828215848c91b6aca208c63e3c8c6c3c28ac20 in / 
# Tue, 17 Aug 2021 01:45:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:29:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:03abe71e39e08cd630ff168b11929dc5c3c5111cfb3d81f5a8183f7ba7162fab`  
		Last Modified: Tue, 17 Aug 2021 02:01:48 GMT  
		Size: 50.4 MB (50437771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e3ddf2aa723d9dc92fc071b3cc373219cd68de4072a024dc13965f2156705`  
		Last Modified: Tue, 17 Aug 2021 03:07:39 GMT  
		Size: 5.0 MB (4984859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbcb287940d650490755774d53a8edf26fba9558538160b4f649b66979ee4d`  
		Last Modified: Tue, 17 Aug 2021 03:07:43 GMT  
		Size: 10.3 MB (10293904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fab97181f913819d52d80648d12308e39e2b6edf93eed0dd25b6269b1e975638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69143422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b34924373ab74ba0650cd2931dacfef322ec14458f9202a4078c99c5f43650a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:51:06 GMT
ADD file:ab809bd14c40234cf29151f2485ed39a9fa31f67c202abe6bf8546f5899aa52f in / 
# Tue, 17 Aug 2021 01:51:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:37:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6758b3369d7c595105d273788911a60f3cbd8b26d39dea406c75de4d1da4a084`  
		Last Modified: Tue, 17 Aug 2021 01:59:02 GMT  
		Size: 53.2 MB (53226590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee5f5767e372ec2c62434ed4325aa1b14846b20d736bdb81e1861163803d98`  
		Last Modified: Tue, 17 Aug 2021 07:45:09 GMT  
		Size: 5.2 MB (5152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1daed3fa6142f9fe36fd70a1e631c71aa839f077885d60cb4e7fb21210dacc`  
		Last Modified: Tue, 17 Aug 2021 07:45:10 GMT  
		Size: 10.8 MB (10763976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:fc2b7d4525cb2656724b5da8e1e3a32b60ed1578e93a940fc4f9c1ed52bcb907
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4ce0505fd2f716a12637bce8cb2ea04b1f403f5bc10c794f0e11ee9e9ccd677d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126428830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d233be97a8804fc816ed0a4d036f84b04e91f53dab70bf7cbbfb72d15d81f11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:06 GMT
ADD file:3052ec53a19fa26baad5d50e4d2867be2cc386ae62195d8dbb9d90d0b904c464 in / 
# Tue, 17 Aug 2021 01:25:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6952a6bd46e0eaa2c0e7e851a45f288b3dc080472a9249e48c74b3fb7551fcc`  
		Last Modified: Tue, 17 Aug 2021 01:31:55 GMT  
		Size: 54.9 MB (54930846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ac09fd3cc15f0b26d3a8005c31390d5de204431a0355ffc55e60a6a8f3b25`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 5.2 MB (5171335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e5aaa7713c8cc3d2dd4d36732e1aac9d876c81ddc49221a0d413f2d4f7dcb1`  
		Last Modified: Tue, 17 Aug 2021 09:31:52 GMT  
		Size: 10.9 MB (10872817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11986d12d3ac34fc246feb151c1fbc9cdf5db866e53edb07c12fcda5e91e187a`  
		Last Modified: Tue, 17 Aug 2021 09:32:14 GMT  
		Size: 55.5 MB (55453832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fc195efcaabeee27dd247ca281492315d995b9c123f7b6c168f62205c525c681
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121304601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ff593b6ceaeb3e7dfb6e363517c76c7d27441894855740c03e86f759bb782b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:59:08 GMT
ADD file:f9ad3ec0db7a58cdae9cae8207122785d2b8c116c5bb4d47d46f530bda897397 in / 
# Tue, 17 Aug 2021 01:59:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:26:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:27:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f84c96ba3e58d3cff4f87a969dd91565bb9be34588bf76d1a5a253c40ee1139`  
		Last Modified: Tue, 17 Aug 2021 02:16:06 GMT  
		Size: 52.5 MB (52493950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97b83ef80c1b594046817ebd2be34eaa8faee56f4463a801453d7757341208b`  
		Last Modified: Tue, 17 Aug 2021 09:42:59 GMT  
		Size: 5.1 MB (5075615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c50a77e6ef78b9b162607f1afc018b1b92ec1874e815ace7ce3c948fe8c8ea`  
		Last Modified: Tue, 17 Aug 2021 09:43:02 GMT  
		Size: 10.6 MB (10572088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c2bac917a1fcd804dd397408311320a680c743c2e90437422491a062c16b37`  
		Last Modified: Tue, 17 Aug 2021 09:43:52 GMT  
		Size: 53.2 MB (53162948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:614f5e84242acb4f77da6c4f20e61e8935fa7023f4de2f109e253786245f81aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116416369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67104fbe683be478e692224d7dbbf566952954f8cd25ca554a571e912d140d67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:17:03 GMT
ADD file:75b6eb36a0ba8612cac405c278e0b6859f0857f284d7f2da3bc8ad6f4596cb7d in / 
# Tue, 17 Aug 2021 02:17:04 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:25:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:25:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:26:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86a6508bfdcb208b57a6ef5ca954ff178d89a14ca7c65b27bcd68df01e915895`  
		Last Modified: Tue, 17 Aug 2021 02:34:04 GMT  
		Size: 50.1 MB (50148031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c894d51adc3dd9d078687cb2de22546210c7c13da66ac22c2e59180e6c194ddb`  
		Last Modified: Tue, 17 Aug 2021 15:43:55 GMT  
		Size: 4.9 MB (4937133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c61d960a4bb6b195a3e18c7e848519224d78371f6f147c8385202bcdab4023`  
		Last Modified: Tue, 17 Aug 2021 15:43:57 GMT  
		Size: 10.2 MB (10217512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cacd13952822a4eee5f0a451c9ca9324612dfe962c2c8f6c1e5ad8ec953c3c`  
		Last Modified: Tue, 17 Aug 2021 15:44:48 GMT  
		Size: 51.1 MB (51113693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37bee1487624fd84c180d6b30ee44482d1ae1d363ae4312e0ae72e29742d84e8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125073913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3efdbbeaeb82295134826aa702e6298a62dd1936103e9b1f058056bf4a1721af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:32 GMT
ADD file:2eb550b4dc61105505c60437af91d7300fc5596834bfce84a75b260663bf4f42 in / 
# Tue, 17 Aug 2021 01:47:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:55:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:55:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:55:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c8e1604d5b38112a190afe29ac6b4d1c501651ae9e68b6eaa49788ae64f145d`  
		Last Modified: Tue, 17 Aug 2021 01:56:14 GMT  
		Size: 53.6 MB (53625965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4b3d12f8e0cac2ab78286575b8f56d2cadedcafd68908cc60821856f5e360`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 5.2 MB (5160051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb41ce34a000fbba6dafcb340db9d0b7f64a8efd27ff966f77978ddd2c567439`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 10.9 MB (10873429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7ff3790681e7d2217b96a8b89bdf6b99ab28fa3c7c0da0c88118fa977a7ce9`  
		Last Modified: Tue, 17 Aug 2021 08:03:58 GMT  
		Size: 55.4 MB (55414468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:04e0650bc727dd18f73c095ef5f35e238acfdbc963764c86f55dbd57a2817916
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129204520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3ac461708875960f1d5e7c484c1b60c5867b04bbdbb89494195e2999ae5c74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:42 GMT
ADD file:8d9eb4b2afc4eb0058f4080c5f0eedf0ddef323f1cc5a0403658254d191f117e in / 
# Tue, 17 Aug 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:02:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:79e62a40ce7bfbbe436e33c1da1c5661386b9674fe81402fdbfbb42a5b84998b`  
		Last Modified: Tue, 17 Aug 2021 01:52:55 GMT  
		Size: 56.0 MB (55967475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3391f9add930caab1f7ad8d326db740aab914960a3522b2baea8f34b06d23`  
		Last Modified: Tue, 17 Aug 2021 02:11:30 GMT  
		Size: 5.3 MB (5301763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c1c03bbd7c2f8c23dd8b5a8bae89de98d00fe400f6f7c89140aed7a78c6aa7`  
		Last Modified: Tue, 17 Aug 2021 02:11:31 GMT  
		Size: 11.3 MB (11250490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71047ae47f0ad2d0279c1731200ffbae15c68839f662197eb53927e89f4a346a`  
		Last Modified: Tue, 17 Aug 2021 02:11:56 GMT  
		Size: 56.7 MB (56684792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c1f36d5b0b0dcee92a157a00014bb120bf3e0526c31c561fddf31d9be0c0b241
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123467584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a236cbbfbe37dcf11589dcef6062492f943e44179a009ba1665e0fcb1a4e1af7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:13:43 GMT
ADD file:a77aad2a2ac623e0a0640ce1caa07dc2982875f5e01f2baec92d08795be4ad93 in / 
# Tue, 17 Aug 2021 01:13:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:51:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e190daae609fdf78d1dc3b15955b491e5dba465be6fc9a8a7ffc7a7039ffccd6`  
		Last Modified: Tue, 17 Aug 2021 01:23:46 GMT  
		Size: 53.2 MB (53198954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86d281139f06d0443f660a40811f7a489e4a83c078e49d5b8f57195e98409cf`  
		Last Modified: Tue, 17 Aug 2021 21:00:30 GMT  
		Size: 5.1 MB (5131004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99713d0cdbd7eef9bc879aca6d384c6712d27d4af1616629bada8c72f448a620`  
		Last Modified: Tue, 17 Aug 2021 21:00:33 GMT  
		Size: 10.9 MB (10873555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa119cf8ddcc3e8e9ab5ccb513faee61d808d3ca9cfb4d4ef9d68386a6848f`  
		Last Modified: Tue, 17 Aug 2021 21:01:23 GMT  
		Size: 54.3 MB (54264071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bdaf74ed5eb85a64320a1879fd8cb3fbc0b25ac5c31d2c487285f9490290ee94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135787107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2446242db75bbe280501c39a5d487742a2b9189f01a6865da572325bd1a7a878`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:35:46 GMT
ADD file:3bdf0f06854c7b6578701900c267a6a5a712e84cc267d519df82eb28d568221c in / 
# Tue, 17 Aug 2021 01:35:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:24:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:26:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d596d5bddf4c6763b1156eb07675e21eb75a9b5bc9e5629b035d92244696d704`  
		Last Modified: Tue, 17 Aug 2021 01:52:09 GMT  
		Size: 58.9 MB (58855169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3055c003e2e867f5f7baa6505d799eff17441266441133ae556e40de99b75429`  
		Last Modified: Tue, 17 Aug 2021 16:10:29 GMT  
		Size: 5.4 MB (5421863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a281bbbade77271f6acd86003d63e414b000f703adebe3ff4c838ab7244b2c`  
		Last Modified: Tue, 17 Aug 2021 16:10:31 GMT  
		Size: 11.6 MB (11626757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d86af2c2f0d04abf574423e9d1d5c3771093d278c3c65bcb999fee07604f643`  
		Last Modified: Tue, 17 Aug 2021 16:12:29 GMT  
		Size: 59.9 MB (59883318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8105fd441cbd36f7bde58e34b24e9329d34e31d2c7e2592edbd60d5ac0d77efd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117103758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27c68b1a73365a21c15885cd64ba01cc9fbb3f9160c6787ce5b37cdaa3cb6a9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:57 GMT
ADD file:17c3a69ac6b2ac905f0d9d5d8d828215848c91b6aca208c63e3c8c6c3c28ac20 in / 
# Tue, 17 Aug 2021 01:45:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:29:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:33:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03abe71e39e08cd630ff168b11929dc5c3c5111cfb3d81f5a8183f7ba7162fab`  
		Last Modified: Tue, 17 Aug 2021 02:01:48 GMT  
		Size: 50.4 MB (50437771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e3ddf2aa723d9dc92fc071b3cc373219cd68de4072a024dc13965f2156705`  
		Last Modified: Tue, 17 Aug 2021 03:07:39 GMT  
		Size: 5.0 MB (4984859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbcb287940d650490755774d53a8edf26fba9558538160b4f649b66979ee4d`  
		Last Modified: Tue, 17 Aug 2021 03:07:43 GMT  
		Size: 10.3 MB (10293904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecda3ed528238bab9bf59ea2bc04887f931df81d6afd6768a21f6cb99a711637`  
		Last Modified: Tue, 17 Aug 2021 03:09:51 GMT  
		Size: 51.4 MB (51387224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:508193ae57b397427a2d0c356c071845bd3d17f174589d82e138df64ec7e90bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123868303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7f4f7bd222e4b52b7b76ccd1407623917c762cf5daa6d1d6646c1c65968e00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:51:06 GMT
ADD file:ab809bd14c40234cf29151f2485ed39a9fa31f67c202abe6bf8546f5899aa52f in / 
# Tue, 17 Aug 2021 01:51:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:37:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6758b3369d7c595105d273788911a60f3cbd8b26d39dea406c75de4d1da4a084`  
		Last Modified: Tue, 17 Aug 2021 01:59:02 GMT  
		Size: 53.2 MB (53226590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee5f5767e372ec2c62434ed4325aa1b14846b20d736bdb81e1861163803d98`  
		Last Modified: Tue, 17 Aug 2021 07:45:09 GMT  
		Size: 5.2 MB (5152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1daed3fa6142f9fe36fd70a1e631c71aa839f077885d60cb4e7fb21210dacc`  
		Last Modified: Tue, 17 Aug 2021 07:45:10 GMT  
		Size: 10.8 MB (10763976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52078ebb293da4fc08dd7b04c3124715e75d72e8d33e91bcdaf326bcad28bdb`  
		Last Modified: Tue, 17 Aug 2021 07:45:26 GMT  
		Size: 54.7 MB (54724881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:xenial`

```console
$ docker pull buildpack-deps@sha256:bb129802c0c6057515fb72e3cea6355cb13e6014d528e081c29c6679f6a35e79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:xenial` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:aa9e0333df32def9001a677ff89a5c09213d91d030b4439bfe9c01153f997ca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.4 MB (236392854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd46abf564eb1523a47e8d464e3a01b07d272b68fd1538cf5d850114d417d258`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 22:03:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:03:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:04:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84cf3b385fa330cddfcec4c9fe29c02ba73e5ce4eeeb01b4b1fcc16ac1c28a9`  
		Last Modified: Mon, 26 Jul 2021 22:15:57 GMT  
		Size: 7.8 MB (7790900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc0223d40ee93a1ec66a4a4c73009a6ec0aecb2dc36910248e21b9066bbe353`  
		Last Modified: Mon, 26 Jul 2021 22:16:16 GMT  
		Size: 41.9 MB (41906076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84e4d3d55d27152a8e4f53008dd952792ba5a25c167f2da2a2040fc9011fea3`  
		Last Modified: Mon, 26 Jul 2021 22:16:46 GMT  
		Size: 140.2 MB (140196965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0d52b28c376957c832f21e2bb02fa870bf44bc3e50c55e0345dd43ecad81791e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202400746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34532f92c4963d1c6422c949b4b5892473edefeb2d84cdfc6e8669bde921cfea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:53:34 GMT
ADD file:4b9fec92db5a0e4059d8b16893d817dca169e585547a48cf5ec6d4afc56e997c in / 
# Mon, 26 Jul 2021 22:53:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 22:53:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:53:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 22:53:41 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 01:31:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:34:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba10bfe0b6395fa726456c96036b4fd8ef0513d396442e7419e81550b626b4a0`  
		Last Modified: Sat, 24 Jul 2021 22:43:19 GMT  
		Size: 40.3 MB (40312522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b2be9419691b3c616ec69316c8bef11216dce2cc63b22ba203ada71a1a1f08`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2278b7cd7720a82be011f94dfd9d056b889b12068623fc864b02b096cb01ad`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e23ab739c679be25d516008b91998dc0513145f9ecb2fa75e1c762def8699`  
		Last Modified: Mon, 26 Jul 2021 22:58:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c3f69a6d2542114190cf9d0dd3b5d65d06d1e187e7573fde2c374fb1ba911f`  
		Last Modified: Tue, 27 Jul 2021 01:52:38 GMT  
		Size: 6.6 MB (6631696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d3e4de014d1c265e7133c67440a52321689ea8c718c3367d477494159d3dcf`  
		Last Modified: Tue, 27 Jul 2021 01:53:18 GMT  
		Size: 38.2 MB (38162616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c51aec69057796c4bd045f048f4f4d9f6638c1094a0cb237a2f8e1fe2055a7`  
		Last Modified: Tue, 27 Jul 2021 01:54:40 GMT  
		Size: 117.3 MB (117292380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5f1a74531a27625f7311e1d718d1bdc2373c90bf1550d7404722ebec31712bab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.1 MB (210145891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2987f35704c7cfe20318be2c51f0f799a493368655c37bbe5d9a5c7ab9af9337`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:14:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:16:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aadea1266928a0dceab31c4c15ffe7dbcda64c245cfec8104807007655c283`  
		Last Modified: Tue, 31 Aug 2021 02:23:32 GMT  
		Size: 6.8 MB (6838692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b021524e25acee25ed838c080f43172f4fbdb58e2f2b790bec964d32b0afa48`  
		Last Modified: Tue, 31 Aug 2021 02:23:51 GMT  
		Size: 39.8 MB (39808352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c042fa608c33de9985c2b60cf95d2d0e70f2e69853346af8ddf52c6c66f0e53d`  
		Last Modified: Tue, 31 Aug 2021 02:24:21 GMT  
		Size: 122.3 MB (122258097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial` - linux; 386

```console
$ docker pull buildpack-deps@sha256:774dc09a5f250b4b70cbb9eb42070e661de99639ab0a30c44fee7feed73fc45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236627828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df62604e2ff855d073d4271194e17d7ff178fbcc55537a86bd2b88e74043d7a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:03:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:03:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:07:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdc5ad45f3591df22f6cfd8a81e806096d73e75cb53dd36f2dc06bedc29cdf8`  
		Last Modified: Tue, 31 Aug 2021 02:11:05 GMT  
		Size: 7.9 MB (7933649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcec5a27c60c6c19817288510b120bb7290e04bbf035fa5d2aacfe5a35bfc3f7`  
		Last Modified: Tue, 31 Aug 2021 02:11:26 GMT  
		Size: 42.9 MB (42891141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84dec47a6a248f9ea193b70e2bdb533bcfe635eef0b254f93e60f330b0a9d921`  
		Last Modified: Tue, 31 Aug 2021 02:12:04 GMT  
		Size: 140.0 MB (139985319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fa632f14251fc91c75fd3c600e393aa69b240b725f3f5db8e60df418550e69de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.5 MB (245531703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd55efc20b2e3259d5ad6e52ceb4fd497e83f0d017a0d9cb26e4584e56211499`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:14:07 GMT
ADD file:8fe1a1dacf1dc31e5c6168e69c34f801191864c5fece1d91b13d59807f6056ca in / 
# Mon, 26 Jul 2021 23:14:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 23:14:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 23:14:28 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 04:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:07:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 04:09:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:19:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d472a4d60588bf877b1577439fb1db8b17861b63117a33841fe29225c530b95e`  
		Last Modified: Sat, 24 Jul 2021 22:43:36 GMT  
		Size: 47.5 MB (47522379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe44c44a8ee34d79983e97d8261707445db2732ccf6a93cc146c4cdbffca5696`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333f9295db0b7ef046f754b97473c3bd3514e0d9b8465d869119004c929e5261`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c736b6f8064fe10fc657f6af155f5b9827223a418712a0397b8ca50f7f19c83`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783e2b245674c811c355b44a116453c6514c3df2c057ed3df4a19bcbf9a717ac`  
		Last Modified: Tue, 27 Jul 2021 04:29:20 GMT  
		Size: 7.7 MB (7692708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3a0fe0a58f94d243f9f5cc3c5b58818b595e4658364d01f29e074a94fb2dd`  
		Last Modified: Tue, 27 Jul 2021 04:29:41 GMT  
		Size: 45.1 MB (45147746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c524fa6303aa9878acc0d304661e148adc711d79187a5cf31e6b844c296d32f`  
		Last Modified: Tue, 27 Jul 2021 04:30:19 GMT  
		Size: 145.2 MB (145167370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c6a4196d8af17c85172d35cd32e4f8366e1b3f614217582dd4dfad72a5cc00fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.0 MB (220978033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:612b92867d5821ccf9e5e4cd95953cd4499ca8f65e1f0b7baec2bae59321550f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:41:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:42:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd8a6861a80aa4b11ce96ec3537844aec4b713e8074deacba0614cd64afaf6f`  
		Last Modified: Tue, 31 Aug 2021 02:48:46 GMT  
		Size: 7.5 MB (7522004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102f08394215864198c62652fc16666081e5739d70caea25d4324e60bcab889`  
		Last Modified: Tue, 31 Aug 2021 02:49:00 GMT  
		Size: 42.7 MB (42688096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4200eefc2db30e95286e811f3f22d74a19ee78596fc4bd4b4caf13951a63a4b`  
		Last Modified: Tue, 31 Aug 2021 02:49:23 GMT  
		Size: 126.7 MB (126678714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:xenial-curl`

```console
$ docker pull buildpack-deps@sha256:f07d52aae65670c4495402c8616ee62cd4a39fa2b7b358bac4141d3f6a7d1724
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:xenial-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9f00f5d40c5d93d1537e58b0b41fc863e794115201436258052f285dbff3394d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54289813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5bfdc15c4830f18177a9c3efef4bf27c4a5900199e74269856f5d796d108024`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 22:03:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:03:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84cf3b385fa330cddfcec4c9fe29c02ba73e5ce4eeeb01b4b1fcc16ac1c28a9`  
		Last Modified: Mon, 26 Jul 2021 22:15:57 GMT  
		Size: 7.8 MB (7790900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5b3b0321d5806a2005a003d6171ca78704b4f354555180850039715adbebd129
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46945750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2794a265e57db998e79510b2a0959572659242687202607c0194f8c56c4c0724`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:53:34 GMT
ADD file:4b9fec92db5a0e4059d8b16893d817dca169e585547a48cf5ec6d4afc56e997c in / 
# Mon, 26 Jul 2021 22:53:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 22:53:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:53:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 22:53:41 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 01:31:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ba10bfe0b6395fa726456c96036b4fd8ef0513d396442e7419e81550b626b4a0`  
		Last Modified: Sat, 24 Jul 2021 22:43:19 GMT  
		Size: 40.3 MB (40312522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b2be9419691b3c616ec69316c8bef11216dce2cc63b22ba203ada71a1a1f08`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2278b7cd7720a82be011f94dfd9d056b889b12068623fc864b02b096cb01ad`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e23ab739c679be25d516008b91998dc0513145f9ecb2fa75e1c762def8699`  
		Last Modified: Mon, 26 Jul 2021 22:58:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c3f69a6d2542114190cf9d0dd3b5d65d06d1e187e7573fde2c374fb1ba911f`  
		Last Modified: Tue, 27 Jul 2021 01:52:38 GMT  
		Size: 6.6 MB (6631696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:53c2ad9b6d5a8f231ddac43584f00467a4b9918a7c614062fc833ffd844e857f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48079442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda81a56396c38d6854bb5ee19197cdce531349b4c380d6335aefdd57e2a1e86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:14:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aadea1266928a0dceab31c4c15ffe7dbcda64c245cfec8104807007655c283`  
		Last Modified: Tue, 31 Aug 2021 02:23:32 GMT  
		Size: 6.8 MB (6838692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:45377dd59b12b41a3c184175c0abed1b1c1c09d4dacab0d58dd20b2522c8664d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53751368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf531ac888458f106c0243748349eeae517521b381458acb72191a28a46fdc1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:03:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:03:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdc5ad45f3591df22f6cfd8a81e806096d73e75cb53dd36f2dc06bedc29cdf8`  
		Last Modified: Tue, 31 Aug 2021 02:11:05 GMT  
		Size: 7.9 MB (7933649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3b4ce36d4c54798487ae7087321faadf62daed06f811a2319250efe6eed04bad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55216587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c715c6822e85a1a0372c9e5ccff135c7dff5e30e5e4cee4eacac586cd03a5239`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:14:07 GMT
ADD file:8fe1a1dacf1dc31e5c6168e69c34f801191864c5fece1d91b13d59807f6056ca in / 
# Mon, 26 Jul 2021 23:14:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 23:14:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 23:14:28 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 04:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:07:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d472a4d60588bf877b1577439fb1db8b17861b63117a33841fe29225c530b95e`  
		Last Modified: Sat, 24 Jul 2021 22:43:36 GMT  
		Size: 47.5 MB (47522379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe44c44a8ee34d79983e97d8261707445db2732ccf6a93cc146c4cdbffca5696`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333f9295db0b7ef046f754b97473c3bd3514e0d9b8465d869119004c929e5261`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c736b6f8064fe10fc657f6af155f5b9827223a418712a0397b8ca50f7f19c83`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783e2b245674c811c355b44a116453c6514c3df2c057ed3df4a19bcbf9a717ac`  
		Last Modified: Tue, 27 Jul 2021 04:29:20 GMT  
		Size: 7.7 MB (7692708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fce0337e93d731b9480e9b84b713df100c81a878790af17ebf225f2e57ee3b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51611223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bd3c2184df3dd73fa66b9b478abedaaac68c45fef540666fe3657eb6c8efb7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd8a6861a80aa4b11ce96ec3537844aec4b713e8074deacba0614cd64afaf6f`  
		Last Modified: Tue, 31 Aug 2021 02:48:46 GMT  
		Size: 7.5 MB (7522004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:xenial-scm`

```console
$ docker pull buildpack-deps@sha256:8c152602c2aeada97c3b7553a69b7ffe2505dea9efdeb971537b168a4f0d772d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:xenial-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a0b568c44cbd3bf705cb7c0702fe00a82518bcf613d6576ec54692a61003aabf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.2 MB (96195889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:218c7c2a627b92b5b033c2dab9d971c7698135ad134928d70db8f8edaf8b3cc1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 22:03:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:03:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:04:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84cf3b385fa330cddfcec4c9fe29c02ba73e5ce4eeeb01b4b1fcc16ac1c28a9`  
		Last Modified: Mon, 26 Jul 2021 22:15:57 GMT  
		Size: 7.8 MB (7790900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc0223d40ee93a1ec66a4a4c73009a6ec0aecb2dc36910248e21b9066bbe353`  
		Last Modified: Mon, 26 Jul 2021 22:16:16 GMT  
		Size: 41.9 MB (41906076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eeeb88d27c0032638c5aaefe92fc8c6aea572cd80b774d91aac9fde8b8dd77cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85108366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ee7f6558335a1e9cdfb0381bb2c44c095c29c37d1b52a3b4f63dd9271d20f85`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:53:34 GMT
ADD file:4b9fec92db5a0e4059d8b16893d817dca169e585547a48cf5ec6d4afc56e997c in / 
# Mon, 26 Jul 2021 22:53:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 22:53:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:53:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 22:53:41 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 01:31:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba10bfe0b6395fa726456c96036b4fd8ef0513d396442e7419e81550b626b4a0`  
		Last Modified: Sat, 24 Jul 2021 22:43:19 GMT  
		Size: 40.3 MB (40312522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b2be9419691b3c616ec69316c8bef11216dce2cc63b22ba203ada71a1a1f08`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2278b7cd7720a82be011f94dfd9d056b889b12068623fc864b02b096cb01ad`  
		Last Modified: Mon, 26 Jul 2021 22:58:16 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e23ab739c679be25d516008b91998dc0513145f9ecb2fa75e1c762def8699`  
		Last Modified: Mon, 26 Jul 2021 22:58:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c3f69a6d2542114190cf9d0dd3b5d65d06d1e187e7573fde2c374fb1ba911f`  
		Last Modified: Tue, 27 Jul 2021 01:52:38 GMT  
		Size: 6.6 MB (6631696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d3e4de014d1c265e7133c67440a52321689ea8c718c3367d477494159d3dcf`  
		Last Modified: Tue, 27 Jul 2021 01:53:18 GMT  
		Size: 38.2 MB (38162616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e47a0201f60f95b8cbea4d83e717f345ee7edcf0bc7ae671fae5cda3e24c2e3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87887794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd8ff1996a08e2ab4f9f5ac3d0a19b55f7f2a37f02054ee40f428404a97102f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:14:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aadea1266928a0dceab31c4c15ffe7dbcda64c245cfec8104807007655c283`  
		Last Modified: Tue, 31 Aug 2021 02:23:32 GMT  
		Size: 6.8 MB (6838692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b021524e25acee25ed838c080f43172f4fbdb58e2f2b790bec964d32b0afa48`  
		Last Modified: Tue, 31 Aug 2021 02:23:51 GMT  
		Size: 39.8 MB (39808352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:99c96123c812918f785aa54ef205394d0732a16ebc10b17702c921ffae070da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96642509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5002ff2050d649c8975cea3b4976206d64870dcea48d80e5220d08e654bbb0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:03:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:03:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdc5ad45f3591df22f6cfd8a81e806096d73e75cb53dd36f2dc06bedc29cdf8`  
		Last Modified: Tue, 31 Aug 2021 02:11:05 GMT  
		Size: 7.9 MB (7933649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcec5a27c60c6c19817288510b120bb7290e04bbf035fa5d2aacfe5a35bfc3f7`  
		Last Modified: Tue, 31 Aug 2021 02:11:26 GMT  
		Size: 42.9 MB (42891141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3edc5049548c99f59ab3f938bd64d7ec5a77ec92a55cb38f248158eaa6de49a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100364333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d645f0f7b9454fe7d2ac0efbd2235fa3a9744fa49227ad3118d2f175bb9a5c5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:14:07 GMT
ADD file:8fe1a1dacf1dc31e5c6168e69c34f801191864c5fece1d91b13d59807f6056ca in / 
# Mon, 26 Jul 2021 23:14:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 23:14:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 23:14:28 GMT
CMD ["/bin/bash"]
# Tue, 27 Jul 2021 04:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 04:07:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 04:09:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d472a4d60588bf877b1577439fb1db8b17861b63117a33841fe29225c530b95e`  
		Last Modified: Sat, 24 Jul 2021 22:43:36 GMT  
		Size: 47.5 MB (47522379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe44c44a8ee34d79983e97d8261707445db2732ccf6a93cc146c4cdbffca5696`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333f9295db0b7ef046f754b97473c3bd3514e0d9b8465d869119004c929e5261`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c736b6f8064fe10fc657f6af155f5b9827223a418712a0397b8ca50f7f19c83`  
		Last Modified: Mon, 26 Jul 2021 23:17:19 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783e2b245674c811c355b44a116453c6514c3df2c057ed3df4a19bcbf9a717ac`  
		Last Modified: Tue, 27 Jul 2021 04:29:20 GMT  
		Size: 7.7 MB (7692708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3a0fe0a58f94d243f9f5cc3c5b58818b595e4658364d01f29e074a94fb2dd`  
		Last Modified: Tue, 27 Jul 2021 04:29:41 GMT  
		Size: 45.1 MB (45147746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a203418fa9ce17ec959479c3f6715d9ecc75466fd0aa528075e0cc9f94ec900a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94299319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c60d1962866a26c61283292dd8fbc87d1d75e3fb6c73d5f60070a001b7d67f40`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:41:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd8a6861a80aa4b11ce96ec3537844aec4b713e8074deacba0614cd64afaf6f`  
		Last Modified: Tue, 31 Aug 2021 02:48:46 GMT  
		Size: 7.5 MB (7522004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102f08394215864198c62652fc16666081e5739d70caea25d4324e60bcab889`  
		Last Modified: Tue, 31 Aug 2021 02:49:00 GMT  
		Size: 42.7 MB (42688096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
