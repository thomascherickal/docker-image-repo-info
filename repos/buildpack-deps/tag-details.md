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
$ docker pull buildpack-deps@sha256:bc56e6f62d4937f18fcd8ec8096bda57cbf9fad4d09cc85d81852e56cf85ca4e
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
$ docker pull buildpack-deps@sha256:415c4103ddc94a0ba15cfc220a261f43f8000d0e8f6c7af73ded0c66e63e3a1b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.4 MB (236392015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a479dc2c011ea4707ab6e48b150b1f6917474987bb4289c17178263b7320b3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:07:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:10:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42950b703a06b97a939a480237f84b19002bdea7a18b13134adc765328699d4d`  
		Last Modified: Tue, 31 Aug 2021 03:16:13 GMT  
		Size: 7.8 MB (7790543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2a7ae66eff85a2438aa0ea3586e8d8d638e66d1b32fe7d59a510cde54c2813`  
		Last Modified: Tue, 31 Aug 2021 03:16:30 GMT  
		Size: 41.9 MB (41905682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f044f40748825a2563b5545ec79398c53a46efb78ed955f6ef280afc9c0403`  
		Last Modified: Tue, 31 Aug 2021 03:16:58 GMT  
		Size: 140.2 MB (140196687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e8113cd72df13ee9ce4ad8efaf0c36e43c6f793f51ce9ad969612d42496f041f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202399881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de0787c69d4b4ca6b9a184d1f1fda5a4239c6913664adffed916ca9d38228288`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:25:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:28:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0c65fb267d23c5dd58ee3a818a8932a3fd565b8db9f6536fe98737a4e08f7`  
		Last Modified: Tue, 31 Aug 2021 03:44:48 GMT  
		Size: 6.6 MB (6631655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ffada20ea8521b2262a77a6239d4fc025f8f59d675a86c60923a075fb73d9d`  
		Last Modified: Tue, 31 Aug 2021 03:45:29 GMT  
		Size: 38.2 MB (38162364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d06b32826b0508bf1815ded75b8923a806d38c71670df7781d94612a6d5ea1`  
		Last Modified: Tue, 31 Aug 2021 03:46:52 GMT  
		Size: 117.3 MB (117292079 bytes)  
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
$ docker pull buildpack-deps@sha256:1a757e119c1ef3b09b0dc43addfebc79a914cc96960ecb404ab95db783caedcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.5 MB (245531585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9528843f5a733b688829d36c8fa4ada566f73da0c5fbc2085afdb9940fdac7d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:44:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:02:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c6ecbb79c70d45fca469278bf60d5e429f108594e71179f4a564aa3531b2d5`  
		Last Modified: Tue, 31 Aug 2021 05:34:20 GMT  
		Size: 7.7 MB (7693285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ba12653da3d4e66d89f4d0e6e7f60832cda0b7b78d6a428c517d0479e4b892`  
		Last Modified: Tue, 31 Aug 2021 05:36:50 GMT  
		Size: 45.1 MB (45147268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf88dce27d7ee92c7e90ace2790c859e6af24fcee1524c43ef37a50718cafa9`  
		Last Modified: Tue, 31 Aug 2021 05:39:27 GMT  
		Size: 145.2 MB (145167399 bytes)  
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
$ docker pull buildpack-deps@sha256:8f59fc3d592604d5cf14967c6283ad74901aa8627db618151ffcb0c09eef7438
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
$ docker pull buildpack-deps@sha256:144843b79263f8392a7a29101e618153b8648d20b3ae167eb6f71299266c968d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54289646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7cbab26ac13f5ebd5488c56aa11bf50c91677879ea96874af2cea8de4ac7cf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42950b703a06b97a939a480237f84b19002bdea7a18b13134adc765328699d4d`  
		Last Modified: Tue, 31 Aug 2021 03:16:13 GMT  
		Size: 7.8 MB (7790543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6b8a933b45c85d87d19be1ed2af4f23e53ad900e83ec143c92ec8447adecd2e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46945438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc60af10bb23d073d0363faaaddde45e0816b07e906287177ec75dcf1b38971`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:25:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0c65fb267d23c5dd58ee3a818a8932a3fd565b8db9f6536fe98737a4e08f7`  
		Last Modified: Tue, 31 Aug 2021 03:44:48 GMT  
		Size: 6.6 MB (6631655 bytes)  
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
$ docker pull buildpack-deps@sha256:1ae02049c2770ff1a92e180affdc536ce7756801970085ef122bbc4f2b2e1275
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55216918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a04612f213ecd554c79419d611c43be61dd722d99a45cebb6d945e93f9b9ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:44:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c6ecbb79c70d45fca469278bf60d5e429f108594e71179f4a564aa3531b2d5`  
		Last Modified: Tue, 31 Aug 2021 05:34:20 GMT  
		Size: 7.7 MB (7693285 bytes)  
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
$ docker pull buildpack-deps@sha256:c5af11486ef7c62ee6881e25b65486423adc05dcbd588bb1957c852da5e0e459
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
$ docker pull buildpack-deps@sha256:bdffd3de9058b91bf7ca86dc5d7b9e0028b9d0d894e630f23ef3c283e9e254b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.2 MB (96195328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433417de2a1ffff8b6c87633942faa9c8645ec88f7cb7a47c9a1d5f56b7e96dc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:07:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42950b703a06b97a939a480237f84b19002bdea7a18b13134adc765328699d4d`  
		Last Modified: Tue, 31 Aug 2021 03:16:13 GMT  
		Size: 7.8 MB (7790543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2a7ae66eff85a2438aa0ea3586e8d8d638e66d1b32fe7d59a510cde54c2813`  
		Last Modified: Tue, 31 Aug 2021 03:16:30 GMT  
		Size: 41.9 MB (41905682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:16.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ca27f899fcaf5240abf6e29d84601c0c2def08b179b0441443c49d7d14f1f7a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85107802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49140e977ceeba1edff0140500feec7c945c1838c132e0dc78f30e976313320`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:25:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0c65fb267d23c5dd58ee3a818a8932a3fd565b8db9f6536fe98737a4e08f7`  
		Last Modified: Tue, 31 Aug 2021 03:44:48 GMT  
		Size: 6.6 MB (6631655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ffada20ea8521b2262a77a6239d4fc025f8f59d675a86c60923a075fb73d9d`  
		Last Modified: Tue, 31 Aug 2021 03:45:29 GMT  
		Size: 38.2 MB (38162364 bytes)  
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
$ docker pull buildpack-deps@sha256:b14a5fb51b5d1ab5613940dea0f744f8a26a25e8961fea9dba6e27f06fb42984
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100364186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d669cab791289e0af0fcec78a739743372399e8bea4102312cd5ca1d5f4af1af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:44:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c6ecbb79c70d45fca469278bf60d5e429f108594e71179f4a564aa3531b2d5`  
		Last Modified: Tue, 31 Aug 2021 05:34:20 GMT  
		Size: 7.7 MB (7693285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ba12653da3d4e66d89f4d0e6e7f60832cda0b7b78d6a428c517d0479e4b892`  
		Last Modified: Tue, 31 Aug 2021 05:36:50 GMT  
		Size: 45.1 MB (45147268 bytes)  
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
$ docker pull buildpack-deps@sha256:73f48ef53511ce25f37dc17849fb467925f1bfdcb758c77e8437284158a251ce
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
$ docker pull buildpack-deps@sha256:41b4e8a1508b92a77cf7045b9fb47c2f19ef527d03d3f30abe7526bce3e48af4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221263528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6458e9c218d3fce85ce404a2f799d5ffd8579fa31b6053bf4260112881026ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:50:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:52:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e71f3df86e3a903eda5c8d686f86fe2c6a0d9456f91023cb6d3c167fb0ce09`  
		Last Modified: Tue, 31 Aug 2021 03:11:51 GMT  
		Size: 6.6 MB (6646777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aedf369e8db7b9d55546c93c9df5a8e9a1fb7a16a0e0bbf55dc096e0d37b6d`  
		Last Modified: Tue, 31 Aug 2021 03:11:50 GMT  
		Size: 3.0 MB (3022329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f6e3df075a373e3c582c41a17ca5730a42dfd186de8e9d011beec3c855af55`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 45.5 MB (45477932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5f5b4343ed989bc45e125a14dcb00230352aed1f238158e92fdc727a33a81e`  
		Last Modified: Tue, 31 Aug 2021 03:12:38 GMT  
		Size: 139.4 MB (139407979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2a0a9aedb9391d38f4ff60c2ab26a5f465a326d22176710fc4e5ac81946a09fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189464780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b350369fb87f1ca87b97cdefe796eaffdef079642accdd4e21ca189c118148a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:11:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:11:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3861a2b4b4379b2bb53b663f814026fd5aa82ec17aba9f350a9597ab5273a6`  
		Last Modified: Tue, 31 Aug 2021 03:33:18 GMT  
		Size: 5.7 MB (5717193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb3fa3c4abd05090e6fe2924b1f9dace9c46f49394e0d3c3fb897ce110a718`  
		Last Modified: Tue, 31 Aug 2021 03:33:15 GMT  
		Size: 2.6 MB (2584566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b133473bb2c65d282eb3de44eb03d1d1132609ed4b032096b6e8d19c0ab159f`  
		Last Modified: Tue, 31 Aug 2021 03:33:59 GMT  
		Size: 40.7 MB (40671642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51d4df10b3dbd2670cfa2e40aa12cda1a31890469777cee489197ac586c3c29`  
		Last Modified: Tue, 31 Aug 2021 03:35:23 GMT  
		Size: 118.2 MB (118184900 bytes)  
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
$ docker pull buildpack-deps@sha256:be35398927073fda01415ea00d7b65e109547bfb420e6ee2fe10eaea460312f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246214005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc7badbbabd3507ddd585d388bf12121101dc802cc082d1f326ffa3fd83edb8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:24:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:24:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:27:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:37:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164a2b27f3d3e3338d0cad4aa8917def23b4e4125d8bd35fd92d28d391bd7193`  
		Last Modified: Tue, 31 Aug 2021 05:04:40 GMT  
		Size: 7.1 MB (7059170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c419c8f7c4b804d1eb861ec26eda86aed2a9e66ffe649c93fe1a1729410d58`  
		Last Modified: Tue, 31 Aug 2021 05:04:32 GMT  
		Size: 3.7 MB (3719596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938b10a4ce464230361253a72401f6202439a4d63ec35d261d6ff9149f4649bf`  
		Last Modified: Tue, 31 Aug 2021 05:06:57 GMT  
		Size: 53.7 MB (53715779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d558be345f86c0280cd8bdfeb4b49282bb6a8c0db05c4992c7dc33a0d667803`  
		Last Modified: Tue, 31 Aug 2021 05:11:31 GMT  
		Size: 151.3 MB (151281702 bytes)  
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
$ docker pull buildpack-deps@sha256:818e2a65de79d2b1ce895b82dee48f2417f031718be7c817c4222fcaa95d9231
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
$ docker pull buildpack-deps@sha256:a9631241b02c1eefcb2ed9e572d399da035b2d31ba96f4f920890be9f5c25e3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36377617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab508500278539dcab46cea380406b2f071afc99044b22913e945cdbdd16089`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e71f3df86e3a903eda5c8d686f86fe2c6a0d9456f91023cb6d3c167fb0ce09`  
		Last Modified: Tue, 31 Aug 2021 03:11:51 GMT  
		Size: 6.6 MB (6646777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aedf369e8db7b9d55546c93c9df5a8e9a1fb7a16a0e0bbf55dc096e0d37b6d`  
		Last Modified: Tue, 31 Aug 2021 03:11:50 GMT  
		Size: 3.0 MB (3022329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4de6313c8ce02507698ca93640ec4e1e18f05c5ef8f36d7304a1959577aa390d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30608238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d9546a7fe288db39f65011e7434b7fd870c2a71706fa6dda7e1f332a5b1dc22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:11:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:11:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3861a2b4b4379b2bb53b663f814026fd5aa82ec17aba9f350a9597ab5273a6`  
		Last Modified: Tue, 31 Aug 2021 03:33:18 GMT  
		Size: 5.7 MB (5717193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb3fa3c4abd05090e6fe2924b1f9dace9c46f49394e0d3c3fb897ce110a718`  
		Last Modified: Tue, 31 Aug 2021 03:33:15 GMT  
		Size: 2.6 MB (2584566 bytes)  
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
$ docker pull buildpack-deps@sha256:1eb162f028cf31cde7114fc0f6bb51f1db2dc03e3176d1153990dbde7931382d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41216524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d7639078879437dfa416b3953499bec521d9fff9e701d6679bf281144fd5947`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:24:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:24:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164a2b27f3d3e3338d0cad4aa8917def23b4e4125d8bd35fd92d28d391bd7193`  
		Last Modified: Tue, 31 Aug 2021 05:04:40 GMT  
		Size: 7.1 MB (7059170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c419c8f7c4b804d1eb861ec26eda86aed2a9e66ffe649c93fe1a1729410d58`  
		Last Modified: Tue, 31 Aug 2021 05:04:32 GMT  
		Size: 3.7 MB (3719596 bytes)  
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
$ docker pull buildpack-deps@sha256:b2231828aa5226c1de624816505fa6465490edf506ecccb8cc2beafafb2425ca
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
$ docker pull buildpack-deps@sha256:3508c4792c4e7a6fd510352bb14f9ad537c6c9ff41b89007e91de0a3b7bb5dc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81855549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558d6838e80be090c8d622b10a109a0b67f97a7fd3f0e372bfb9c79dc97e390c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:50:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e71f3df86e3a903eda5c8d686f86fe2c6a0d9456f91023cb6d3c167fb0ce09`  
		Last Modified: Tue, 31 Aug 2021 03:11:51 GMT  
		Size: 6.6 MB (6646777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aedf369e8db7b9d55546c93c9df5a8e9a1fb7a16a0e0bbf55dc096e0d37b6d`  
		Last Modified: Tue, 31 Aug 2021 03:11:50 GMT  
		Size: 3.0 MB (3022329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f6e3df075a373e3c582c41a17ca5730a42dfd186de8e9d011beec3c855af55`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 45.5 MB (45477932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:49e9f28bfc9877d8e8794697518e82825dc28e24ed031ac69edb0e1a65970827
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71279880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86458a097534e95b06eef13c786435c977c4c921862e0408b970a8d6d43d2292`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:11:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:11:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3861a2b4b4379b2bb53b663f814026fd5aa82ec17aba9f350a9597ab5273a6`  
		Last Modified: Tue, 31 Aug 2021 03:33:18 GMT  
		Size: 5.7 MB (5717193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb3fa3c4abd05090e6fe2924b1f9dace9c46f49394e0d3c3fb897ce110a718`  
		Last Modified: Tue, 31 Aug 2021 03:33:15 GMT  
		Size: 2.6 MB (2584566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b133473bb2c65d282eb3de44eb03d1d1132609ed4b032096b6e8d19c0ab159f`  
		Last Modified: Tue, 31 Aug 2021 03:33:59 GMT  
		Size: 40.7 MB (40671642 bytes)  
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
$ docker pull buildpack-deps@sha256:c6ca25bd3d97675c6185c06e5dcad36d82c57c206638e2db2ddee006a3a856c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94932303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00355361f57b82c0833e27d0ca30f7b5b6584bcb6d34a048ea1c6aa45ecf6ac2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:24:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:24:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:27:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164a2b27f3d3e3338d0cad4aa8917def23b4e4125d8bd35fd92d28d391bd7193`  
		Last Modified: Tue, 31 Aug 2021 05:04:40 GMT  
		Size: 7.1 MB (7059170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c419c8f7c4b804d1eb861ec26eda86aed2a9e66ffe649c93fe1a1729410d58`  
		Last Modified: Tue, 31 Aug 2021 05:04:32 GMT  
		Size: 3.7 MB (3719596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938b10a4ce464230361253a72401f6202439a4d63ec35d261d6ff9149f4649bf`  
		Last Modified: Tue, 31 Aug 2021 05:06:57 GMT  
		Size: 53.7 MB (53715779 bytes)  
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
$ docker pull buildpack-deps@sha256:f942c52d1fb8b6331953961709f7ea58df2457ca017d579d607702dae21e12da
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
$ docker pull buildpack-deps@sha256:683c8077722d969d03b468003dfe5a8781396fdbf2da8cc7ed293fd146bb6c31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241806439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f84f61f7cf291360eaf1ca0bf7b39a73b8ed8a565b3ced1f9f61a7164e75761`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:53:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:53:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:57:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1af8c8529138158c1ab9fc21b416a8348bcd120814c9105e5671a61366f1a4`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 7.8 MB (7771403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0df72f91f5e22bfe2c01836dcbb5cded6ba8b11975958672f924786ad44d121`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 3.6 MB (3624569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de940d7df01050bdb7ed77215e5c4ab341f72f7375f15a4463755ab286bc27f3`  
		Last Modified: Tue, 31 Aug 2021 03:13:09 GMT  
		Size: 60.7 MB (60718404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97a35b3662c00e3df90d0a430c5f8e1b47d098f26bf2809569c0453e71bd23f`  
		Last Modified: Tue, 31 Aug 2021 03:13:39 GMT  
		Size: 141.1 MB (141121989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4718fac5e814608335c977561e58a57e08fe828af6a27fe6518b24b9d246902d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207235901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1416b3f4cb8bc1878564692611dd119f31bba74d8498e5baf113b7f3cd7bb879`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:14:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:16:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:17:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c22e0906b4cd7dbb582181e7accbb483c55c760bfd4b2b06e28360279752f8`  
		Last Modified: Tue, 31 Aug 2021 03:35:41 GMT  
		Size: 6.8 MB (6768939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32fb178417438073a96fd01d75df3f32b76e8f1fb7b8dda7e693977a8025b43`  
		Last Modified: Tue, 31 Aug 2021 03:35:38 GMT  
		Size: 3.1 MB (3103787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0210be10f1605c0377e7fff7c8b6f3da7e7c69e756087b20718b4627035213`  
		Last Modified: Tue, 31 Aug 2021 03:36:34 GMT  
		Size: 55.5 MB (55453740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7b29c11815c04ded1d01feff6045c2405b932d7c2efc8af609bbabb13cb243`  
		Last Modified: Tue, 31 Aug 2021 03:37:59 GMT  
		Size: 117.8 MB (117840612 bytes)  
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
$ docker pull buildpack-deps@sha256:e519b10a76931d3242c67d57a628aec5f4e87b4595e1857d3bef0b2f6682058f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.4 MB (265375561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce85cc33f0ebc0dc5502c39e00c609993e0a5c7c28f4b5208f4acd693fee7155`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:40:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:43:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:55:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea9c7aedd6fb1a65cbeb9dbdebba7c78d501eb289eb92d2a11549fdbcac73f`  
		Last Modified: Tue, 31 Aug 2021 05:12:25 GMT  
		Size: 8.7 MB (8725966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4311ec6f0315cc94b2915046b0ea2dd892eece9196a601d82612067c158282`  
		Last Modified: Tue, 31 Aug 2021 05:11:56 GMT  
		Size: 4.5 MB (4456534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feb34377851231e9abee7d1f2f04aab8d35c219fec2687aac4046aae381b19e`  
		Last Modified: Tue, 31 Aug 2021 05:14:33 GMT  
		Size: 69.4 MB (69386748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bbc4692c5fde1d728b1a0b30b861560fcca966924a9939ac9a8a627c4a9522`  
		Last Modified: Tue, 31 Aug 2021 05:18:33 GMT  
		Size: 149.5 MB (149514522 bytes)  
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
$ docker pull buildpack-deps@sha256:0624329af768cbcdc97bb86460cf0d6a5559748c30f8643a9a23d9eb467f9193
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
$ docker pull buildpack-deps@sha256:750e084148cedb701692437bd5ac7648c8a8c151ef3bdd38a7a24fab10c9547b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39966046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fcbf592558a0b39f289c7a26daf7ce442d24b683b93abaee3ce35581337184`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:53:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1af8c8529138158c1ab9fc21b416a8348bcd120814c9105e5671a61366f1a4`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 7.8 MB (7771403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0df72f91f5e22bfe2c01836dcbb5cded6ba8b11975958672f924786ad44d121`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 3.6 MB (3624569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:55fa535446a8e6e8f4d38aabec939003121aa37e1ffec727dc230a00bc1223d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33941549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ed5867781a9efbdb982b87ebdc9d4b7e122304480acbb12b2366cb9a262b7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:14:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c22e0906b4cd7dbb582181e7accbb483c55c760bfd4b2b06e28360279752f8`  
		Last Modified: Tue, 31 Aug 2021 03:35:41 GMT  
		Size: 6.8 MB (6768939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32fb178417438073a96fd01d75df3f32b76e8f1fb7b8dda7e693977a8025b43`  
		Last Modified: Tue, 31 Aug 2021 03:35:38 GMT  
		Size: 3.1 MB (3103787 bytes)  
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
$ docker pull buildpack-deps@sha256:6906d9d9368197b792f3ae55b4002a9bb48c9dc4ff2005828e973956a2d60bea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46474291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0835e68757385fd7dcef70a25271212c73cea8cfb97a3c2be41c9358be6fb56`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:40:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea9c7aedd6fb1a65cbeb9dbdebba7c78d501eb289eb92d2a11549fdbcac73f`  
		Last Modified: Tue, 31 Aug 2021 05:12:25 GMT  
		Size: 8.7 MB (8725966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4311ec6f0315cc94b2915046b0ea2dd892eece9196a601d82612067c158282`  
		Last Modified: Tue, 31 Aug 2021 05:11:56 GMT  
		Size: 4.5 MB (4456534 bytes)  
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
$ docker pull buildpack-deps@sha256:533652c5d770a1d2054633fd5befb427a5e3083313f1e8fa3637b5127a79c5ee
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
$ docker pull buildpack-deps@sha256:8b8b97d300d1bc88549237ed88c7cdf64686a1328ee3a4ab78fbdd1ef5f8da2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100684450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c974b9e6e210580e3ae60d84424224f343c342c509e2c10ad8648f3bd6123cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:53:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:53:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1af8c8529138158c1ab9fc21b416a8348bcd120814c9105e5671a61366f1a4`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 7.8 MB (7771403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0df72f91f5e22bfe2c01836dcbb5cded6ba8b11975958672f924786ad44d121`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 3.6 MB (3624569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de940d7df01050bdb7ed77215e5c4ab341f72f7375f15a4463755ab286bc27f3`  
		Last Modified: Tue, 31 Aug 2021 03:13:09 GMT  
		Size: 60.7 MB (60718404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fc96eae5b17a1509ebd86aec2fc4f5ab815303f932dee306ef7d372ef9d27f73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89395289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2592dcde1e1046cc64d12828ff8273c7be8298f1cd34cdb716f3b31771c3187a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:14:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:16:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c22e0906b4cd7dbb582181e7accbb483c55c760bfd4b2b06e28360279752f8`  
		Last Modified: Tue, 31 Aug 2021 03:35:41 GMT  
		Size: 6.8 MB (6768939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32fb178417438073a96fd01d75df3f32b76e8f1fb7b8dda7e693977a8025b43`  
		Last Modified: Tue, 31 Aug 2021 03:35:38 GMT  
		Size: 3.1 MB (3103787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0210be10f1605c0377e7fff7c8b6f3da7e7c69e756087b20718b4627035213`  
		Last Modified: Tue, 31 Aug 2021 03:36:34 GMT  
		Size: 55.5 MB (55453740 bytes)  
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
$ docker pull buildpack-deps@sha256:c004774b38314517688fc6d7d94f8e6f42c0a8d1039132f47cc28362ddbcf89a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115861039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d7512b0ae7b5e20b692c2aaddd3902fccd66cca69da3d103fe14b95a702faf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:40:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:43:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea9c7aedd6fb1a65cbeb9dbdebba7c78d501eb289eb92d2a11549fdbcac73f`  
		Last Modified: Tue, 31 Aug 2021 05:12:25 GMT  
		Size: 8.7 MB (8725966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4311ec6f0315cc94b2915046b0ea2dd892eece9196a601d82612067c158282`  
		Last Modified: Tue, 31 Aug 2021 05:11:56 GMT  
		Size: 4.5 MB (4456534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feb34377851231e9abee7d1f2f04aab8d35c219fec2687aac4046aae381b19e`  
		Last Modified: Tue, 31 Aug 2021 05:14:33 GMT  
		Size: 69.4 MB (69386748 bytes)  
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
$ docker pull buildpack-deps@sha256:a973b51dffd6768a5c4055c422ec5d667320c9c3c6ee66adb6e0183b42f95bbc
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
$ docker pull buildpack-deps@sha256:ee876b5182702366abacc4e22f28a86fe10dc38d7dd7cb878fe3aa5c2ff2f592
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248811826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afd0b8377ef4379047117c097d974a1716e0a336ccfa034f68ec346f778e5708`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:03 GMT
ADD file:4ac73e113682ef48b7466c4f8765ca7fd54ae98228caa319438a76c35d762b1b in / 
# Tue, 31 Aug 2021 01:21:04 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:57:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:58:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:58:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:02:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7e10407b4d96b1866d5b77b368ac8b2b9b3ef9b210bad0b4784407405121b92`  
		Last Modified: Tue, 31 Aug 2021 01:22:35 GMT  
		Size: 31.7 MB (31703609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2bdc17338d4753c86d8e5520aadb12207bd763dac1f00aa8eb9042fcd88034`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 5.4 MB (5430701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03dd940109a3cc748ce9b671747e7089353d649088e88252f777dcf586a8963`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 3.7 MB (3662065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa3b3922cd293eb3f32aea33d2e5e755a7eae3fce018122e98ef65dd1094a4c`  
		Last Modified: Tue, 31 Aug 2021 03:14:08 GMT  
		Size: 43.5 MB (43541507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c749bf16aecacb19367e45ff9160888d2640ef0ef96d4540fda2a73cad278d`  
		Last Modified: Tue, 31 Aug 2021 03:14:41 GMT  
		Size: 164.5 MB (164473944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1ff7ba11a2f63f4d14d3f50ddd146ecde5b0508600eb4c590f95c80b587bde58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208947575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a963770795b9d8c43ab41d4b55f510efe9f03b2f8352127cbff2d225907b67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:17 GMT
ADD file:cd7671d88520bafabf9a3bea20bd80ee0d2881b895c7f5ce1aaa4958e396074f in / 
# Tue, 31 Aug 2021 01:41:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:18:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:18:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:19:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:21:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:48989deb32eb328d42c26dae334c8da758b723afff40db2647f6780446ec97e8`  
		Last Modified: Tue, 31 Aug 2021 01:45:34 GMT  
		Size: 26.9 MB (26860548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fec9a0a8408a0d36cfa8cb75d2b9e32ea29b69e96c4038df08fc8f06ef52d8b`  
		Last Modified: Tue, 31 Aug 2021 03:38:16 GMT  
		Size: 4.9 MB (4859278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e811318e550593783ac5850dd96d8ac3a3fe682126dabd9493f201cc9f9d0c78`  
		Last Modified: Tue, 31 Aug 2021 03:38:14 GMT  
		Size: 3.1 MB (3138679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36aaae4759daf4d1e91747ae90020318048e7da07cf05181f7ab2f9999eb3ff6`  
		Last Modified: Tue, 31 Aug 2021 03:38:56 GMT  
		Size: 40.0 MB (39953103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe95157c0c6b5402391e23ed75940081585914a4733e580e0d9ba6f2d81fbf2`  
		Last Modified: Tue, 31 Aug 2021 03:40:29 GMT  
		Size: 134.1 MB (134135967 bytes)  
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
$ docker pull buildpack-deps@sha256:058e78da9e2ac970d7448e82c797d473413620255fff6c64cdf88de5f10830a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.1 MB (268065940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb635bb0a138e9db48877563d235b9e64ecbca3ba1667396421a48c2c52b2fa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:57:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:19:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615e5e41d59fe32c6e6c5284994935d713f08ed29bdc3f9841683f0793cf8394`  
		Last Modified: Tue, 31 Aug 2021 05:20:33 GMT  
		Size: 6.2 MB (6155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99aa8209221f270d9ffc050088f6998d6ceefa228f2ca68f9eb5bc410b24fadc`  
		Last Modified: Tue, 31 Aug 2021 05:19:57 GMT  
		Size: 4.5 MB (4523763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e43d357f3322abb3a717de7eaf87420b14cbcae1a2c006e9267578aa7c7881`  
		Last Modified: Tue, 31 Aug 2021 05:22:13 GMT  
		Size: 49.5 MB (49467214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c991a658b76da93bd82aa1b744de18c388c34d14ed61e2ec281aed8ac7bd7b9e`  
		Last Modified: Tue, 31 Aug 2021 05:27:03 GMT  
		Size: 170.7 MB (170733574 bytes)  
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
$ docker pull buildpack-deps@sha256:ff1b1d9dc00dadeca39b39907fcd12af254500e39e8c65acf9ea9c60ecfbdf7b
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
$ docker pull buildpack-deps@sha256:38c9947bebf08bf338214a9539d13131ceceef2eb56a3a962fd487d03a4a48ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd9b43ff77c32f2171be9117ae172526d0bbc561da8f7525f999efc126f5eb09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:03 GMT
ADD file:4ac73e113682ef48b7466c4f8765ca7fd54ae98228caa319438a76c35d762b1b in / 
# Tue, 31 Aug 2021 01:21:04 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:57:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:58:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d7e10407b4d96b1866d5b77b368ac8b2b9b3ef9b210bad0b4784407405121b92`  
		Last Modified: Tue, 31 Aug 2021 01:22:35 GMT  
		Size: 31.7 MB (31703609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2bdc17338d4753c86d8e5520aadb12207bd763dac1f00aa8eb9042fcd88034`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 5.4 MB (5430701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03dd940109a3cc748ce9b671747e7089353d649088e88252f777dcf586a8963`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 3.7 MB (3662065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d61014dc4d388d078b9c36260a7cc23617d103342e7e04975cedb5f704468fda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34858505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c935c4d2289718675e23151e3e67200070942fbce6e4b507ddff7a679fbdec1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:17 GMT
ADD file:cd7671d88520bafabf9a3bea20bd80ee0d2881b895c7f5ce1aaa4958e396074f in / 
# Tue, 31 Aug 2021 01:41:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:18:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:18:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:48989deb32eb328d42c26dae334c8da758b723afff40db2647f6780446ec97e8`  
		Last Modified: Tue, 31 Aug 2021 01:45:34 GMT  
		Size: 26.9 MB (26860548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fec9a0a8408a0d36cfa8cb75d2b9e32ea29b69e96c4038df08fc8f06ef52d8b`  
		Last Modified: Tue, 31 Aug 2021 03:38:16 GMT  
		Size: 4.9 MB (4859278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e811318e550593783ac5850dd96d8ac3a3fe682126dabd9493f201cc9f9d0c78`  
		Last Modified: Tue, 31 Aug 2021 03:38:14 GMT  
		Size: 3.1 MB (3138679 bytes)  
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
$ docker pull buildpack-deps@sha256:b93bc595a55dddf7b45d8d5ac826b9ff698374ac6f9058ef103104b9f0f85926
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47865152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd812682377fde30cb7af2ebe1f69410167761e73b69535b5e0a2cd6e9411295`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:57:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615e5e41d59fe32c6e6c5284994935d713f08ed29bdc3f9841683f0793cf8394`  
		Last Modified: Tue, 31 Aug 2021 05:20:33 GMT  
		Size: 6.2 MB (6155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99aa8209221f270d9ffc050088f6998d6ceefa228f2ca68f9eb5bc410b24fadc`  
		Last Modified: Tue, 31 Aug 2021 05:19:57 GMT  
		Size: 4.5 MB (4523763 bytes)  
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
$ docker pull buildpack-deps@sha256:0e63d7d04671f447f35c721d0cc0329e2e6bbf0421f4b74e8e0ed0f9c7abcc7e
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
$ docker pull buildpack-deps@sha256:53963b8dedc84f611319c16f86c364bb1ade2088bd39dcffef7bc047e2606111
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.3 MB (84337882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:070fc06a5156d80575b1bd08707831468912b0a8af4a60a8ddbbac20d0f8acde`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:03 GMT
ADD file:4ac73e113682ef48b7466c4f8765ca7fd54ae98228caa319438a76c35d762b1b in / 
# Tue, 31 Aug 2021 01:21:04 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:57:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:58:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:58:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7e10407b4d96b1866d5b77b368ac8b2b9b3ef9b210bad0b4784407405121b92`  
		Last Modified: Tue, 31 Aug 2021 01:22:35 GMT  
		Size: 31.7 MB (31703609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2bdc17338d4753c86d8e5520aadb12207bd763dac1f00aa8eb9042fcd88034`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 5.4 MB (5430701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03dd940109a3cc748ce9b671747e7089353d649088e88252f777dcf586a8963`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 3.7 MB (3662065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa3b3922cd293eb3f32aea33d2e5e755a7eae3fce018122e98ef65dd1094a4c`  
		Last Modified: Tue, 31 Aug 2021 03:14:08 GMT  
		Size: 43.5 MB (43541507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2e03a791f00acdebdb202ef33d78e6946ecbbabb9b3e2a6b6c42d561a9504308
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74811608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fa7a2751d29365ef5f45ca3f55897eea12bb3795441d0f5ccba9ce32318a043`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:17 GMT
ADD file:cd7671d88520bafabf9a3bea20bd80ee0d2881b895c7f5ce1aaa4958e396074f in / 
# Tue, 31 Aug 2021 01:41:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:18:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:18:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:19:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:48989deb32eb328d42c26dae334c8da758b723afff40db2647f6780446ec97e8`  
		Last Modified: Tue, 31 Aug 2021 01:45:34 GMT  
		Size: 26.9 MB (26860548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fec9a0a8408a0d36cfa8cb75d2b9e32ea29b69e96c4038df08fc8f06ef52d8b`  
		Last Modified: Tue, 31 Aug 2021 03:38:16 GMT  
		Size: 4.9 MB (4859278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e811318e550593783ac5850dd96d8ac3a3fe682126dabd9493f201cc9f9d0c78`  
		Last Modified: Tue, 31 Aug 2021 03:38:14 GMT  
		Size: 3.1 MB (3138679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36aaae4759daf4d1e91747ae90020318048e7da07cf05181f7ab2f9999eb3ff6`  
		Last Modified: Tue, 31 Aug 2021 03:38:56 GMT  
		Size: 40.0 MB (39953103 bytes)  
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
$ docker pull buildpack-deps@sha256:08c18882a70aad8af2599f0170a98f8c20db30a91fcc5a77d3b043e5bfc7614c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.3 MB (97332366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5211c4bfed288ada093bfbb9e2f58c5f291103d5c360755d5ac8be047e188f50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:57:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615e5e41d59fe32c6e6c5284994935d713f08ed29bdc3f9841683f0793cf8394`  
		Last Modified: Tue, 31 Aug 2021 05:20:33 GMT  
		Size: 6.2 MB (6155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99aa8209221f270d9ffc050088f6998d6ceefa228f2ca68f9eb5bc410b24fadc`  
		Last Modified: Tue, 31 Aug 2021 05:19:57 GMT  
		Size: 4.5 MB (4523763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e43d357f3322abb3a717de7eaf87420b14cbcae1a2c006e9267578aa7c7881`  
		Last Modified: Tue, 31 Aug 2021 05:22:13 GMT  
		Size: 49.5 MB (49467214 bytes)  
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
$ docker pull buildpack-deps@sha256:b6112899295bc4ee493ef3e21ee6ef732d267ed29af52121df1810f1838d1093
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
$ docker pull buildpack-deps@sha256:9af39729d3d63f5797c785605e9c26effbfb09444ef91f5bd0099e5827edd880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.9 MB (406868171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa7f2e7a9355bb02a5478b27f15892dda84f9277790d6bf142f99d5982080d53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:12 GMT
ADD file:355a5f56bf0136597bcd90b01ff73fc517b6bf7e76f45b65bf1af1136f434462 in / 
# Tue, 31 Aug 2021 01:21:12 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:03:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:05:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25907b3add375d4f44a3bf4bfc3544b51ff9f4a23fe8c186f3b20e54b37d19ae`  
		Last Modified: Tue, 31 Aug 2021 01:22:53 GMT  
		Size: 30.6 MB (30602781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ef40c83a42d65ce37ce8bc08e06a0c4b994512527cad13196aca51586d9bd7`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.7 MB (3692694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871edcbb988433606f5a8d03efc8f0d9d49a4cd78a5d506401ec3b7854a2162`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.6 MB (3552016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59778cb761facf0aaa7ff7cab370d47bdee8a1c0764186ec8286f50fb911a78b`  
		Last Modified: Tue, 31 Aug 2021 03:15:08 GMT  
		Size: 38.1 MB (38114895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffa26f12ed647c5e1c9898915298f9e7389c733e2825bad35dac65a6b529755`  
		Last Modified: Tue, 31 Aug 2021 03:16:00 GMT  
		Size: 330.9 MB (330905785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b4cd810e63cec40720081b46d9f7d51f6879f979f24a21782c183d6cdf2533d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.3 MB (371327940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea1b0d70c3fe313e6e52e4f870b7ec6ddf510caa3a0accad930efba05e6b01b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:42 GMT
ADD file:0abcd0c1c6aecb3d5af2aa5d9c631949d716076e338faccdd7802906b4979bd6 in / 
# Tue, 31 Aug 2021 01:41:43 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:21:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:22:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:22:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:24:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be5e7fb59932c05a5acf0221847ae12179d4f81037fdeb44f8c408bc27ec1511`  
		Last Modified: Tue, 31 Aug 2021 01:46:11 GMT  
		Size: 27.3 MB (27313903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c8f5e7395b48e26211a363f2c66ea0e729fa5f4ce1e980a22a70c47eacbf1`  
		Last Modified: Tue, 31 Aug 2021 03:40:47 GMT  
		Size: 3.4 MB (3438915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30125ee4f15b1f56a8279e5c1f488ef77c51231b62f4da3cb1a03b8a32fdae7`  
		Last Modified: Tue, 31 Aug 2021 03:40:46 GMT  
		Size: 3.7 MB (3742231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01de5d75b44b35b6f46117f4d1484f24b516edeed132dc1815d6a78fb0cbbd6`  
		Last Modified: Tue, 31 Aug 2021 03:41:28 GMT  
		Size: 40.3 MB (40317890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061c3e4e41e25d781afd762c7e0519095f1075b1d9504f209328e2b477700b75`  
		Last Modified: Tue, 31 Aug 2021 03:44:30 GMT  
		Size: 296.5 MB (296515001 bytes)  
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
$ docker pull buildpack-deps@sha256:2be72be9ca82b6475c433d3069b67ee4c9d76f0bf162b5d92392859509e87877
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413058139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef497b78fbb6c17ea0698512be7ab72912b9c4103be39f07db90a3ade98dd07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:28 GMT
ADD file:776487dfd6a31c5a5d57d6924dd11136cb94d2e661eb085c76b14213c2220e3f in / 
# Tue, 31 Aug 2021 02:11:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:21:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:23:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:42:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f23233eca55841e558566a0a689d1261b17a023a5d0ed1e0ee267da33ff84a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:11 GMT  
		Size: 36.1 MB (36055099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10a1f2d8a9c3bf4f6060f088986f3f74fbf50acda4d6016dfd6d1115fbf3a9d`  
		Last Modified: Tue, 31 Aug 2021 05:27:38 GMT  
		Size: 4.1 MB (4096829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26809db5804495bc5bf81be1fbeae7b7a82215d30ff3e0c59d3353cc857206`  
		Last Modified: Tue, 31 Aug 2021 05:27:21 GMT  
		Size: 4.2 MB (4241626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671fe0a2b7c06f1e3c899f5ad9e8b89dbbef68ba1f5bc446f05beaeca064dd31`  
		Last Modified: Tue, 31 Aug 2021 05:29:18 GMT  
		Size: 42.6 MB (42605912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9257fa229b5f286c331fe7b926deef3aee7709c3b87ae22f5cd31d4efc1765`  
		Last Modified: Tue, 31 Aug 2021 05:33:16 GMT  
		Size: 326.1 MB (326058673 bytes)  
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
$ docker pull buildpack-deps@sha256:40969d345ea67b862a72d9d24144395ddea299a517a4c456f060cf108f177c84
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
$ docker pull buildpack-deps@sha256:dd6c280b99daea86543d074f477b5b196e3136433686b6848dc654663bb60e58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37847491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883360346d84b6140d17a89c82dded9c76d0c86eda04909badf532a6d40fcfd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:12 GMT
ADD file:355a5f56bf0136597bcd90b01ff73fc517b6bf7e76f45b65bf1af1136f434462 in / 
# Tue, 31 Aug 2021 01:21:12 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:03:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:25907b3add375d4f44a3bf4bfc3544b51ff9f4a23fe8c186f3b20e54b37d19ae`  
		Last Modified: Tue, 31 Aug 2021 01:22:53 GMT  
		Size: 30.6 MB (30602781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ef40c83a42d65ce37ce8bc08e06a0c4b994512527cad13196aca51586d9bd7`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.7 MB (3692694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871edcbb988433606f5a8d03efc8f0d9d49a4cd78a5d506401ec3b7854a2162`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.6 MB (3552016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9a3d5880ea36b8866fa5d8f9d4b3604048c83a329f3e4a4ea6aba5eed872f1fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34495049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e2e9a9304e887c58fb5516661169e2e18ea005307279c2d8d325a22f638621`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:42 GMT
ADD file:0abcd0c1c6aecb3d5af2aa5d9c631949d716076e338faccdd7802906b4979bd6 in / 
# Tue, 31 Aug 2021 01:41:43 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:21:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:22:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be5e7fb59932c05a5acf0221847ae12179d4f81037fdeb44f8c408bc27ec1511`  
		Last Modified: Tue, 31 Aug 2021 01:46:11 GMT  
		Size: 27.3 MB (27313903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c8f5e7395b48e26211a363f2c66ea0e729fa5f4ce1e980a22a70c47eacbf1`  
		Last Modified: Tue, 31 Aug 2021 03:40:47 GMT  
		Size: 3.4 MB (3438915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30125ee4f15b1f56a8279e5c1f488ef77c51231b62f4da3cb1a03b8a32fdae7`  
		Last Modified: Tue, 31 Aug 2021 03:40:46 GMT  
		Size: 3.7 MB (3742231 bytes)  
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
$ docker pull buildpack-deps@sha256:838cee7286d3baa3d78a9117036d5697643c8db2337680cedb6d584405b7ba53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44393554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c7088c04b44397a9f243f59f8046529d76d35591ab07d0f3564045047c59cd2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:28 GMT
ADD file:776487dfd6a31c5a5d57d6924dd11136cb94d2e661eb085c76b14213c2220e3f in / 
# Tue, 31 Aug 2021 02:11:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:21:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7f23233eca55841e558566a0a689d1261b17a023a5d0ed1e0ee267da33ff84a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:11 GMT  
		Size: 36.1 MB (36055099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10a1f2d8a9c3bf4f6060f088986f3f74fbf50acda4d6016dfd6d1115fbf3a9d`  
		Last Modified: Tue, 31 Aug 2021 05:27:38 GMT  
		Size: 4.1 MB (4096829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26809db5804495bc5bf81be1fbeae7b7a82215d30ff3e0c59d3353cc857206`  
		Last Modified: Tue, 31 Aug 2021 05:27:21 GMT  
		Size: 4.2 MB (4241626 bytes)  
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
$ docker pull buildpack-deps@sha256:f5326c47df09b079464b892d20fd05a3aadbc1575839f1804e8fedc6aba2e4ab
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
$ docker pull buildpack-deps@sha256:f68d3b481c199cba164a796afe4f6c460293fe1810d2bd5fc323bedca9db34e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75962386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edb492d2fe194b03eeee021b94668fa6d5019b08c3d8a268a8145465c35158d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:12 GMT
ADD file:355a5f56bf0136597bcd90b01ff73fc517b6bf7e76f45b65bf1af1136f434462 in / 
# Tue, 31 Aug 2021 01:21:12 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:03:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25907b3add375d4f44a3bf4bfc3544b51ff9f4a23fe8c186f3b20e54b37d19ae`  
		Last Modified: Tue, 31 Aug 2021 01:22:53 GMT  
		Size: 30.6 MB (30602781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ef40c83a42d65ce37ce8bc08e06a0c4b994512527cad13196aca51586d9bd7`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.7 MB (3692694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871edcbb988433606f5a8d03efc8f0d9d49a4cd78a5d506401ec3b7854a2162`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.6 MB (3552016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59778cb761facf0aaa7ff7cab370d47bdee8a1c0764186ec8286f50fb911a78b`  
		Last Modified: Tue, 31 Aug 2021 03:15:08 GMT  
		Size: 38.1 MB (38114895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eb7e85f3681ff91b3c2ad5df257554ba0bed79851ceb90c2bdd39bd717ebdee1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74812939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a076702ca7e06d53c2bf037f5a9e46dd84724a6de0ee98774d147661533654`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:42 GMT
ADD file:0abcd0c1c6aecb3d5af2aa5d9c631949d716076e338faccdd7802906b4979bd6 in / 
# Tue, 31 Aug 2021 01:41:43 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:21:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:22:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:22:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be5e7fb59932c05a5acf0221847ae12179d4f81037fdeb44f8c408bc27ec1511`  
		Last Modified: Tue, 31 Aug 2021 01:46:11 GMT  
		Size: 27.3 MB (27313903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c8f5e7395b48e26211a363f2c66ea0e729fa5f4ce1e980a22a70c47eacbf1`  
		Last Modified: Tue, 31 Aug 2021 03:40:47 GMT  
		Size: 3.4 MB (3438915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30125ee4f15b1f56a8279e5c1f488ef77c51231b62f4da3cb1a03b8a32fdae7`  
		Last Modified: Tue, 31 Aug 2021 03:40:46 GMT  
		Size: 3.7 MB (3742231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01de5d75b44b35b6f46117f4d1484f24b516edeed132dc1815d6a78fb0cbbd6`  
		Last Modified: Tue, 31 Aug 2021 03:41:28 GMT  
		Size: 40.3 MB (40317890 bytes)  
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
$ docker pull buildpack-deps@sha256:5842de42899adb406caffa3d495ad51cfc06dd3bf5ec1eb8022df11e29c74efd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86999466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ff5b2bb66e5ad11a8cdfc7a5f24440425e23f96b465dd30a510fe40c40ee67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:28 GMT
ADD file:776487dfd6a31c5a5d57d6924dd11136cb94d2e661eb085c76b14213c2220e3f in / 
# Tue, 31 Aug 2021 02:11:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:21:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:23:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f23233eca55841e558566a0a689d1261b17a023a5d0ed1e0ee267da33ff84a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:11 GMT  
		Size: 36.1 MB (36055099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10a1f2d8a9c3bf4f6060f088986f3f74fbf50acda4d6016dfd6d1115fbf3a9d`  
		Last Modified: Tue, 31 Aug 2021 05:27:38 GMT  
		Size: 4.1 MB (4096829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26809db5804495bc5bf81be1fbeae7b7a82215d30ff3e0c59d3353cc857206`  
		Last Modified: Tue, 31 Aug 2021 05:27:21 GMT  
		Size: 4.2 MB (4241626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671fe0a2b7c06f1e3c899f5ad9e8b89dbbef68ba1f5bc446f05beaeca064dd31`  
		Last Modified: Tue, 31 Aug 2021 05:29:18 GMT  
		Size: 42.6 MB (42605912 bytes)  
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
$ docker pull buildpack-deps@sha256:73f48ef53511ce25f37dc17849fb467925f1bfdcb758c77e8437284158a251ce
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
$ docker pull buildpack-deps@sha256:41b4e8a1508b92a77cf7045b9fb47c2f19ef527d03d3f30abe7526bce3e48af4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221263528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6458e9c218d3fce85ce404a2f799d5ffd8579fa31b6053bf4260112881026ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:50:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:52:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e71f3df86e3a903eda5c8d686f86fe2c6a0d9456f91023cb6d3c167fb0ce09`  
		Last Modified: Tue, 31 Aug 2021 03:11:51 GMT  
		Size: 6.6 MB (6646777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aedf369e8db7b9d55546c93c9df5a8e9a1fb7a16a0e0bbf55dc096e0d37b6d`  
		Last Modified: Tue, 31 Aug 2021 03:11:50 GMT  
		Size: 3.0 MB (3022329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f6e3df075a373e3c582c41a17ca5730a42dfd186de8e9d011beec3c855af55`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 45.5 MB (45477932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5f5b4343ed989bc45e125a14dcb00230352aed1f238158e92fdc727a33a81e`  
		Last Modified: Tue, 31 Aug 2021 03:12:38 GMT  
		Size: 139.4 MB (139407979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2a0a9aedb9391d38f4ff60c2ab26a5f465a326d22176710fc4e5ac81946a09fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189464780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b350369fb87f1ca87b97cdefe796eaffdef079642accdd4e21ca189c118148a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:11:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:11:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3861a2b4b4379b2bb53b663f814026fd5aa82ec17aba9f350a9597ab5273a6`  
		Last Modified: Tue, 31 Aug 2021 03:33:18 GMT  
		Size: 5.7 MB (5717193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb3fa3c4abd05090e6fe2924b1f9dace9c46f49394e0d3c3fb897ce110a718`  
		Last Modified: Tue, 31 Aug 2021 03:33:15 GMT  
		Size: 2.6 MB (2584566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b133473bb2c65d282eb3de44eb03d1d1132609ed4b032096b6e8d19c0ab159f`  
		Last Modified: Tue, 31 Aug 2021 03:33:59 GMT  
		Size: 40.7 MB (40671642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51d4df10b3dbd2670cfa2e40aa12cda1a31890469777cee489197ac586c3c29`  
		Last Modified: Tue, 31 Aug 2021 03:35:23 GMT  
		Size: 118.2 MB (118184900 bytes)  
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
$ docker pull buildpack-deps@sha256:be35398927073fda01415ea00d7b65e109547bfb420e6ee2fe10eaea460312f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246214005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc7badbbabd3507ddd585d388bf12121101dc802cc082d1f326ffa3fd83edb8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:24:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:24:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:27:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:37:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164a2b27f3d3e3338d0cad4aa8917def23b4e4125d8bd35fd92d28d391bd7193`  
		Last Modified: Tue, 31 Aug 2021 05:04:40 GMT  
		Size: 7.1 MB (7059170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c419c8f7c4b804d1eb861ec26eda86aed2a9e66ffe649c93fe1a1729410d58`  
		Last Modified: Tue, 31 Aug 2021 05:04:32 GMT  
		Size: 3.7 MB (3719596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938b10a4ce464230361253a72401f6202439a4d63ec35d261d6ff9149f4649bf`  
		Last Modified: Tue, 31 Aug 2021 05:06:57 GMT  
		Size: 53.7 MB (53715779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d558be345f86c0280cd8bdfeb4b49282bb6a8c0db05c4992c7dc33a0d667803`  
		Last Modified: Tue, 31 Aug 2021 05:11:31 GMT  
		Size: 151.3 MB (151281702 bytes)  
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
$ docker pull buildpack-deps@sha256:818e2a65de79d2b1ce895b82dee48f2417f031718be7c817c4222fcaa95d9231
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
$ docker pull buildpack-deps@sha256:a9631241b02c1eefcb2ed9e572d399da035b2d31ba96f4f920890be9f5c25e3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36377617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab508500278539dcab46cea380406b2f071afc99044b22913e945cdbdd16089`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e71f3df86e3a903eda5c8d686f86fe2c6a0d9456f91023cb6d3c167fb0ce09`  
		Last Modified: Tue, 31 Aug 2021 03:11:51 GMT  
		Size: 6.6 MB (6646777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aedf369e8db7b9d55546c93c9df5a8e9a1fb7a16a0e0bbf55dc096e0d37b6d`  
		Last Modified: Tue, 31 Aug 2021 03:11:50 GMT  
		Size: 3.0 MB (3022329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4de6313c8ce02507698ca93640ec4e1e18f05c5ef8f36d7304a1959577aa390d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30608238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d9546a7fe288db39f65011e7434b7fd870c2a71706fa6dda7e1f332a5b1dc22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:11:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:11:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3861a2b4b4379b2bb53b663f814026fd5aa82ec17aba9f350a9597ab5273a6`  
		Last Modified: Tue, 31 Aug 2021 03:33:18 GMT  
		Size: 5.7 MB (5717193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb3fa3c4abd05090e6fe2924b1f9dace9c46f49394e0d3c3fb897ce110a718`  
		Last Modified: Tue, 31 Aug 2021 03:33:15 GMT  
		Size: 2.6 MB (2584566 bytes)  
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
$ docker pull buildpack-deps@sha256:1eb162f028cf31cde7114fc0f6bb51f1db2dc03e3176d1153990dbde7931382d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41216524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d7639078879437dfa416b3953499bec521d9fff9e701d6679bf281144fd5947`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:24:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:24:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164a2b27f3d3e3338d0cad4aa8917def23b4e4125d8bd35fd92d28d391bd7193`  
		Last Modified: Tue, 31 Aug 2021 05:04:40 GMT  
		Size: 7.1 MB (7059170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c419c8f7c4b804d1eb861ec26eda86aed2a9e66ffe649c93fe1a1729410d58`  
		Last Modified: Tue, 31 Aug 2021 05:04:32 GMT  
		Size: 3.7 MB (3719596 bytes)  
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
$ docker pull buildpack-deps@sha256:b2231828aa5226c1de624816505fa6465490edf506ecccb8cc2beafafb2425ca
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
$ docker pull buildpack-deps@sha256:3508c4792c4e7a6fd510352bb14f9ad537c6c9ff41b89007e91de0a3b7bb5dc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81855549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558d6838e80be090c8d622b10a109a0b67f97a7fd3f0e372bfb9c79dc97e390c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:49:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:49:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:50:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e71f3df86e3a903eda5c8d686f86fe2c6a0d9456f91023cb6d3c167fb0ce09`  
		Last Modified: Tue, 31 Aug 2021 03:11:51 GMT  
		Size: 6.6 MB (6646777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aedf369e8db7b9d55546c93c9df5a8e9a1fb7a16a0e0bbf55dc096e0d37b6d`  
		Last Modified: Tue, 31 Aug 2021 03:11:50 GMT  
		Size: 3.0 MB (3022329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f6e3df075a373e3c582c41a17ca5730a42dfd186de8e9d011beec3c855af55`  
		Last Modified: Tue, 31 Aug 2021 03:12:08 GMT  
		Size: 45.5 MB (45477932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:49e9f28bfc9877d8e8794697518e82825dc28e24ed031ac69edb0e1a65970827
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71279880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86458a097534e95b06eef13c786435c977c4c921862e0408b970a8d6d43d2292`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:11:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:11:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3861a2b4b4379b2bb53b663f814026fd5aa82ec17aba9f350a9597ab5273a6`  
		Last Modified: Tue, 31 Aug 2021 03:33:18 GMT  
		Size: 5.7 MB (5717193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb3fa3c4abd05090e6fe2924b1f9dace9c46f49394e0d3c3fb897ce110a718`  
		Last Modified: Tue, 31 Aug 2021 03:33:15 GMT  
		Size: 2.6 MB (2584566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b133473bb2c65d282eb3de44eb03d1d1132609ed4b032096b6e8d19c0ab159f`  
		Last Modified: Tue, 31 Aug 2021 03:33:59 GMT  
		Size: 40.7 MB (40671642 bytes)  
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
$ docker pull buildpack-deps@sha256:c6ca25bd3d97675c6185c06e5dcad36d82c57c206638e2db2ddee006a3a856c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94932303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00355361f57b82c0833e27d0ca30f7b5b6584bcb6d34a048ea1c6aa45ecf6ac2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:24:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:24:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:27:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164a2b27f3d3e3338d0cad4aa8917def23b4e4125d8bd35fd92d28d391bd7193`  
		Last Modified: Tue, 31 Aug 2021 05:04:40 GMT  
		Size: 7.1 MB (7059170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c419c8f7c4b804d1eb861ec26eda86aed2a9e66ffe649c93fe1a1729410d58`  
		Last Modified: Tue, 31 Aug 2021 05:04:32 GMT  
		Size: 3.7 MB (3719596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938b10a4ce464230361253a72401f6202439a4d63ec35d261d6ff9149f4649bf`  
		Last Modified: Tue, 31 Aug 2021 05:06:57 GMT  
		Size: 53.7 MB (53715779 bytes)  
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
$ docker pull buildpack-deps@sha256:f6c911ff12af5e812a96df5b24fc67cc7d2924c07d13d52f9d3ee90fc9f8b81c
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
$ docker pull buildpack-deps@sha256:9b65dde79ee2e03922f844db61fb0dd2e97297df7ab620ead878c347744f430c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295058728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6bab944fcaa224ed17b83c9812ae6117a5f28d269b0b0477135bb05e601420e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:31:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:32:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:34:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f9763e0efd7dcf980819e39cb728c9f11f3c3f7dd944e21177efba57f6fe3`  
		Last Modified: Fri, 03 Sep 2021 02:51:03 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95efca74ef694ced85d684e7faecd407beb97667568054d98e5e09166a32d88a`  
		Last Modified: Fri, 03 Sep 2021 02:51:05 GMT  
		Size: 10.6 MB (10570971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df2396712ed6cf1ebf81db19d8e162b1c621c3fca9971be211747d7e10bf8`  
		Last Modified: Fri, 03 Sep 2021 02:51:58 GMT  
		Size: 52.3 MB (52319329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0847f5ab2d0f284ff33db1f85872a599e314abb845aaab72c0e9a3e57a063c96`  
		Last Modified: Fri, 03 Sep 2021 02:54:01 GMT  
		Size: 174.6 MB (174643286 bytes)  
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
$ docker pull buildpack-deps@sha256:0eeacd7d46019ece9dda8918d9976ff85578d8108a73ac7ed44ff3cc3aa32fe1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327743866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6fcb7ffe5e59562a791d18986a198b675f7b171f4eeaa206755542198904057`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853d83532467d1599448d38360ea9d52789d7d10f30c6734e17728c98743435b`  
		Last Modified: Fri, 03 Sep 2021 01:19:38 GMT  
		Size: 5.3 MB (5282881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6935e9ec29feb2101753d15eca8fa2727e2b060c07d2f720f471c55fb344c2a4`  
		Last Modified: Fri, 03 Sep 2021 01:19:39 GMT  
		Size: 11.3 MB (11250633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf6b2b625a6c874fcfb0e659f71235906f8459aa36ce32066b8efe1daf7c855`  
		Last Modified: Fri, 03 Sep 2021 01:20:07 GMT  
		Size: 55.9 MB (55916333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626b405c2848d11cb9e5ff331bbdc4a25b3874bca022fb01d015d9cc9f417cc8`  
		Last Modified: Fri, 03 Sep 2021 01:21:03 GMT  
		Size: 199.4 MB (199363086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4cbe9b6745b5af922a656e1d62acd8a038f7fd8d380e564bbdb7b25b95595ace
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301401029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd513018a9e3b431230adc2461695e8f74bd2b65f6e8645e4509f58f77252e9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:46:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:48:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918f43385735f5455e955ef94ef61f2089c0caebab840605cb52e5dd7525cd4`  
		Last Modified: Fri, 03 Sep 2021 01:59:04 GMT  
		Size: 53.3 MB (53297975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65f346af31b808f018e37721ec5d0556c4de13c57d89116afa4b6828afe09c5`  
		Last Modified: Fri, 03 Sep 2021 02:01:15 GMT  
		Size: 178.9 MB (178937584 bytes)  
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
$ docker pull buildpack-deps@sha256:40197898caa51e4f5c2a304bd81d55820af4a1476de2a1a330d051d454943f57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295584326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af2f830a774ba7fd46337da52dbfe51265f7563bc6cce99f5c38ad75cf30c14`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:07:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f48d5133e49359781fde1a8e72c81879ba30ffcb5b6d759f0ecb28fe6bbbe8`  
		Last Modified: Fri, 03 Sep 2021 02:19:40 GMT  
		Size: 5.1 MB (5137216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab672e8b32c6e3623bde683097d4c5fe5a73090dcb963e9f5512dfc21c485f58`  
		Last Modified: Fri, 03 Sep 2021 02:19:41 GMT  
		Size: 10.8 MB (10761458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7068e3642fc5ba5e489f8857ba725ba64ef0ce4b28acbf1545d133584bae2`  
		Last Modified: Fri, 03 Sep 2021 02:19:59 GMT  
		Size: 54.1 MB (54050487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02058994960995fa08f9f85746bee63cac5d73869afec780cbf963e361fe892`  
		Last Modified: Fri, 03 Sep 2021 02:20:31 GMT  
		Size: 172.4 MB (172434011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:ae9619a5c3c818d5149c0130318f141746acf3f6a1a24b58383ff902654a83e8
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
$ docker pull buildpack-deps@sha256:c1bf509fa76457be540f8f2fb10d9d26aa4890c9a4346c713745b6206fdda4be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68096113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73cdc4ca1ff77a007de35ea79cc9c08626250d2979cb0558df1bac7e1abd8c70`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:31:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f9763e0efd7dcf980819e39cb728c9f11f3c3f7dd944e21177efba57f6fe3`  
		Last Modified: Fri, 03 Sep 2021 02:51:03 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95efca74ef694ced85d684e7faecd407beb97667568054d98e5e09166a32d88a`  
		Last Modified: Fri, 03 Sep 2021 02:51:05 GMT  
		Size: 10.6 MB (10570971 bytes)  
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
$ docker pull buildpack-deps@sha256:ca1f95f69b1217eedf8fd5df25b029787d2b20be1c3808d4b56a7809cfafb72e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72464447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5250d94db9c58649245be60756b66f56ad4035644a1d6f28e3abd1e9e21ec49a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853d83532467d1599448d38360ea9d52789d7d10f30c6734e17728c98743435b`  
		Last Modified: Fri, 03 Sep 2021 01:19:38 GMT  
		Size: 5.3 MB (5282881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6935e9ec29feb2101753d15eca8fa2727e2b060c07d2f720f471c55fb344c2a4`  
		Last Modified: Fri, 03 Sep 2021 01:19:39 GMT  
		Size: 11.3 MB (11250633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1a5a8c8829bff1d7a89f8d97006a6ea359c46bb260fe809df4e907b5afd30a91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69165470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e5a9049a5620e106a070b8340f0b607aa86268008ceffc8ca4c29af118cfa3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
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
$ docker pull buildpack-deps@sha256:28124d888ebc509c072830169a01df6f23dcbbc8d88409f6aa3510b89267f1e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69099828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4861250614c542c631365e5d324fc1d562da14639c4308cea90abf09db002747`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f48d5133e49359781fde1a8e72c81879ba30ffcb5b6d759f0ecb28fe6bbbe8`  
		Last Modified: Fri, 03 Sep 2021 02:19:40 GMT  
		Size: 5.1 MB (5137216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab672e8b32c6e3623bde683097d4c5fe5a73090dcb963e9f5512dfc21c485f58`  
		Last Modified: Fri, 03 Sep 2021 02:19:41 GMT  
		Size: 10.8 MB (10761458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:48885a657fa24cd5afeda8c2cbdf0574e118c803fa71d6222275d03343dd73fc
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
$ docker pull buildpack-deps@sha256:25400321d2573328a3a4a5ca398f3e0d11056d903e39f334939e80717fd8127d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120415442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c9ec9c2d5a6c44f4f20dee32d5687a7f6699b5ad60a5fd9da4530f37f0f010`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:31:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:32:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f9763e0efd7dcf980819e39cb728c9f11f3c3f7dd944e21177efba57f6fe3`  
		Last Modified: Fri, 03 Sep 2021 02:51:03 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95efca74ef694ced85d684e7faecd407beb97667568054d98e5e09166a32d88a`  
		Last Modified: Fri, 03 Sep 2021 02:51:05 GMT  
		Size: 10.6 MB (10570971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df2396712ed6cf1ebf81db19d8e162b1c621c3fca9971be211747d7e10bf8`  
		Last Modified: Fri, 03 Sep 2021 02:51:58 GMT  
		Size: 52.3 MB (52319329 bytes)  
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
$ docker pull buildpack-deps@sha256:ad88db1472e0c705f72cf52470e55fd98ca5e14e00e67cfa4c1ae2491f4b42ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128380780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f54f21a8eb6c7073aabdfbc66893ce44b6e77dbf73034a40c13c913bd246f5b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853d83532467d1599448d38360ea9d52789d7d10f30c6734e17728c98743435b`  
		Last Modified: Fri, 03 Sep 2021 01:19:38 GMT  
		Size: 5.3 MB (5282881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6935e9ec29feb2101753d15eca8fa2727e2b060c07d2f720f471c55fb344c2a4`  
		Last Modified: Fri, 03 Sep 2021 01:19:39 GMT  
		Size: 11.3 MB (11250633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf6b2b625a6c874fcfb0e659f71235906f8459aa36ce32066b8efe1daf7c855`  
		Last Modified: Fri, 03 Sep 2021 01:20:07 GMT  
		Size: 55.9 MB (55916333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6f7f0eda304eea56cad106a2326a1c13b9795bf40b8cb034bf22216101812a76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122463445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472a6e379480171cbaf23c6d657f64a0656a5f76461f1ee4e7b779f4d3d2e2da`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:46:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918f43385735f5455e955ef94ef61f2089c0caebab840605cb52e5dd7525cd4`  
		Last Modified: Fri, 03 Sep 2021 01:59:04 GMT  
		Size: 53.3 MB (53297975 bytes)  
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
$ docker pull buildpack-deps@sha256:485ac24b4b3a8b7585b955839727007d6a2758907be6a957c535027848236e2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aa3622158c598757cde789c4df5c79291a8281dfa04b2a762e7e95f1e603db9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f48d5133e49359781fde1a8e72c81879ba30ffcb5b6d759f0ecb28fe6bbbe8`  
		Last Modified: Fri, 03 Sep 2021 02:19:40 GMT  
		Size: 5.1 MB (5137216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab672e8b32c6e3623bde683097d4c5fe5a73090dcb963e9f5512dfc21c485f58`  
		Last Modified: Fri, 03 Sep 2021 02:19:41 GMT  
		Size: 10.8 MB (10761458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7068e3642fc5ba5e489f8857ba725ba64ef0ce4b28acbf1545d133584bae2`  
		Last Modified: Fri, 03 Sep 2021 02:19:59 GMT  
		Size: 54.1 MB (54050487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:2cb37b188a530c3d81b8def93a5be2a1062bbcd5627bdd2e187c01dd9e71af18
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
$ docker pull buildpack-deps@sha256:e20d79afa0c9535fe3231377c6ee4df39fa7b7aae0bfaa47986c5b4f835d3ed9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286124730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8309dfe7b477df76d3a3edcb146b58d2f1222ab3881f9e3f1ff6474fdf42b695`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:55 GMT
ADD file:2edb17d6de848884fe9c4f448cf83c7eb38db986179ad828a28e287727206359 in / 
# Fri, 03 Sep 2021 00:50:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:35:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:35:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:39:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6cb7b6b06f67582053bf766e2dfc8cf86da6a819d6b0f89087b19d266364c4e`  
		Last Modified: Fri, 03 Sep 2021 01:06:27 GMT  
		Size: 48.2 MB (48153787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e990870d90c5fbe59daeaf6595ea5f84dfc9b19d83ceee42f1c77151b28c8`  
		Last Modified: Fri, 03 Sep 2021 02:54:23 GMT  
		Size: 7.4 MB (7376968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f97aee7b401dda2cdbd199f93baedfb4d6c1c77abcb61a736f63fc9818d541`  
		Last Modified: Fri, 03 Sep 2021 02:54:24 GMT  
		Size: 9.7 MB (9687490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df658833310cf636515e182b07f0f757747de5e7bf7cb2d5798c438dffe9a962`  
		Last Modified: Fri, 03 Sep 2021 02:55:13 GMT  
		Size: 49.6 MB (49574916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c5eacbd1943e12eba81a033914a38c27e596c6baab6126ef425dcec1b36a99`  
		Last Modified: Fri, 03 Sep 2021 02:57:09 GMT  
		Size: 171.3 MB (171331569 bytes)  
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
$ docker pull buildpack-deps@sha256:a9d2f53fb8f3c5d3342cfffc6c2a66a1ca03d58fa39476d86109e1caaf8985a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321916290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8c7bbcb5af6fee646d2097ff955284ad700486cf13df70b89023e993d37d7e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:07 GMT
ADD file:b57b08af647bb21d95dcfaaf631569421b159ccb57981aa968957e83d0d88be1 in / 
# Fri, 03 Sep 2021 00:40:07 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51869ffe8843ba6b44f606117326ad744bef79bc74f8eb46ebdc19e9299ede76`  
		Last Modified: Fri, 03 Sep 2021 00:48:31 GMT  
		Size: 51.2 MB (51207209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b7c65ab186ac667e4c325c9bc0aedb35fa5c3c0e94bcf31756f2242bad69c`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 8.0 MB (7999823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e5b243d4918f63b95623e21cd2da926e7a519a11f79d5dccbe9e1c921fdb3`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 10.3 MB (10339942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ad561c8654d0087f55d8ba8f2c88f6bf9760d1a07c98c20226182dd661df18`  
		Last Modified: Fri, 03 Sep 2021 01:21:49 GMT  
		Size: 53.4 MB (53438188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7076e49e31f46f892cc53ebc742d6b7aac932b484254aa2eebc010ca0de90549`  
		Last Modified: Fri, 03 Sep 2021 01:22:43 GMT  
		Size: 198.9 MB (198931128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d634063a8331fe4268a41b3671e01c2b40010cb1103b24ef8d58479399c4c2e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297107089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43fc77b654d792f05d7cbb25930e90bacd59e074b1fbc0bfdb319d8b890be9c9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:26 GMT
ADD file:b1e1d3ff824c87ebeca7b3a0ef30937ea44a74450c5e2b2d2ae40d557df10ca0 in / 
# Fri, 03 Sep 2021 01:10:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:49:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:50:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:52:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ba0bd93a428688eed3f712e236aed68cd618f1aa507a5f75a9041f2e9849710`  
		Last Modified: Fri, 03 Sep 2021 01:19:10 GMT  
		Size: 49.1 MB (49080081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbdd3e2a4240b488fa8b608a56ca7e673ac5ef915e2f613574e7216ba4bd4d`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 7.3 MB (7253475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39492d54de9c1aa951897ec16b4ed7089bac77f23415e8ba2a8afa6bdca35fcc`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08a1f31fe454064309426ca44c375688e97aae9e8881495a117da13b13d3406`  
		Last Modified: Fri, 03 Sep 2021 02:02:20 GMT  
		Size: 50.8 MB (50843995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02609cf933fae5e74db6107e0fc797cf5c673d66c6246d39e2867543a7c9e2bb`  
		Last Modified: Fri, 03 Sep 2021 02:04:28 GMT  
		Size: 179.9 MB (179913101 bytes)  
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
$ docker pull buildpack-deps@sha256:0dfdccd8f2e50a7fe191748419f24a6e62487c3033a08f6c45e4b7cdee793dc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294549065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75aca64b33ae679db5de7e6910db6d3a4551b9aa423452fdf55deb81d8635ecd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:12 GMT
ADD file:282d4f0b6aa732d36151d4d99869e435e6fa273ff73904ae6da0df618b7c2a3e in / 
# Fri, 03 Sep 2021 00:44:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:08:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:08:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:11:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:98373502f525a0ec193f60462454ed062dd42ded2a98cb5fab011b55ec824c77`  
		Last Modified: Fri, 03 Sep 2021 00:53:16 GMT  
		Size: 49.0 MB (49004112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcc170cd12eeca791be319fcc5b66571023e31a38e6dd0c2b630227e512460e`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 7.4 MB (7400980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab67ee15cd57c1d22855cdec415bdc1e7b43122552befb5143f4e3e061dd107`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 9.9 MB (9883239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492849c87aa7918355ea3ddd15023d5192779474cd1ad01937363046cd5ed777`  
		Last Modified: Fri, 03 Sep 2021 02:20:59 GMT  
		Size: 51.4 MB (51380450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f583bcb6e3e69399c59333e43ffaa7efcf40301ec6fec56dcecb4f1ee5b35be1`  
		Last Modified: Fri, 03 Sep 2021 02:21:28 GMT  
		Size: 176.9 MB (176880284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:0096028425fb87ab1f534c9ae686a9a6f25c66feb1fa2a176edc07b0fbc0c84c
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
$ docker pull buildpack-deps@sha256:654299e0118d6a69615e00c53b04d58fde3187ff53e7332965448d5a8b6cb7e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65218245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7958978b70ef9cc355af985d00871287d008c0a09cb758947b336312d38665c5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:55 GMT
ADD file:2edb17d6de848884fe9c4f448cf83c7eb38db986179ad828a28e287727206359 in / 
# Fri, 03 Sep 2021 00:50:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:35:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:35:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a6cb7b6b06f67582053bf766e2dfc8cf86da6a819d6b0f89087b19d266364c4e`  
		Last Modified: Fri, 03 Sep 2021 01:06:27 GMT  
		Size: 48.2 MB (48153787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e990870d90c5fbe59daeaf6595ea5f84dfc9b19d83ceee42f1c77151b28c8`  
		Last Modified: Fri, 03 Sep 2021 02:54:23 GMT  
		Size: 7.4 MB (7376968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f97aee7b401dda2cdbd199f93baedfb4d6c1c77abcb61a736f63fc9818d541`  
		Last Modified: Fri, 03 Sep 2021 02:54:24 GMT  
		Size: 9.7 MB (9687490 bytes)  
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
$ docker pull buildpack-deps@sha256:409bd0ff35f739218799caf530b96c8f0a81a073f110da04d0af46d02d94ca38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69546974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6ae4e01bc97eb70eacb03cab757785d3c6e6e409a2d6443876ee11c2be7384`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:07 GMT
ADD file:b57b08af647bb21d95dcfaaf631569421b159ccb57981aa968957e83d0d88be1 in / 
# Fri, 03 Sep 2021 00:40:07 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:51869ffe8843ba6b44f606117326ad744bef79bc74f8eb46ebdc19e9299ede76`  
		Last Modified: Fri, 03 Sep 2021 00:48:31 GMT  
		Size: 51.2 MB (51207209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b7c65ab186ac667e4c325c9bc0aedb35fa5c3c0e94bcf31756f2242bad69c`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 8.0 MB (7999823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e5b243d4918f63b95623e21cd2da926e7a519a11f79d5dccbe9e1c921fdb3`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 10.3 MB (10339942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2f28d7aade7f73d14ae1136cef4108958febc1311acc07fcc5fcc5a3078c265f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66349993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb0417ec2edc8a010da78cdc28304c5b85cddce016a1cbacbcdfdf4ac7a6462`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:26 GMT
ADD file:b1e1d3ff824c87ebeca7b3a0ef30937ea44a74450c5e2b2d2ae40d557df10ca0 in / 
# Fri, 03 Sep 2021 01:10:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:49:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6ba0bd93a428688eed3f712e236aed68cd618f1aa507a5f75a9041f2e9849710`  
		Last Modified: Fri, 03 Sep 2021 01:19:10 GMT  
		Size: 49.1 MB (49080081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbdd3e2a4240b488fa8b608a56ca7e673ac5ef915e2f613574e7216ba4bd4d`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 7.3 MB (7253475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39492d54de9c1aa951897ec16b4ed7089bac77f23415e8ba2a8afa6bdca35fcc`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 10.0 MB (10016437 bytes)  
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
$ docker pull buildpack-deps@sha256:833091c790c7673c548e2e68fc482448c15ac5fb2e6c0a88628b9e881f9e8e9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66288331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42deb34c0183bafb7ed29008b674d1aa82da25fcb658d14cb1d759811030ffff`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:12 GMT
ADD file:282d4f0b6aa732d36151d4d99869e435e6fa273ff73904ae6da0df618b7c2a3e in / 
# Fri, 03 Sep 2021 00:44:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:08:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:08:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:98373502f525a0ec193f60462454ed062dd42ded2a98cb5fab011b55ec824c77`  
		Last Modified: Fri, 03 Sep 2021 00:53:16 GMT  
		Size: 49.0 MB (49004112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcc170cd12eeca791be319fcc5b66571023e31a38e6dd0c2b630227e512460e`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 7.4 MB (7400980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab67ee15cd57c1d22855cdec415bdc1e7b43122552befb5143f4e3e061dd107`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 9.9 MB (9883239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:d4b3badbfa050224faf7fb987b034e2dc26578f552cb8fa691d61cfce4aef99b
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
$ docker pull buildpack-deps@sha256:d2eb0e782e068ad39cf40f1625eb353b831463e636f95693ae41fb05f691cdcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114793161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4876ab18741ccd6ccef6cd50c172e9fff1ef364bccb1d3e70b093053ea4dda0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:55 GMT
ADD file:2edb17d6de848884fe9c4f448cf83c7eb38db986179ad828a28e287727206359 in / 
# Fri, 03 Sep 2021 00:50:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:35:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:35:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6cb7b6b06f67582053bf766e2dfc8cf86da6a819d6b0f89087b19d266364c4e`  
		Last Modified: Fri, 03 Sep 2021 01:06:27 GMT  
		Size: 48.2 MB (48153787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e990870d90c5fbe59daeaf6595ea5f84dfc9b19d83ceee42f1c77151b28c8`  
		Last Modified: Fri, 03 Sep 2021 02:54:23 GMT  
		Size: 7.4 MB (7376968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f97aee7b401dda2cdbd199f93baedfb4d6c1c77abcb61a736f63fc9818d541`  
		Last Modified: Fri, 03 Sep 2021 02:54:24 GMT  
		Size: 9.7 MB (9687490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df658833310cf636515e182b07f0f757747de5e7bf7cb2d5798c438dffe9a962`  
		Last Modified: Fri, 03 Sep 2021 02:55:13 GMT  
		Size: 49.6 MB (49574916 bytes)  
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
$ docker pull buildpack-deps@sha256:4cbbd2739a0403a4bc5fb44d0c0547c78cb6b4b5725d748ea8aaec196c62bf51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122985162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:097bbb812919407eacd1ae1255f64f143c4e079f4ace3fa2d93973ef58a05977`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:07 GMT
ADD file:b57b08af647bb21d95dcfaaf631569421b159ccb57981aa968957e83d0d88be1 in / 
# Fri, 03 Sep 2021 00:40:07 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51869ffe8843ba6b44f606117326ad744bef79bc74f8eb46ebdc19e9299ede76`  
		Last Modified: Fri, 03 Sep 2021 00:48:31 GMT  
		Size: 51.2 MB (51207209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b7c65ab186ac667e4c325c9bc0aedb35fa5c3c0e94bcf31756f2242bad69c`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 8.0 MB (7999823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e5b243d4918f63b95623e21cd2da926e7a519a11f79d5dccbe9e1c921fdb3`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 10.3 MB (10339942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ad561c8654d0087f55d8ba8f2c88f6bf9760d1a07c98c20226182dd661df18`  
		Last Modified: Fri, 03 Sep 2021 01:21:49 GMT  
		Size: 53.4 MB (53438188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6ab856bb690e3f3d77b73c06897b06e791118de0900b70a0631d7650121f0011
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117193988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f098c7247d21412ac50e09a060a32e85b985ca806949eabd5b8c55abfe0d879`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:26 GMT
ADD file:b1e1d3ff824c87ebeca7b3a0ef30937ea44a74450c5e2b2d2ae40d557df10ca0 in / 
# Fri, 03 Sep 2021 01:10:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:49:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:50:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ba0bd93a428688eed3f712e236aed68cd618f1aa507a5f75a9041f2e9849710`  
		Last Modified: Fri, 03 Sep 2021 01:19:10 GMT  
		Size: 49.1 MB (49080081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbdd3e2a4240b488fa8b608a56ca7e673ac5ef915e2f613574e7216ba4bd4d`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 7.3 MB (7253475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39492d54de9c1aa951897ec16b4ed7089bac77f23415e8ba2a8afa6bdca35fcc`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08a1f31fe454064309426ca44c375688e97aae9e8881495a117da13b13d3406`  
		Last Modified: Fri, 03 Sep 2021 02:02:20 GMT  
		Size: 50.8 MB (50843995 bytes)  
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
$ docker pull buildpack-deps@sha256:df83420f47187698a53a1d1619e3c8e76c62a31683d662fab930ad0f56c4a474
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117668781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09411ac234644b4a157d54187b1c193b7de35f4649ab96a23bff0dc7a43fe190`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:12 GMT
ADD file:282d4f0b6aa732d36151d4d99869e435e6fa273ff73904ae6da0df618b7c2a3e in / 
# Fri, 03 Sep 2021 00:44:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:08:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:08:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:98373502f525a0ec193f60462454ed062dd42ded2a98cb5fab011b55ec824c77`  
		Last Modified: Fri, 03 Sep 2021 00:53:16 GMT  
		Size: 49.0 MB (49004112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcc170cd12eeca791be319fcc5b66571023e31a38e6dd0c2b630227e512460e`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 7.4 MB (7400980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab67ee15cd57c1d22855cdec415bdc1e7b43122552befb5143f4e3e061dd107`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 9.9 MB (9883239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492849c87aa7918355ea3ddd15023d5192779474cd1ad01937363046cd5ed777`  
		Last Modified: Fri, 03 Sep 2021 02:20:59 GMT  
		Size: 51.4 MB (51380450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:ae9619a5c3c818d5149c0130318f141746acf3f6a1a24b58383ff902654a83e8
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
$ docker pull buildpack-deps@sha256:c1bf509fa76457be540f8f2fb10d9d26aa4890c9a4346c713745b6206fdda4be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68096113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73cdc4ca1ff77a007de35ea79cc9c08626250d2979cb0558df1bac7e1abd8c70`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:31:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f9763e0efd7dcf980819e39cb728c9f11f3c3f7dd944e21177efba57f6fe3`  
		Last Modified: Fri, 03 Sep 2021 02:51:03 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95efca74ef694ced85d684e7faecd407beb97667568054d98e5e09166a32d88a`  
		Last Modified: Fri, 03 Sep 2021 02:51:05 GMT  
		Size: 10.6 MB (10570971 bytes)  
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
$ docker pull buildpack-deps@sha256:ca1f95f69b1217eedf8fd5df25b029787d2b20be1c3808d4b56a7809cfafb72e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72464447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5250d94db9c58649245be60756b66f56ad4035644a1d6f28e3abd1e9e21ec49a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853d83532467d1599448d38360ea9d52789d7d10f30c6734e17728c98743435b`  
		Last Modified: Fri, 03 Sep 2021 01:19:38 GMT  
		Size: 5.3 MB (5282881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6935e9ec29feb2101753d15eca8fa2727e2b060c07d2f720f471c55fb344c2a4`  
		Last Modified: Fri, 03 Sep 2021 01:19:39 GMT  
		Size: 11.3 MB (11250633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1a5a8c8829bff1d7a89f8d97006a6ea359c46bb260fe809df4e907b5afd30a91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69165470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e5a9049a5620e106a070b8340f0b607aa86268008ceffc8ca4c29af118cfa3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
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
$ docker pull buildpack-deps@sha256:28124d888ebc509c072830169a01df6f23dcbbc8d88409f6aa3510b89267f1e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69099828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4861250614c542c631365e5d324fc1d562da14639c4308cea90abf09db002747`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f48d5133e49359781fde1a8e72c81879ba30ffcb5b6d759f0ecb28fe6bbbe8`  
		Last Modified: Fri, 03 Sep 2021 02:19:40 GMT  
		Size: 5.1 MB (5137216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab672e8b32c6e3623bde683097d4c5fe5a73090dcb963e9f5512dfc21c485f58`  
		Last Modified: Fri, 03 Sep 2021 02:19:41 GMT  
		Size: 10.8 MB (10761458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:f942c52d1fb8b6331953961709f7ea58df2457ca017d579d607702dae21e12da
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
$ docker pull buildpack-deps@sha256:683c8077722d969d03b468003dfe5a8781396fdbf2da8cc7ed293fd146bb6c31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241806439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f84f61f7cf291360eaf1ca0bf7b39a73b8ed8a565b3ced1f9f61a7164e75761`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:53:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:53:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:57:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1af8c8529138158c1ab9fc21b416a8348bcd120814c9105e5671a61366f1a4`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 7.8 MB (7771403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0df72f91f5e22bfe2c01836dcbb5cded6ba8b11975958672f924786ad44d121`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 3.6 MB (3624569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de940d7df01050bdb7ed77215e5c4ab341f72f7375f15a4463755ab286bc27f3`  
		Last Modified: Tue, 31 Aug 2021 03:13:09 GMT  
		Size: 60.7 MB (60718404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97a35b3662c00e3df90d0a430c5f8e1b47d098f26bf2809569c0453e71bd23f`  
		Last Modified: Tue, 31 Aug 2021 03:13:39 GMT  
		Size: 141.1 MB (141121989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4718fac5e814608335c977561e58a57e08fe828af6a27fe6518b24b9d246902d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207235901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1416b3f4cb8bc1878564692611dd119f31bba74d8498e5baf113b7f3cd7bb879`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:14:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:16:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:17:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c22e0906b4cd7dbb582181e7accbb483c55c760bfd4b2b06e28360279752f8`  
		Last Modified: Tue, 31 Aug 2021 03:35:41 GMT  
		Size: 6.8 MB (6768939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32fb178417438073a96fd01d75df3f32b76e8f1fb7b8dda7e693977a8025b43`  
		Last Modified: Tue, 31 Aug 2021 03:35:38 GMT  
		Size: 3.1 MB (3103787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0210be10f1605c0377e7fff7c8b6f3da7e7c69e756087b20718b4627035213`  
		Last Modified: Tue, 31 Aug 2021 03:36:34 GMT  
		Size: 55.5 MB (55453740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7b29c11815c04ded1d01feff6045c2405b932d7c2efc8af609bbabb13cb243`  
		Last Modified: Tue, 31 Aug 2021 03:37:59 GMT  
		Size: 117.8 MB (117840612 bytes)  
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
$ docker pull buildpack-deps@sha256:e519b10a76931d3242c67d57a628aec5f4e87b4595e1857d3bef0b2f6682058f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.4 MB (265375561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce85cc33f0ebc0dc5502c39e00c609993e0a5c7c28f4b5208f4acd693fee7155`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:40:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:43:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:55:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea9c7aedd6fb1a65cbeb9dbdebba7c78d501eb289eb92d2a11549fdbcac73f`  
		Last Modified: Tue, 31 Aug 2021 05:12:25 GMT  
		Size: 8.7 MB (8725966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4311ec6f0315cc94b2915046b0ea2dd892eece9196a601d82612067c158282`  
		Last Modified: Tue, 31 Aug 2021 05:11:56 GMT  
		Size: 4.5 MB (4456534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feb34377851231e9abee7d1f2f04aab8d35c219fec2687aac4046aae381b19e`  
		Last Modified: Tue, 31 Aug 2021 05:14:33 GMT  
		Size: 69.4 MB (69386748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bbc4692c5fde1d728b1a0b30b861560fcca966924a9939ac9a8a627c4a9522`  
		Last Modified: Tue, 31 Aug 2021 05:18:33 GMT  
		Size: 149.5 MB (149514522 bytes)  
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
$ docker pull buildpack-deps@sha256:0624329af768cbcdc97bb86460cf0d6a5559748c30f8643a9a23d9eb467f9193
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
$ docker pull buildpack-deps@sha256:750e084148cedb701692437bd5ac7648c8a8c151ef3bdd38a7a24fab10c9547b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39966046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fcbf592558a0b39f289c7a26daf7ce442d24b683b93abaee3ce35581337184`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:53:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1af8c8529138158c1ab9fc21b416a8348bcd120814c9105e5671a61366f1a4`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 7.8 MB (7771403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0df72f91f5e22bfe2c01836dcbb5cded6ba8b11975958672f924786ad44d121`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 3.6 MB (3624569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:55fa535446a8e6e8f4d38aabec939003121aa37e1ffec727dc230a00bc1223d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33941549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ed5867781a9efbdb982b87ebdc9d4b7e122304480acbb12b2366cb9a262b7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:14:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c22e0906b4cd7dbb582181e7accbb483c55c760bfd4b2b06e28360279752f8`  
		Last Modified: Tue, 31 Aug 2021 03:35:41 GMT  
		Size: 6.8 MB (6768939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32fb178417438073a96fd01d75df3f32b76e8f1fb7b8dda7e693977a8025b43`  
		Last Modified: Tue, 31 Aug 2021 03:35:38 GMT  
		Size: 3.1 MB (3103787 bytes)  
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
$ docker pull buildpack-deps@sha256:6906d9d9368197b792f3ae55b4002a9bb48c9dc4ff2005828e973956a2d60bea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46474291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0835e68757385fd7dcef70a25271212c73cea8cfb97a3c2be41c9358be6fb56`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:40:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea9c7aedd6fb1a65cbeb9dbdebba7c78d501eb289eb92d2a11549fdbcac73f`  
		Last Modified: Tue, 31 Aug 2021 05:12:25 GMT  
		Size: 8.7 MB (8725966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4311ec6f0315cc94b2915046b0ea2dd892eece9196a601d82612067c158282`  
		Last Modified: Tue, 31 Aug 2021 05:11:56 GMT  
		Size: 4.5 MB (4456534 bytes)  
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
$ docker pull buildpack-deps@sha256:533652c5d770a1d2054633fd5befb427a5e3083313f1e8fa3637b5127a79c5ee
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
$ docker pull buildpack-deps@sha256:8b8b97d300d1bc88549237ed88c7cdf64686a1328ee3a4ab78fbdd1ef5f8da2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100684450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c974b9e6e210580e3ae60d84424224f343c342c509e2c10ad8648f3bd6123cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:53:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:53:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1af8c8529138158c1ab9fc21b416a8348bcd120814c9105e5671a61366f1a4`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 7.8 MB (7771403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0df72f91f5e22bfe2c01836dcbb5cded6ba8b11975958672f924786ad44d121`  
		Last Modified: Tue, 31 Aug 2021 03:12:49 GMT  
		Size: 3.6 MB (3624569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de940d7df01050bdb7ed77215e5c4ab341f72f7375f15a4463755ab286bc27f3`  
		Last Modified: Tue, 31 Aug 2021 03:13:09 GMT  
		Size: 60.7 MB (60718404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fc96eae5b17a1509ebd86aec2fc4f5ab815303f932dee306ef7d372ef9d27f73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89395289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2592dcde1e1046cc64d12828ff8273c7be8298f1cd34cdb716f3b31771c3187a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:14:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:16:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c22e0906b4cd7dbb582181e7accbb483c55c760bfd4b2b06e28360279752f8`  
		Last Modified: Tue, 31 Aug 2021 03:35:41 GMT  
		Size: 6.8 MB (6768939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32fb178417438073a96fd01d75df3f32b76e8f1fb7b8dda7e693977a8025b43`  
		Last Modified: Tue, 31 Aug 2021 03:35:38 GMT  
		Size: 3.1 MB (3103787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0210be10f1605c0377e7fff7c8b6f3da7e7c69e756087b20718b4627035213`  
		Last Modified: Tue, 31 Aug 2021 03:36:34 GMT  
		Size: 55.5 MB (55453740 bytes)  
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
$ docker pull buildpack-deps@sha256:c004774b38314517688fc6d7d94f8e6f42c0a8d1039132f47cc28362ddbcf89a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115861039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d7512b0ae7b5e20b692c2aaddd3902fccd66cca69da3d103fe14b95a702faf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:40:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:43:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea9c7aedd6fb1a65cbeb9dbdebba7c78d501eb289eb92d2a11549fdbcac73f`  
		Last Modified: Tue, 31 Aug 2021 05:12:25 GMT  
		Size: 8.7 MB (8725966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4311ec6f0315cc94b2915046b0ea2dd892eece9196a601d82612067c158282`  
		Last Modified: Tue, 31 Aug 2021 05:11:56 GMT  
		Size: 4.5 MB (4456534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feb34377851231e9abee7d1f2f04aab8d35c219fec2687aac4046aae381b19e`  
		Last Modified: Tue, 31 Aug 2021 05:14:33 GMT  
		Size: 69.4 MB (69386748 bytes)  
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
$ docker pull buildpack-deps@sha256:a973b51dffd6768a5c4055c422ec5d667320c9c3c6ee66adb6e0183b42f95bbc
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
$ docker pull buildpack-deps@sha256:ee876b5182702366abacc4e22f28a86fe10dc38d7dd7cb878fe3aa5c2ff2f592
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248811826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afd0b8377ef4379047117c097d974a1716e0a336ccfa034f68ec346f778e5708`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:03 GMT
ADD file:4ac73e113682ef48b7466c4f8765ca7fd54ae98228caa319438a76c35d762b1b in / 
# Tue, 31 Aug 2021 01:21:04 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:57:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:58:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:58:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:02:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7e10407b4d96b1866d5b77b368ac8b2b9b3ef9b210bad0b4784407405121b92`  
		Last Modified: Tue, 31 Aug 2021 01:22:35 GMT  
		Size: 31.7 MB (31703609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2bdc17338d4753c86d8e5520aadb12207bd763dac1f00aa8eb9042fcd88034`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 5.4 MB (5430701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03dd940109a3cc748ce9b671747e7089353d649088e88252f777dcf586a8963`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 3.7 MB (3662065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa3b3922cd293eb3f32aea33d2e5e755a7eae3fce018122e98ef65dd1094a4c`  
		Last Modified: Tue, 31 Aug 2021 03:14:08 GMT  
		Size: 43.5 MB (43541507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c749bf16aecacb19367e45ff9160888d2640ef0ef96d4540fda2a73cad278d`  
		Last Modified: Tue, 31 Aug 2021 03:14:41 GMT  
		Size: 164.5 MB (164473944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1ff7ba11a2f63f4d14d3f50ddd146ecde5b0508600eb4c590f95c80b587bde58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208947575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a963770795b9d8c43ab41d4b55f510efe9f03b2f8352127cbff2d225907b67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:17 GMT
ADD file:cd7671d88520bafabf9a3bea20bd80ee0d2881b895c7f5ce1aaa4958e396074f in / 
# Tue, 31 Aug 2021 01:41:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:18:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:18:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:19:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:21:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:48989deb32eb328d42c26dae334c8da758b723afff40db2647f6780446ec97e8`  
		Last Modified: Tue, 31 Aug 2021 01:45:34 GMT  
		Size: 26.9 MB (26860548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fec9a0a8408a0d36cfa8cb75d2b9e32ea29b69e96c4038df08fc8f06ef52d8b`  
		Last Modified: Tue, 31 Aug 2021 03:38:16 GMT  
		Size: 4.9 MB (4859278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e811318e550593783ac5850dd96d8ac3a3fe682126dabd9493f201cc9f9d0c78`  
		Last Modified: Tue, 31 Aug 2021 03:38:14 GMT  
		Size: 3.1 MB (3138679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36aaae4759daf4d1e91747ae90020318048e7da07cf05181f7ab2f9999eb3ff6`  
		Last Modified: Tue, 31 Aug 2021 03:38:56 GMT  
		Size: 40.0 MB (39953103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe95157c0c6b5402391e23ed75940081585914a4733e580e0d9ba6f2d81fbf2`  
		Last Modified: Tue, 31 Aug 2021 03:40:29 GMT  
		Size: 134.1 MB (134135967 bytes)  
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
$ docker pull buildpack-deps@sha256:058e78da9e2ac970d7448e82c797d473413620255fff6c64cdf88de5f10830a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.1 MB (268065940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb635bb0a138e9db48877563d235b9e64ecbca3ba1667396421a48c2c52b2fa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:57:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:19:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615e5e41d59fe32c6e6c5284994935d713f08ed29bdc3f9841683f0793cf8394`  
		Last Modified: Tue, 31 Aug 2021 05:20:33 GMT  
		Size: 6.2 MB (6155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99aa8209221f270d9ffc050088f6998d6ceefa228f2ca68f9eb5bc410b24fadc`  
		Last Modified: Tue, 31 Aug 2021 05:19:57 GMT  
		Size: 4.5 MB (4523763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e43d357f3322abb3a717de7eaf87420b14cbcae1a2c006e9267578aa7c7881`  
		Last Modified: Tue, 31 Aug 2021 05:22:13 GMT  
		Size: 49.5 MB (49467214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c991a658b76da93bd82aa1b744de18c388c34d14ed61e2ec281aed8ac7bd7b9e`  
		Last Modified: Tue, 31 Aug 2021 05:27:03 GMT  
		Size: 170.7 MB (170733574 bytes)  
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
$ docker pull buildpack-deps@sha256:ff1b1d9dc00dadeca39b39907fcd12af254500e39e8c65acf9ea9c60ecfbdf7b
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
$ docker pull buildpack-deps@sha256:38c9947bebf08bf338214a9539d13131ceceef2eb56a3a962fd487d03a4a48ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd9b43ff77c32f2171be9117ae172526d0bbc561da8f7525f999efc126f5eb09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:03 GMT
ADD file:4ac73e113682ef48b7466c4f8765ca7fd54ae98228caa319438a76c35d762b1b in / 
# Tue, 31 Aug 2021 01:21:04 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:57:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:58:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d7e10407b4d96b1866d5b77b368ac8b2b9b3ef9b210bad0b4784407405121b92`  
		Last Modified: Tue, 31 Aug 2021 01:22:35 GMT  
		Size: 31.7 MB (31703609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2bdc17338d4753c86d8e5520aadb12207bd763dac1f00aa8eb9042fcd88034`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 5.4 MB (5430701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03dd940109a3cc748ce9b671747e7089353d649088e88252f777dcf586a8963`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 3.7 MB (3662065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d61014dc4d388d078b9c36260a7cc23617d103342e7e04975cedb5f704468fda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34858505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c935c4d2289718675e23151e3e67200070942fbce6e4b507ddff7a679fbdec1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:17 GMT
ADD file:cd7671d88520bafabf9a3bea20bd80ee0d2881b895c7f5ce1aaa4958e396074f in / 
# Tue, 31 Aug 2021 01:41:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:18:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:18:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:48989deb32eb328d42c26dae334c8da758b723afff40db2647f6780446ec97e8`  
		Last Modified: Tue, 31 Aug 2021 01:45:34 GMT  
		Size: 26.9 MB (26860548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fec9a0a8408a0d36cfa8cb75d2b9e32ea29b69e96c4038df08fc8f06ef52d8b`  
		Last Modified: Tue, 31 Aug 2021 03:38:16 GMT  
		Size: 4.9 MB (4859278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e811318e550593783ac5850dd96d8ac3a3fe682126dabd9493f201cc9f9d0c78`  
		Last Modified: Tue, 31 Aug 2021 03:38:14 GMT  
		Size: 3.1 MB (3138679 bytes)  
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
$ docker pull buildpack-deps@sha256:b93bc595a55dddf7b45d8d5ac826b9ff698374ac6f9058ef103104b9f0f85926
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47865152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd812682377fde30cb7af2ebe1f69410167761e73b69535b5e0a2cd6e9411295`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:57:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615e5e41d59fe32c6e6c5284994935d713f08ed29bdc3f9841683f0793cf8394`  
		Last Modified: Tue, 31 Aug 2021 05:20:33 GMT  
		Size: 6.2 MB (6155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99aa8209221f270d9ffc050088f6998d6ceefa228f2ca68f9eb5bc410b24fadc`  
		Last Modified: Tue, 31 Aug 2021 05:19:57 GMT  
		Size: 4.5 MB (4523763 bytes)  
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
$ docker pull buildpack-deps@sha256:0e63d7d04671f447f35c721d0cc0329e2e6bbf0421f4b74e8e0ed0f9c7abcc7e
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
$ docker pull buildpack-deps@sha256:53963b8dedc84f611319c16f86c364bb1ade2088bd39dcffef7bc047e2606111
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.3 MB (84337882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:070fc06a5156d80575b1bd08707831468912b0a8af4a60a8ddbbac20d0f8acde`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:03 GMT
ADD file:4ac73e113682ef48b7466c4f8765ca7fd54ae98228caa319438a76c35d762b1b in / 
# Tue, 31 Aug 2021 01:21:04 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:57:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:58:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:58:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7e10407b4d96b1866d5b77b368ac8b2b9b3ef9b210bad0b4784407405121b92`  
		Last Modified: Tue, 31 Aug 2021 01:22:35 GMT  
		Size: 31.7 MB (31703609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2bdc17338d4753c86d8e5520aadb12207bd763dac1f00aa8eb9042fcd88034`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 5.4 MB (5430701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03dd940109a3cc748ce9b671747e7089353d649088e88252f777dcf586a8963`  
		Last Modified: Tue, 31 Aug 2021 03:13:50 GMT  
		Size: 3.7 MB (3662065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa3b3922cd293eb3f32aea33d2e5e755a7eae3fce018122e98ef65dd1094a4c`  
		Last Modified: Tue, 31 Aug 2021 03:14:08 GMT  
		Size: 43.5 MB (43541507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2e03a791f00acdebdb202ef33d78e6946ecbbabb9b3e2a6b6c42d561a9504308
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74811608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fa7a2751d29365ef5f45ca3f55897eea12bb3795441d0f5ccba9ce32318a043`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:17 GMT
ADD file:cd7671d88520bafabf9a3bea20bd80ee0d2881b895c7f5ce1aaa4958e396074f in / 
# Tue, 31 Aug 2021 01:41:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:18:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:18:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:19:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:48989deb32eb328d42c26dae334c8da758b723afff40db2647f6780446ec97e8`  
		Last Modified: Tue, 31 Aug 2021 01:45:34 GMT  
		Size: 26.9 MB (26860548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fec9a0a8408a0d36cfa8cb75d2b9e32ea29b69e96c4038df08fc8f06ef52d8b`  
		Last Modified: Tue, 31 Aug 2021 03:38:16 GMT  
		Size: 4.9 MB (4859278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e811318e550593783ac5850dd96d8ac3a3fe682126dabd9493f201cc9f9d0c78`  
		Last Modified: Tue, 31 Aug 2021 03:38:14 GMT  
		Size: 3.1 MB (3138679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36aaae4759daf4d1e91747ae90020318048e7da07cf05181f7ab2f9999eb3ff6`  
		Last Modified: Tue, 31 Aug 2021 03:38:56 GMT  
		Size: 40.0 MB (39953103 bytes)  
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
$ docker pull buildpack-deps@sha256:08c18882a70aad8af2599f0170a98f8c20db30a91fcc5a77d3b043e5bfc7614c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.3 MB (97332366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5211c4bfed288ada093bfbb9e2f58c5f291103d5c360755d5ac8be047e188f50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:57:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615e5e41d59fe32c6e6c5284994935d713f08ed29bdc3f9841683f0793cf8394`  
		Last Modified: Tue, 31 Aug 2021 05:20:33 GMT  
		Size: 6.2 MB (6155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99aa8209221f270d9ffc050088f6998d6ceefa228f2ca68f9eb5bc410b24fadc`  
		Last Modified: Tue, 31 Aug 2021 05:19:57 GMT  
		Size: 4.5 MB (4523763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e43d357f3322abb3a717de7eaf87420b14cbcae1a2c006e9267578aa7c7881`  
		Last Modified: Tue, 31 Aug 2021 05:22:13 GMT  
		Size: 49.5 MB (49467214 bytes)  
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
$ docker pull buildpack-deps@sha256:b6112899295bc4ee493ef3e21ee6ef732d267ed29af52121df1810f1838d1093
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
$ docker pull buildpack-deps@sha256:9af39729d3d63f5797c785605e9c26effbfb09444ef91f5bd0099e5827edd880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.9 MB (406868171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa7f2e7a9355bb02a5478b27f15892dda84f9277790d6bf142f99d5982080d53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:12 GMT
ADD file:355a5f56bf0136597bcd90b01ff73fc517b6bf7e76f45b65bf1af1136f434462 in / 
# Tue, 31 Aug 2021 01:21:12 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:03:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:05:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25907b3add375d4f44a3bf4bfc3544b51ff9f4a23fe8c186f3b20e54b37d19ae`  
		Last Modified: Tue, 31 Aug 2021 01:22:53 GMT  
		Size: 30.6 MB (30602781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ef40c83a42d65ce37ce8bc08e06a0c4b994512527cad13196aca51586d9bd7`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.7 MB (3692694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871edcbb988433606f5a8d03efc8f0d9d49a4cd78a5d506401ec3b7854a2162`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.6 MB (3552016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59778cb761facf0aaa7ff7cab370d47bdee8a1c0764186ec8286f50fb911a78b`  
		Last Modified: Tue, 31 Aug 2021 03:15:08 GMT  
		Size: 38.1 MB (38114895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffa26f12ed647c5e1c9898915298f9e7389c733e2825bad35dac65a6b529755`  
		Last Modified: Tue, 31 Aug 2021 03:16:00 GMT  
		Size: 330.9 MB (330905785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b4cd810e63cec40720081b46d9f7d51f6879f979f24a21782c183d6cdf2533d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.3 MB (371327940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea1b0d70c3fe313e6e52e4f870b7ec6ddf510caa3a0accad930efba05e6b01b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:42 GMT
ADD file:0abcd0c1c6aecb3d5af2aa5d9c631949d716076e338faccdd7802906b4979bd6 in / 
# Tue, 31 Aug 2021 01:41:43 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:21:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:22:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:22:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:24:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be5e7fb59932c05a5acf0221847ae12179d4f81037fdeb44f8c408bc27ec1511`  
		Last Modified: Tue, 31 Aug 2021 01:46:11 GMT  
		Size: 27.3 MB (27313903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c8f5e7395b48e26211a363f2c66ea0e729fa5f4ce1e980a22a70c47eacbf1`  
		Last Modified: Tue, 31 Aug 2021 03:40:47 GMT  
		Size: 3.4 MB (3438915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30125ee4f15b1f56a8279e5c1f488ef77c51231b62f4da3cb1a03b8a32fdae7`  
		Last Modified: Tue, 31 Aug 2021 03:40:46 GMT  
		Size: 3.7 MB (3742231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01de5d75b44b35b6f46117f4d1484f24b516edeed132dc1815d6a78fb0cbbd6`  
		Last Modified: Tue, 31 Aug 2021 03:41:28 GMT  
		Size: 40.3 MB (40317890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061c3e4e41e25d781afd762c7e0519095f1075b1d9504f209328e2b477700b75`  
		Last Modified: Tue, 31 Aug 2021 03:44:30 GMT  
		Size: 296.5 MB (296515001 bytes)  
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
$ docker pull buildpack-deps@sha256:2be72be9ca82b6475c433d3069b67ee4c9d76f0bf162b5d92392859509e87877
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413058139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef497b78fbb6c17ea0698512be7ab72912b9c4103be39f07db90a3ade98dd07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:28 GMT
ADD file:776487dfd6a31c5a5d57d6924dd11136cb94d2e661eb085c76b14213c2220e3f in / 
# Tue, 31 Aug 2021 02:11:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:21:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:23:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:42:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f23233eca55841e558566a0a689d1261b17a023a5d0ed1e0ee267da33ff84a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:11 GMT  
		Size: 36.1 MB (36055099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10a1f2d8a9c3bf4f6060f088986f3f74fbf50acda4d6016dfd6d1115fbf3a9d`  
		Last Modified: Tue, 31 Aug 2021 05:27:38 GMT  
		Size: 4.1 MB (4096829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26809db5804495bc5bf81be1fbeae7b7a82215d30ff3e0c59d3353cc857206`  
		Last Modified: Tue, 31 Aug 2021 05:27:21 GMT  
		Size: 4.2 MB (4241626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671fe0a2b7c06f1e3c899f5ad9e8b89dbbef68ba1f5bc446f05beaeca064dd31`  
		Last Modified: Tue, 31 Aug 2021 05:29:18 GMT  
		Size: 42.6 MB (42605912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9257fa229b5f286c331fe7b926deef3aee7709c3b87ae22f5cd31d4efc1765`  
		Last Modified: Tue, 31 Aug 2021 05:33:16 GMT  
		Size: 326.1 MB (326058673 bytes)  
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
$ docker pull buildpack-deps@sha256:40969d345ea67b862a72d9d24144395ddea299a517a4c456f060cf108f177c84
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
$ docker pull buildpack-deps@sha256:dd6c280b99daea86543d074f477b5b196e3136433686b6848dc654663bb60e58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37847491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883360346d84b6140d17a89c82dded9c76d0c86eda04909badf532a6d40fcfd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:12 GMT
ADD file:355a5f56bf0136597bcd90b01ff73fc517b6bf7e76f45b65bf1af1136f434462 in / 
# Tue, 31 Aug 2021 01:21:12 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:03:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:25907b3add375d4f44a3bf4bfc3544b51ff9f4a23fe8c186f3b20e54b37d19ae`  
		Last Modified: Tue, 31 Aug 2021 01:22:53 GMT  
		Size: 30.6 MB (30602781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ef40c83a42d65ce37ce8bc08e06a0c4b994512527cad13196aca51586d9bd7`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.7 MB (3692694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871edcbb988433606f5a8d03efc8f0d9d49a4cd78a5d506401ec3b7854a2162`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.6 MB (3552016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9a3d5880ea36b8866fa5d8f9d4b3604048c83a329f3e4a4ea6aba5eed872f1fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34495049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e2e9a9304e887c58fb5516661169e2e18ea005307279c2d8d325a22f638621`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:42 GMT
ADD file:0abcd0c1c6aecb3d5af2aa5d9c631949d716076e338faccdd7802906b4979bd6 in / 
# Tue, 31 Aug 2021 01:41:43 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:21:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:22:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be5e7fb59932c05a5acf0221847ae12179d4f81037fdeb44f8c408bc27ec1511`  
		Last Modified: Tue, 31 Aug 2021 01:46:11 GMT  
		Size: 27.3 MB (27313903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c8f5e7395b48e26211a363f2c66ea0e729fa5f4ce1e980a22a70c47eacbf1`  
		Last Modified: Tue, 31 Aug 2021 03:40:47 GMT  
		Size: 3.4 MB (3438915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30125ee4f15b1f56a8279e5c1f488ef77c51231b62f4da3cb1a03b8a32fdae7`  
		Last Modified: Tue, 31 Aug 2021 03:40:46 GMT  
		Size: 3.7 MB (3742231 bytes)  
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
$ docker pull buildpack-deps@sha256:838cee7286d3baa3d78a9117036d5697643c8db2337680cedb6d584405b7ba53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44393554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c7088c04b44397a9f243f59f8046529d76d35591ab07d0f3564045047c59cd2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:28 GMT
ADD file:776487dfd6a31c5a5d57d6924dd11136cb94d2e661eb085c76b14213c2220e3f in / 
# Tue, 31 Aug 2021 02:11:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:21:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7f23233eca55841e558566a0a689d1261b17a023a5d0ed1e0ee267da33ff84a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:11 GMT  
		Size: 36.1 MB (36055099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10a1f2d8a9c3bf4f6060f088986f3f74fbf50acda4d6016dfd6d1115fbf3a9d`  
		Last Modified: Tue, 31 Aug 2021 05:27:38 GMT  
		Size: 4.1 MB (4096829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26809db5804495bc5bf81be1fbeae7b7a82215d30ff3e0c59d3353cc857206`  
		Last Modified: Tue, 31 Aug 2021 05:27:21 GMT  
		Size: 4.2 MB (4241626 bytes)  
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
$ docker pull buildpack-deps@sha256:f5326c47df09b079464b892d20fd05a3aadbc1575839f1804e8fedc6aba2e4ab
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
$ docker pull buildpack-deps@sha256:f68d3b481c199cba164a796afe4f6c460293fe1810d2bd5fc323bedca9db34e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75962386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edb492d2fe194b03eeee021b94668fa6d5019b08c3d8a268a8145465c35158d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:12 GMT
ADD file:355a5f56bf0136597bcd90b01ff73fc517b6bf7e76f45b65bf1af1136f434462 in / 
# Tue, 31 Aug 2021 01:21:12 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:03:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25907b3add375d4f44a3bf4bfc3544b51ff9f4a23fe8c186f3b20e54b37d19ae`  
		Last Modified: Tue, 31 Aug 2021 01:22:53 GMT  
		Size: 30.6 MB (30602781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ef40c83a42d65ce37ce8bc08e06a0c4b994512527cad13196aca51586d9bd7`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.7 MB (3692694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871edcbb988433606f5a8d03efc8f0d9d49a4cd78a5d506401ec3b7854a2162`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.6 MB (3552016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59778cb761facf0aaa7ff7cab370d47bdee8a1c0764186ec8286f50fb911a78b`  
		Last Modified: Tue, 31 Aug 2021 03:15:08 GMT  
		Size: 38.1 MB (38114895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eb7e85f3681ff91b3c2ad5df257554ba0bed79851ceb90c2bdd39bd717ebdee1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74812939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a076702ca7e06d53c2bf037f5a9e46dd84724a6de0ee98774d147661533654`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:42 GMT
ADD file:0abcd0c1c6aecb3d5af2aa5d9c631949d716076e338faccdd7802906b4979bd6 in / 
# Tue, 31 Aug 2021 01:41:43 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:21:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:22:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:22:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be5e7fb59932c05a5acf0221847ae12179d4f81037fdeb44f8c408bc27ec1511`  
		Last Modified: Tue, 31 Aug 2021 01:46:11 GMT  
		Size: 27.3 MB (27313903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c8f5e7395b48e26211a363f2c66ea0e729fa5f4ce1e980a22a70c47eacbf1`  
		Last Modified: Tue, 31 Aug 2021 03:40:47 GMT  
		Size: 3.4 MB (3438915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30125ee4f15b1f56a8279e5c1f488ef77c51231b62f4da3cb1a03b8a32fdae7`  
		Last Modified: Tue, 31 Aug 2021 03:40:46 GMT  
		Size: 3.7 MB (3742231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01de5d75b44b35b6f46117f4d1484f24b516edeed132dc1815d6a78fb0cbbd6`  
		Last Modified: Tue, 31 Aug 2021 03:41:28 GMT  
		Size: 40.3 MB (40317890 bytes)  
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
$ docker pull buildpack-deps@sha256:5842de42899adb406caffa3d495ad51cfc06dd3bf5ec1eb8022df11e29c74efd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86999466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ff5b2bb66e5ad11a8cdfc7a5f24440425e23f96b465dd30a510fe40c40ee67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:28 GMT
ADD file:776487dfd6a31c5a5d57d6924dd11136cb94d2e661eb085c76b14213c2220e3f in / 
# Tue, 31 Aug 2021 02:11:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:21:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:23:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f23233eca55841e558566a0a689d1261b17a023a5d0ed1e0ee267da33ff84a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:11 GMT  
		Size: 36.1 MB (36055099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10a1f2d8a9c3bf4f6060f088986f3f74fbf50acda4d6016dfd6d1115fbf3a9d`  
		Last Modified: Tue, 31 Aug 2021 05:27:38 GMT  
		Size: 4.1 MB (4096829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26809db5804495bc5bf81be1fbeae7b7a82215d30ff3e0c59d3353cc857206`  
		Last Modified: Tue, 31 Aug 2021 05:27:21 GMT  
		Size: 4.2 MB (4241626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671fe0a2b7c06f1e3c899f5ad9e8b89dbbef68ba1f5bc446f05beaeca064dd31`  
		Last Modified: Tue, 31 Aug 2021 05:29:18 GMT  
		Size: 42.6 MB (42605912 bytes)  
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
$ docker pull buildpack-deps@sha256:f6c911ff12af5e812a96df5b24fc67cc7d2924c07d13d52f9d3ee90fc9f8b81c
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
$ docker pull buildpack-deps@sha256:9b65dde79ee2e03922f844db61fb0dd2e97297df7ab620ead878c347744f430c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295058728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6bab944fcaa224ed17b83c9812ae6117a5f28d269b0b0477135bb05e601420e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:31:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:32:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:34:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f9763e0efd7dcf980819e39cb728c9f11f3c3f7dd944e21177efba57f6fe3`  
		Last Modified: Fri, 03 Sep 2021 02:51:03 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95efca74ef694ced85d684e7faecd407beb97667568054d98e5e09166a32d88a`  
		Last Modified: Fri, 03 Sep 2021 02:51:05 GMT  
		Size: 10.6 MB (10570971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df2396712ed6cf1ebf81db19d8e162b1c621c3fca9971be211747d7e10bf8`  
		Last Modified: Fri, 03 Sep 2021 02:51:58 GMT  
		Size: 52.3 MB (52319329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0847f5ab2d0f284ff33db1f85872a599e314abb845aaab72c0e9a3e57a063c96`  
		Last Modified: Fri, 03 Sep 2021 02:54:01 GMT  
		Size: 174.6 MB (174643286 bytes)  
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
$ docker pull buildpack-deps@sha256:0eeacd7d46019ece9dda8918d9976ff85578d8108a73ac7ed44ff3cc3aa32fe1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327743866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6fcb7ffe5e59562a791d18986a198b675f7b171f4eeaa206755542198904057`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853d83532467d1599448d38360ea9d52789d7d10f30c6734e17728c98743435b`  
		Last Modified: Fri, 03 Sep 2021 01:19:38 GMT  
		Size: 5.3 MB (5282881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6935e9ec29feb2101753d15eca8fa2727e2b060c07d2f720f471c55fb344c2a4`  
		Last Modified: Fri, 03 Sep 2021 01:19:39 GMT  
		Size: 11.3 MB (11250633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf6b2b625a6c874fcfb0e659f71235906f8459aa36ce32066b8efe1daf7c855`  
		Last Modified: Fri, 03 Sep 2021 01:20:07 GMT  
		Size: 55.9 MB (55916333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626b405c2848d11cb9e5ff331bbdc4a25b3874bca022fb01d015d9cc9f417cc8`  
		Last Modified: Fri, 03 Sep 2021 01:21:03 GMT  
		Size: 199.4 MB (199363086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4cbe9b6745b5af922a656e1d62acd8a038f7fd8d380e564bbdb7b25b95595ace
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301401029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd513018a9e3b431230adc2461695e8f74bd2b65f6e8645e4509f58f77252e9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:46:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:48:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918f43385735f5455e955ef94ef61f2089c0caebab840605cb52e5dd7525cd4`  
		Last Modified: Fri, 03 Sep 2021 01:59:04 GMT  
		Size: 53.3 MB (53297975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65f346af31b808f018e37721ec5d0556c4de13c57d89116afa4b6828afe09c5`  
		Last Modified: Fri, 03 Sep 2021 02:01:15 GMT  
		Size: 178.9 MB (178937584 bytes)  
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
$ docker pull buildpack-deps@sha256:40197898caa51e4f5c2a304bd81d55820af4a1476de2a1a330d051d454943f57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295584326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af2f830a774ba7fd46337da52dbfe51265f7563bc6cce99f5c38ad75cf30c14`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:07:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f48d5133e49359781fde1a8e72c81879ba30ffcb5b6d759f0ecb28fe6bbbe8`  
		Last Modified: Fri, 03 Sep 2021 02:19:40 GMT  
		Size: 5.1 MB (5137216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab672e8b32c6e3623bde683097d4c5fe5a73090dcb963e9f5512dfc21c485f58`  
		Last Modified: Fri, 03 Sep 2021 02:19:41 GMT  
		Size: 10.8 MB (10761458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7068e3642fc5ba5e489f8857ba725ba64ef0ce4b28acbf1545d133584bae2`  
		Last Modified: Fri, 03 Sep 2021 02:19:59 GMT  
		Size: 54.1 MB (54050487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02058994960995fa08f9f85746bee63cac5d73869afec780cbf963e361fe892`  
		Last Modified: Fri, 03 Sep 2021 02:20:31 GMT  
		Size: 172.4 MB (172434011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable`

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

## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:00ef0e1ed6ae3742f7b122d8218abd5ea6930bd68d52ea85fe28564fbacb8a1c
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
$ docker pull buildpack-deps@sha256:89a8e4c88902421a8ec8adc91e2cf9e808e860a68739a110c01aebe91b59c9e8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58603798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40c53b759346b2b704090e35da282424f48a13899669a6aff4084f8355de8a85`
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
$ docker pull buildpack-deps@sha256:f96c451143ba8ef2d97c78c62b8f2cfb2139be821eb01d2201714d40d0425257
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62015314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d634f6450bfc2871badaec2fe16a729b3acb4aaf7d10d46941b6f1b49dad976`
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

## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:e8bd06c9058b509c658bb6933521c295ad27e6bdf2876e4e2e801e8d302b1d57
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
$ docker pull buildpack-deps@sha256:04b27e881f1fd6778bbb2d8d0b731458d3000b2abe8f7e2259d97617f39b893c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106587812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f2d0d5fb01b8578c38085b55152fac616466476f7c3ccc7799c0082b32cdd4`
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
$ docker pull buildpack-deps@sha256:4b82ca05cfcc3d4db445a63e663876f11fadf48c6c04ff1efffa3cac11c5ebc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113280413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40551e8c31ce139ca23f251e1c53f664d21686d1c874cfc000837b7674b68dd2`
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

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:2cb37b188a530c3d81b8def93a5be2a1062bbcd5627bdd2e187c01dd9e71af18
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
$ docker pull buildpack-deps@sha256:e20d79afa0c9535fe3231377c6ee4df39fa7b7aae0bfaa47986c5b4f835d3ed9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286124730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8309dfe7b477df76d3a3edcb146b58d2f1222ab3881f9e3f1ff6474fdf42b695`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:55 GMT
ADD file:2edb17d6de848884fe9c4f448cf83c7eb38db986179ad828a28e287727206359 in / 
# Fri, 03 Sep 2021 00:50:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:35:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:35:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:39:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6cb7b6b06f67582053bf766e2dfc8cf86da6a819d6b0f89087b19d266364c4e`  
		Last Modified: Fri, 03 Sep 2021 01:06:27 GMT  
		Size: 48.2 MB (48153787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e990870d90c5fbe59daeaf6595ea5f84dfc9b19d83ceee42f1c77151b28c8`  
		Last Modified: Fri, 03 Sep 2021 02:54:23 GMT  
		Size: 7.4 MB (7376968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f97aee7b401dda2cdbd199f93baedfb4d6c1c77abcb61a736f63fc9818d541`  
		Last Modified: Fri, 03 Sep 2021 02:54:24 GMT  
		Size: 9.7 MB (9687490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df658833310cf636515e182b07f0f757747de5e7bf7cb2d5798c438dffe9a962`  
		Last Modified: Fri, 03 Sep 2021 02:55:13 GMT  
		Size: 49.6 MB (49574916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c5eacbd1943e12eba81a033914a38c27e596c6baab6126ef425dcec1b36a99`  
		Last Modified: Fri, 03 Sep 2021 02:57:09 GMT  
		Size: 171.3 MB (171331569 bytes)  
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
$ docker pull buildpack-deps@sha256:a9d2f53fb8f3c5d3342cfffc6c2a66a1ca03d58fa39476d86109e1caaf8985a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321916290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8c7bbcb5af6fee646d2097ff955284ad700486cf13df70b89023e993d37d7e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:07 GMT
ADD file:b57b08af647bb21d95dcfaaf631569421b159ccb57981aa968957e83d0d88be1 in / 
# Fri, 03 Sep 2021 00:40:07 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51869ffe8843ba6b44f606117326ad744bef79bc74f8eb46ebdc19e9299ede76`  
		Last Modified: Fri, 03 Sep 2021 00:48:31 GMT  
		Size: 51.2 MB (51207209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b7c65ab186ac667e4c325c9bc0aedb35fa5c3c0e94bcf31756f2242bad69c`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 8.0 MB (7999823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e5b243d4918f63b95623e21cd2da926e7a519a11f79d5dccbe9e1c921fdb3`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 10.3 MB (10339942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ad561c8654d0087f55d8ba8f2c88f6bf9760d1a07c98c20226182dd661df18`  
		Last Modified: Fri, 03 Sep 2021 01:21:49 GMT  
		Size: 53.4 MB (53438188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7076e49e31f46f892cc53ebc742d6b7aac932b484254aa2eebc010ca0de90549`  
		Last Modified: Fri, 03 Sep 2021 01:22:43 GMT  
		Size: 198.9 MB (198931128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d634063a8331fe4268a41b3671e01c2b40010cb1103b24ef8d58479399c4c2e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297107089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43fc77b654d792f05d7cbb25930e90bacd59e074b1fbc0bfdb319d8b890be9c9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:26 GMT
ADD file:b1e1d3ff824c87ebeca7b3a0ef30937ea44a74450c5e2b2d2ae40d557df10ca0 in / 
# Fri, 03 Sep 2021 01:10:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:49:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:50:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:52:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ba0bd93a428688eed3f712e236aed68cd618f1aa507a5f75a9041f2e9849710`  
		Last Modified: Fri, 03 Sep 2021 01:19:10 GMT  
		Size: 49.1 MB (49080081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbdd3e2a4240b488fa8b608a56ca7e673ac5ef915e2f613574e7216ba4bd4d`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 7.3 MB (7253475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39492d54de9c1aa951897ec16b4ed7089bac77f23415e8ba2a8afa6bdca35fcc`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08a1f31fe454064309426ca44c375688e97aae9e8881495a117da13b13d3406`  
		Last Modified: Fri, 03 Sep 2021 02:02:20 GMT  
		Size: 50.8 MB (50843995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02609cf933fae5e74db6107e0fc797cf5c673d66c6246d39e2867543a7c9e2bb`  
		Last Modified: Fri, 03 Sep 2021 02:04:28 GMT  
		Size: 179.9 MB (179913101 bytes)  
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
$ docker pull buildpack-deps@sha256:0dfdccd8f2e50a7fe191748419f24a6e62487c3033a08f6c45e4b7cdee793dc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294549065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75aca64b33ae679db5de7e6910db6d3a4551b9aa423452fdf55deb81d8635ecd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:12 GMT
ADD file:282d4f0b6aa732d36151d4d99869e435e6fa273ff73904ae6da0df618b7c2a3e in / 
# Fri, 03 Sep 2021 00:44:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:08:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:08:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:11:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:98373502f525a0ec193f60462454ed062dd42ded2a98cb5fab011b55ec824c77`  
		Last Modified: Fri, 03 Sep 2021 00:53:16 GMT  
		Size: 49.0 MB (49004112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcc170cd12eeca791be319fcc5b66571023e31a38e6dd0c2b630227e512460e`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 7.4 MB (7400980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab67ee15cd57c1d22855cdec415bdc1e7b43122552befb5143f4e3e061dd107`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 9.9 MB (9883239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492849c87aa7918355ea3ddd15023d5192779474cd1ad01937363046cd5ed777`  
		Last Modified: Fri, 03 Sep 2021 02:20:59 GMT  
		Size: 51.4 MB (51380450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f583bcb6e3e69399c59333e43ffaa7efcf40301ec6fec56dcecb4f1ee5b35be1`  
		Last Modified: Fri, 03 Sep 2021 02:21:28 GMT  
		Size: 176.9 MB (176880284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:0096028425fb87ab1f534c9ae686a9a6f25c66feb1fa2a176edc07b0fbc0c84c
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
$ docker pull buildpack-deps@sha256:654299e0118d6a69615e00c53b04d58fde3187ff53e7332965448d5a8b6cb7e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65218245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7958978b70ef9cc355af985d00871287d008c0a09cb758947b336312d38665c5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:55 GMT
ADD file:2edb17d6de848884fe9c4f448cf83c7eb38db986179ad828a28e287727206359 in / 
# Fri, 03 Sep 2021 00:50:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:35:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:35:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a6cb7b6b06f67582053bf766e2dfc8cf86da6a819d6b0f89087b19d266364c4e`  
		Last Modified: Fri, 03 Sep 2021 01:06:27 GMT  
		Size: 48.2 MB (48153787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e990870d90c5fbe59daeaf6595ea5f84dfc9b19d83ceee42f1c77151b28c8`  
		Last Modified: Fri, 03 Sep 2021 02:54:23 GMT  
		Size: 7.4 MB (7376968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f97aee7b401dda2cdbd199f93baedfb4d6c1c77abcb61a736f63fc9818d541`  
		Last Modified: Fri, 03 Sep 2021 02:54:24 GMT  
		Size: 9.7 MB (9687490 bytes)  
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
$ docker pull buildpack-deps@sha256:409bd0ff35f739218799caf530b96c8f0a81a073f110da04d0af46d02d94ca38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69546974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6ae4e01bc97eb70eacb03cab757785d3c6e6e409a2d6443876ee11c2be7384`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:07 GMT
ADD file:b57b08af647bb21d95dcfaaf631569421b159ccb57981aa968957e83d0d88be1 in / 
# Fri, 03 Sep 2021 00:40:07 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:51869ffe8843ba6b44f606117326ad744bef79bc74f8eb46ebdc19e9299ede76`  
		Last Modified: Fri, 03 Sep 2021 00:48:31 GMT  
		Size: 51.2 MB (51207209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b7c65ab186ac667e4c325c9bc0aedb35fa5c3c0e94bcf31756f2242bad69c`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 8.0 MB (7999823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e5b243d4918f63b95623e21cd2da926e7a519a11f79d5dccbe9e1c921fdb3`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 10.3 MB (10339942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2f28d7aade7f73d14ae1136cef4108958febc1311acc07fcc5fcc5a3078c265f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66349993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb0417ec2edc8a010da78cdc28304c5b85cddce016a1cbacbcdfdf4ac7a6462`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:26 GMT
ADD file:b1e1d3ff824c87ebeca7b3a0ef30937ea44a74450c5e2b2d2ae40d557df10ca0 in / 
# Fri, 03 Sep 2021 01:10:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:49:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6ba0bd93a428688eed3f712e236aed68cd618f1aa507a5f75a9041f2e9849710`  
		Last Modified: Fri, 03 Sep 2021 01:19:10 GMT  
		Size: 49.1 MB (49080081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbdd3e2a4240b488fa8b608a56ca7e673ac5ef915e2f613574e7216ba4bd4d`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 7.3 MB (7253475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39492d54de9c1aa951897ec16b4ed7089bac77f23415e8ba2a8afa6bdca35fcc`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 10.0 MB (10016437 bytes)  
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
$ docker pull buildpack-deps@sha256:833091c790c7673c548e2e68fc482448c15ac5fb2e6c0a88628b9e881f9e8e9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66288331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42deb34c0183bafb7ed29008b674d1aa82da25fcb658d14cb1d759811030ffff`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:12 GMT
ADD file:282d4f0b6aa732d36151d4d99869e435e6fa273ff73904ae6da0df618b7c2a3e in / 
# Fri, 03 Sep 2021 00:44:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:08:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:08:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:98373502f525a0ec193f60462454ed062dd42ded2a98cb5fab011b55ec824c77`  
		Last Modified: Fri, 03 Sep 2021 00:53:16 GMT  
		Size: 49.0 MB (49004112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcc170cd12eeca791be319fcc5b66571023e31a38e6dd0c2b630227e512460e`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 7.4 MB (7400980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab67ee15cd57c1d22855cdec415bdc1e7b43122552befb5143f4e3e061dd107`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 9.9 MB (9883239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:d4b3badbfa050224faf7fb987b034e2dc26578f552cb8fa691d61cfce4aef99b
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
$ docker pull buildpack-deps@sha256:d2eb0e782e068ad39cf40f1625eb353b831463e636f95693ae41fb05f691cdcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114793161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4876ab18741ccd6ccef6cd50c172e9fff1ef364bccb1d3e70b093053ea4dda0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:55 GMT
ADD file:2edb17d6de848884fe9c4f448cf83c7eb38db986179ad828a28e287727206359 in / 
# Fri, 03 Sep 2021 00:50:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:35:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:35:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6cb7b6b06f67582053bf766e2dfc8cf86da6a819d6b0f89087b19d266364c4e`  
		Last Modified: Fri, 03 Sep 2021 01:06:27 GMT  
		Size: 48.2 MB (48153787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e990870d90c5fbe59daeaf6595ea5f84dfc9b19d83ceee42f1c77151b28c8`  
		Last Modified: Fri, 03 Sep 2021 02:54:23 GMT  
		Size: 7.4 MB (7376968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f97aee7b401dda2cdbd199f93baedfb4d6c1c77abcb61a736f63fc9818d541`  
		Last Modified: Fri, 03 Sep 2021 02:54:24 GMT  
		Size: 9.7 MB (9687490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df658833310cf636515e182b07f0f757747de5e7bf7cb2d5798c438dffe9a962`  
		Last Modified: Fri, 03 Sep 2021 02:55:13 GMT  
		Size: 49.6 MB (49574916 bytes)  
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
$ docker pull buildpack-deps@sha256:4cbbd2739a0403a4bc5fb44d0c0547c78cb6b4b5725d748ea8aaec196c62bf51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122985162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:097bbb812919407eacd1ae1255f64f143c4e079f4ace3fa2d93973ef58a05977`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:07 GMT
ADD file:b57b08af647bb21d95dcfaaf631569421b159ccb57981aa968957e83d0d88be1 in / 
# Fri, 03 Sep 2021 00:40:07 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51869ffe8843ba6b44f606117326ad744bef79bc74f8eb46ebdc19e9299ede76`  
		Last Modified: Fri, 03 Sep 2021 00:48:31 GMT  
		Size: 51.2 MB (51207209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b7c65ab186ac667e4c325c9bc0aedb35fa5c3c0e94bcf31756f2242bad69c`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 8.0 MB (7999823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e5b243d4918f63b95623e21cd2da926e7a519a11f79d5dccbe9e1c921fdb3`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 10.3 MB (10339942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ad561c8654d0087f55d8ba8f2c88f6bf9760d1a07c98c20226182dd661df18`  
		Last Modified: Fri, 03 Sep 2021 01:21:49 GMT  
		Size: 53.4 MB (53438188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6ab856bb690e3f3d77b73c06897b06e791118de0900b70a0631d7650121f0011
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117193988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f098c7247d21412ac50e09a060a32e85b985ca806949eabd5b8c55abfe0d879`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:26 GMT
ADD file:b1e1d3ff824c87ebeca7b3a0ef30937ea44a74450c5e2b2d2ae40d557df10ca0 in / 
# Fri, 03 Sep 2021 01:10:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:49:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:50:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ba0bd93a428688eed3f712e236aed68cd618f1aa507a5f75a9041f2e9849710`  
		Last Modified: Fri, 03 Sep 2021 01:19:10 GMT  
		Size: 49.1 MB (49080081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbdd3e2a4240b488fa8b608a56ca7e673ac5ef915e2f613574e7216ba4bd4d`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 7.3 MB (7253475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39492d54de9c1aa951897ec16b4ed7089bac77f23415e8ba2a8afa6bdca35fcc`  
		Last Modified: Fri, 03 Sep 2021 02:01:33 GMT  
		Size: 10.0 MB (10016437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08a1f31fe454064309426ca44c375688e97aae9e8881495a117da13b13d3406`  
		Last Modified: Fri, 03 Sep 2021 02:02:20 GMT  
		Size: 50.8 MB (50843995 bytes)  
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
$ docker pull buildpack-deps@sha256:df83420f47187698a53a1d1619e3c8e76c62a31683d662fab930ad0f56c4a474
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117668781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09411ac234644b4a157d54187b1c193b7de35f4649ab96a23bff0dc7a43fe190`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:12 GMT
ADD file:282d4f0b6aa732d36151d4d99869e435e6fa273ff73904ae6da0df618b7c2a3e in / 
# Fri, 03 Sep 2021 00:44:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:08:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:08:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:98373502f525a0ec193f60462454ed062dd42ded2a98cb5fab011b55ec824c77`  
		Last Modified: Fri, 03 Sep 2021 00:53:16 GMT  
		Size: 49.0 MB (49004112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcc170cd12eeca791be319fcc5b66571023e31a38e6dd0c2b630227e512460e`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 7.4 MB (7400980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab67ee15cd57c1d22855cdec415bdc1e7b43122552befb5143f4e3e061dd107`  
		Last Modified: Fri, 03 Sep 2021 02:20:43 GMT  
		Size: 9.9 MB (9883239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492849c87aa7918355ea3ddd15023d5192779474cd1ad01937363046cd5ed777`  
		Last Modified: Fri, 03 Sep 2021 02:20:59 GMT  
		Size: 51.4 MB (51380450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:48885a657fa24cd5afeda8c2cbdf0574e118c803fa71d6222275d03343dd73fc
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
$ docker pull buildpack-deps@sha256:25400321d2573328a3a4a5ca398f3e0d11056d903e39f334939e80717fd8127d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120415442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c9ec9c2d5a6c44f4f20dee32d5687a7f6699b5ad60a5fd9da4530f37f0f010`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:31:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:32:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f9763e0efd7dcf980819e39cb728c9f11f3c3f7dd944e21177efba57f6fe3`  
		Last Modified: Fri, 03 Sep 2021 02:51:03 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95efca74ef694ced85d684e7faecd407beb97667568054d98e5e09166a32d88a`  
		Last Modified: Fri, 03 Sep 2021 02:51:05 GMT  
		Size: 10.6 MB (10570971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df2396712ed6cf1ebf81db19d8e162b1c621c3fca9971be211747d7e10bf8`  
		Last Modified: Fri, 03 Sep 2021 02:51:58 GMT  
		Size: 52.3 MB (52319329 bytes)  
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
$ docker pull buildpack-deps@sha256:ad88db1472e0c705f72cf52470e55fd98ca5e14e00e67cfa4c1ae2491f4b42ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128380780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f54f21a8eb6c7073aabdfbc66893ce44b6e77dbf73034a40c13c913bd246f5b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853d83532467d1599448d38360ea9d52789d7d10f30c6734e17728c98743435b`  
		Last Modified: Fri, 03 Sep 2021 01:19:38 GMT  
		Size: 5.3 MB (5282881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6935e9ec29feb2101753d15eca8fa2727e2b060c07d2f720f471c55fb344c2a4`  
		Last Modified: Fri, 03 Sep 2021 01:19:39 GMT  
		Size: 11.3 MB (11250633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf6b2b625a6c874fcfb0e659f71235906f8459aa36ce32066b8efe1daf7c855`  
		Last Modified: Fri, 03 Sep 2021 01:20:07 GMT  
		Size: 55.9 MB (55916333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6f7f0eda304eea56cad106a2326a1c13b9795bf40b8cb034bf22216101812a76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122463445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472a6e379480171cbaf23c6d657f64a0656a5f76461f1ee4e7b779f4d3d2e2da`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:46:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918f43385735f5455e955ef94ef61f2089c0caebab840605cb52e5dd7525cd4`  
		Last Modified: Fri, 03 Sep 2021 01:59:04 GMT  
		Size: 53.3 MB (53297975 bytes)  
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
$ docker pull buildpack-deps@sha256:485ac24b4b3a8b7585b955839727007d6a2758907be6a957c535027848236e2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aa3622158c598757cde789c4df5c79291a8281dfa04b2a762e7e95f1e603db9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f48d5133e49359781fde1a8e72c81879ba30ffcb5b6d759f0ecb28fe6bbbe8`  
		Last Modified: Fri, 03 Sep 2021 02:19:40 GMT  
		Size: 5.1 MB (5137216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab672e8b32c6e3623bde683097d4c5fe5a73090dcb963e9f5512dfc21c485f58`  
		Last Modified: Fri, 03 Sep 2021 02:19:41 GMT  
		Size: 10.8 MB (10761458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7068e3642fc5ba5e489f8857ba725ba64ef0ce4b28acbf1545d133584bae2`  
		Last Modified: Fri, 03 Sep 2021 02:19:59 GMT  
		Size: 54.1 MB (54050487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:b7b4f0ece65b074c9d6465add20a3fd59f023956d8d1461b383b807416e92590
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
$ docker pull buildpack-deps@sha256:312dbc24fd48a99d2c8e324c03a5dfb7928284770bbd559ec47b2b4d8382fe18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (296977595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83104ea9971af673818cd9916722260c75af80d5d3520275340b764a3e2806d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:53:41 GMT
ADD file:9d67c83a2e727f33502861325786047b9c6034b490854b93efb2d59cf973e5b6 in / 
# Fri, 03 Sep 2021 00:53:42 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:39:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:41:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:43:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c25501d6a46457c5895808abc531a7dcd2b4008bc42a432fcd73b6325c3fdacf`  
		Last Modified: Fri, 03 Sep 2021 01:10:41 GMT  
		Size: 53.0 MB (52980070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca497a6979f627d04639faa5571c98e112e1c56465986fce9d78c17101a5ce`  
		Last Modified: Fri, 03 Sep 2021 02:57:25 GMT  
		Size: 5.1 MB (5077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eab0927e6f1d00c87c3eed02237eb8b36a819bc0188dabfab4074f096423576`  
		Last Modified: Fri, 03 Sep 2021 02:57:28 GMT  
		Size: 10.6 MB (10595736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab42f59e6f95fa1040561c411658a005c01b13425791de2b04eb66b15d32f5a3`  
		Last Modified: Fri, 03 Sep 2021 02:58:18 GMT  
		Size: 53.4 MB (53391660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbdab329b941eb9b5a0920dd09c0f3b52f5900994fd8ac2a79843340f1255b9`  
		Last Modified: Fri, 03 Sep 2021 03:00:17 GMT  
		Size: 174.9 MB (174932511 bytes)  
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
$ docker pull buildpack-deps@sha256:594eba6af483ca41e9233481be60cd814ba90398bf03737f2551e73e46ec5aa6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.9 MB (303910086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0161f0f77632a8b6b2d5ab1ff8176ab0b046cec405e4ba28c3715d712ff40ade`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:53:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:57:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8b578c68c33ad5ddf748ce7497de380f1903d441aee0c8b0b1af0471180e1`  
		Last Modified: Fri, 03 Sep 2021 02:04:43 GMT  
		Size: 5.1 MB (5132409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a57f2a02c7810a593cba16221fab32426c75881bc128a91ef728048538e53`  
		Last Modified: Fri, 03 Sep 2021 02:04:45 GMT  
		Size: 10.9 MB (10900458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a709b007930a1acd8d8ea50132cb0b6a34e4f6f470c1b917f467d1263256229`  
		Last Modified: Fri, 03 Sep 2021 02:05:35 GMT  
		Size: 54.5 MB (54506202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ca150cc0a0aa1d2beaafe2c77fbea8098752fad83a288ae3b3e886c8433967`  
		Last Modified: Fri, 03 Sep 2021 02:07:42 GMT  
		Size: 179.2 MB (179236012 bytes)  
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
$ docker pull buildpack-deps@sha256:69c71c75852870453dc0d1277edbeb9ea1c9c28f01aa1a9892dfc39e09d09476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.9 MB (330944138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d681c903dd19ca6ed2ae3d8c0ea14fec1b73199236d7bbc5ca7d54928999190`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:16:10 GMT
ADD file:22169a464bc792387d0c6cd4ca985b70527601306f274a47f7a26223b125d1b8 in / 
# Fri, 03 Sep 2021 01:16:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:59:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:14:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d209f64ed888c716b8fc1f768d766ccf831d8a034eb5e3ca12945873acb106f6`  
		Last Modified: Fri, 03 Sep 2021 01:32:35 GMT  
		Size: 51.3 MB (51289049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da873824fc3fcd77f59d7598fa94a4e0eef799c270584961cd61b0193ad259c`  
		Last Modified: Fri, 03 Sep 2021 02:39:12 GMT  
		Size: 5.0 MB (4986349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfba85c856d5ce39bea54898a8e2d95aa9c37df4c646386dfd0d1099c262561`  
		Last Modified: Fri, 03 Sep 2021 02:39:16 GMT  
		Size: 10.3 MB (10313344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4008dd868e4d390b41b3510374a17a33a9fe636188767c8e61b168424fb1ec02`  
		Last Modified: Fri, 03 Sep 2021 02:41:24 GMT  
		Size: 51.8 MB (51762819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b8ae83be84c8d55337208fb9000f1b2a330bfea5fa83da9bc2d1a3bd17a8d`  
		Last Modified: Fri, 03 Sep 2021 02:47:19 GMT  
		Size: 212.6 MB (212592577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ee6ec64674c7094ece69127d33fd409aca766bc90372c49929d9cde777eddfb3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297684388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564aabb2b94f791d5fcad3ec0a5a9cf9618560055a58e4cf9fa3934c331741a9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:46:03 GMT
ADD file:4dec873e9e3022f644e228769ed26be34f63fb2d9b0ddc10816af8c9eaa11a15 in / 
# Fri, 03 Sep 2021 00:46:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:11:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:12:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:15:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c1522cfd5f84804048a7cb823dfa679d77781943db2c6e71d872921d6d7542e`  
		Last Modified: Fri, 03 Sep 2021 00:54:32 GMT  
		Size: 53.8 MB (53772150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305bda156f1bbe0e441c40cfe1badc3590f18bfe3b1708ce8d2050c033c40ea2`  
		Last Modified: Fri, 03 Sep 2021 02:21:38 GMT  
		Size: 5.2 MB (5153859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac738bf714d2148f583c8c4ff6147a0840fc80305cf406c832bb05ad7eeaa9`  
		Last Modified: Fri, 03 Sep 2021 02:21:39 GMT  
		Size: 10.8 MB (10791081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d4c39e7ec2e00b89fdc841a618fe0f405052037f5cfe5c1660d4c10ca31846`  
		Last Modified: Fri, 03 Sep 2021 02:21:56 GMT  
		Size: 55.2 MB (55154031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f94cae41323c5342edb9cb4f876d2c8817d403218531980e3dd840ba496505`  
		Last Modified: Fri, 03 Sep 2021 02:22:25 GMT  
		Size: 172.8 MB (172813267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:160fb6732d0c7e61ee4d351ced056fb9a48cacb5d55b57a436d60b8f4526e88e
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
$ docker pull buildpack-deps@sha256:b9f458071c07c1922362c241070e5e92fcae56e600b5fba756c6c7f016a7b8dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68653424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e3b381e72d26f967883d0038a368254c7a7d6c8a34171e0360b55d6a190f08`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:53:41 GMT
ADD file:9d67c83a2e727f33502861325786047b9c6034b490854b93efb2d59cf973e5b6 in / 
# Fri, 03 Sep 2021 00:53:42 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:39:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c25501d6a46457c5895808abc531a7dcd2b4008bc42a432fcd73b6325c3fdacf`  
		Last Modified: Fri, 03 Sep 2021 01:10:41 GMT  
		Size: 53.0 MB (52980070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca497a6979f627d04639faa5571c98e112e1c56465986fce9d78c17101a5ce`  
		Last Modified: Fri, 03 Sep 2021 02:57:25 GMT  
		Size: 5.1 MB (5077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eab0927e6f1d00c87c3eed02237eb8b36a819bc0188dabfab4074f096423576`  
		Last Modified: Fri, 03 Sep 2021 02:57:28 GMT  
		Size: 10.6 MB (10595736 bytes)  
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
$ docker pull buildpack-deps@sha256:172f86014cfd23f8534f1d81a96c73a480f0fcf8f38814951938b8646bc3cf67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73100008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ceb13982ea1259ee29ad6b3ac68115fee570615ace45461936af7d9edd4e5f8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:36 GMT
ADD file:64515d15f0b2fac0544e320a88716de6bf306c10f7e9400a945fca420a730843 in / 
# Fri, 03 Sep 2021 00:41:37 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:965ebee0ec76f6f76a0d14e40b7923292e9028532546ec1a748a8fed8267c897`  
		Last Modified: Fri, 03 Sep 2021 00:51:22 GMT  
		Size: 56.5 MB (56525268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56089068afb291eba965e50fb15a03f5ae7c433295ed8d952822fe54d1c1dd97`  
		Last Modified: Fri, 03 Sep 2021 01:22:57 GMT  
		Size: 5.3 MB (5303864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab52954bb9b6200d56553ce69fb7dae734a92c479ff8e38af69fa29a7d28110c`  
		Last Modified: Fri, 03 Sep 2021 01:22:58 GMT  
		Size: 11.3 MB (11270876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0742b4ef0a1e6d36f6a1baf7431d7ce25444bf9575509f0ba031b8b243cf1251
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70167872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fac613c7b4b40ce813d10d55b6b0ad58587ca17e308844e5aa980796ab1392f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:53:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8b578c68c33ad5ddf748ce7497de380f1903d441aee0c8b0b1af0471180e1`  
		Last Modified: Fri, 03 Sep 2021 02:04:43 GMT  
		Size: 5.1 MB (5132409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a57f2a02c7810a593cba16221fab32426c75881bc128a91ef728048538e53`  
		Last Modified: Fri, 03 Sep 2021 02:04:45 GMT  
		Size: 10.9 MB (10900458 bytes)  
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
$ docker pull buildpack-deps@sha256:bedca7b6c6375e09dd1ffb3eec3b607a8b8b9a15dd142b77525579bde87a41b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66588742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183f6c97e7e26c4086f4b6cb32c3908d6b090e56eab64119950c4a699dca29b0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:16:10 GMT
ADD file:22169a464bc792387d0c6cd4ca985b70527601306f274a47f7a26223b125d1b8 in / 
# Fri, 03 Sep 2021 01:16:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:59:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d209f64ed888c716b8fc1f768d766ccf831d8a034eb5e3ca12945873acb106f6`  
		Last Modified: Fri, 03 Sep 2021 01:32:35 GMT  
		Size: 51.3 MB (51289049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da873824fc3fcd77f59d7598fa94a4e0eef799c270584961cd61b0193ad259c`  
		Last Modified: Fri, 03 Sep 2021 02:39:12 GMT  
		Size: 5.0 MB (4986349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfba85c856d5ce39bea54898a8e2d95aa9c37df4c646386dfd0d1099c262561`  
		Last Modified: Fri, 03 Sep 2021 02:39:16 GMT  
		Size: 10.3 MB (10313344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:91057d86526bc5e96ff66eeb074c812f9321e33bef9d4b0ced773e1083ae997c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69717090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66bb7f34fb2e0b2a3dd65188ea09c38f4c42f4f90fe3d73d760f0816a9dde63b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:46:03 GMT
ADD file:4dec873e9e3022f644e228769ed26be34f63fb2d9b0ddc10816af8c9eaa11a15 in / 
# Fri, 03 Sep 2021 00:46:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:11:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:12:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2c1522cfd5f84804048a7cb823dfa679d77781943db2c6e71d872921d6d7542e`  
		Last Modified: Fri, 03 Sep 2021 00:54:32 GMT  
		Size: 53.8 MB (53772150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305bda156f1bbe0e441c40cfe1badc3590f18bfe3b1708ce8d2050c033c40ea2`  
		Last Modified: Fri, 03 Sep 2021 02:21:38 GMT  
		Size: 5.2 MB (5153859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac738bf714d2148f583c8c4ff6147a0840fc80305cf406c832bb05ad7eeaa9`  
		Last Modified: Fri, 03 Sep 2021 02:21:39 GMT  
		Size: 10.8 MB (10791081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:468dabbed82f94098143cae8671e5332569a713921a0df9d9983b603374d71b8
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
$ docker pull buildpack-deps@sha256:f4d652abef61df48e9ffc5b9cfa0ff60275c7ece073c683f3470789e1ee2eae4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122045084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce452975c108df26a1608befc48d7763e67342afecc2dc1030811fa8f36585aa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:53:41 GMT
ADD file:9d67c83a2e727f33502861325786047b9c6034b490854b93efb2d59cf973e5b6 in / 
# Fri, 03 Sep 2021 00:53:42 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:39:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:41:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c25501d6a46457c5895808abc531a7dcd2b4008bc42a432fcd73b6325c3fdacf`  
		Last Modified: Fri, 03 Sep 2021 01:10:41 GMT  
		Size: 53.0 MB (52980070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca497a6979f627d04639faa5571c98e112e1c56465986fce9d78c17101a5ce`  
		Last Modified: Fri, 03 Sep 2021 02:57:25 GMT  
		Size: 5.1 MB (5077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eab0927e6f1d00c87c3eed02237eb8b36a819bc0188dabfab4074f096423576`  
		Last Modified: Fri, 03 Sep 2021 02:57:28 GMT  
		Size: 10.6 MB (10595736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab42f59e6f95fa1040561c411658a005c01b13425791de2b04eb66b15d32f5a3`  
		Last Modified: Fri, 03 Sep 2021 02:58:18 GMT  
		Size: 53.4 MB (53391660 bytes)  
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
$ docker pull buildpack-deps@sha256:5e902fe3e8b8a92742d88713fae4924948e30a80da779cbbb73d5209c94f20d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.2 MB (130210303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a489eac282dc42cf470be83be408afb4620ba4535365f52b1c9a23b11639610a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:36 GMT
ADD file:64515d15f0b2fac0544e320a88716de6bf306c10f7e9400a945fca420a730843 in / 
# Fri, 03 Sep 2021 00:41:37 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:15:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:965ebee0ec76f6f76a0d14e40b7923292e9028532546ec1a748a8fed8267c897`  
		Last Modified: Fri, 03 Sep 2021 00:51:22 GMT  
		Size: 56.5 MB (56525268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56089068afb291eba965e50fb15a03f5ae7c433295ed8d952822fe54d1c1dd97`  
		Last Modified: Fri, 03 Sep 2021 01:22:57 GMT  
		Size: 5.3 MB (5303864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab52954bb9b6200d56553ce69fb7dae734a92c479ff8e38af69fa29a7d28110c`  
		Last Modified: Fri, 03 Sep 2021 01:22:58 GMT  
		Size: 11.3 MB (11270876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e266a96f5269409185770fdf13c62fab48d43de3f82cf97cb0f93890ae2b4a2`  
		Last Modified: Fri, 03 Sep 2021 01:23:25 GMT  
		Size: 57.1 MB (57110295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e7bbed7ac5659c6cd1aececdfaa4dc4744c5e258ee5c650a8ec37b539fda309b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124674074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f801a22581fced8c27b30a1378a19368e58a491bf7f4c84d59eb7a011e8343`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:53:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8b578c68c33ad5ddf748ce7497de380f1903d441aee0c8b0b1af0471180e1`  
		Last Modified: Fri, 03 Sep 2021 02:04:43 GMT  
		Size: 5.1 MB (5132409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a57f2a02c7810a593cba16221fab32426c75881bc128a91ef728048538e53`  
		Last Modified: Fri, 03 Sep 2021 02:04:45 GMT  
		Size: 10.9 MB (10900458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a709b007930a1acd8d8ea50132cb0b6a34e4f6f470c1b917f467d1263256229`  
		Last Modified: Fri, 03 Sep 2021 02:05:35 GMT  
		Size: 54.5 MB (54506202 bytes)  
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
$ docker pull buildpack-deps@sha256:75dacb3d7efa37c55a2ee04f476c40809377e9cbe9f4873bbb31898f271409e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118351561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0997c4f2769ed1634128d9554d1a4e7dd0308c463b797eeb1c5b77933109c777`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:16:10 GMT
ADD file:22169a464bc792387d0c6cd4ca985b70527601306f274a47f7a26223b125d1b8 in / 
# Fri, 03 Sep 2021 01:16:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:59:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d209f64ed888c716b8fc1f768d766ccf831d8a034eb5e3ca12945873acb106f6`  
		Last Modified: Fri, 03 Sep 2021 01:32:35 GMT  
		Size: 51.3 MB (51289049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da873824fc3fcd77f59d7598fa94a4e0eef799c270584961cd61b0193ad259c`  
		Last Modified: Fri, 03 Sep 2021 02:39:12 GMT  
		Size: 5.0 MB (4986349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfba85c856d5ce39bea54898a8e2d95aa9c37df4c646386dfd0d1099c262561`  
		Last Modified: Fri, 03 Sep 2021 02:39:16 GMT  
		Size: 10.3 MB (10313344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4008dd868e4d390b41b3510374a17a33a9fe636188767c8e61b168424fb1ec02`  
		Last Modified: Fri, 03 Sep 2021 02:41:24 GMT  
		Size: 51.8 MB (51762819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:75558dfed6e9f5fec05b1fdb390d686321ea9d9e006fbe11632fd936473b5cd9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124871121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4667324b850550595dc9a21fae5846f605d83d5551da54cc420b955bdffabc72`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:46:03 GMT
ADD file:4dec873e9e3022f644e228769ed26be34f63fb2d9b0ddc10816af8c9eaa11a15 in / 
# Fri, 03 Sep 2021 00:46:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:11:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:12:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c1522cfd5f84804048a7cb823dfa679d77781943db2c6e71d872921d6d7542e`  
		Last Modified: Fri, 03 Sep 2021 00:54:32 GMT  
		Size: 53.8 MB (53772150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305bda156f1bbe0e441c40cfe1badc3590f18bfe3b1708ce8d2050c033c40ea2`  
		Last Modified: Fri, 03 Sep 2021 02:21:38 GMT  
		Size: 5.2 MB (5153859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac738bf714d2148f583c8c4ff6147a0840fc80305cf406c832bb05ad7eeaa9`  
		Last Modified: Fri, 03 Sep 2021 02:21:39 GMT  
		Size: 10.8 MB (10791081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d4c39e7ec2e00b89fdc841a618fe0f405052037f5cfe5c1660d4c10ca31846`  
		Last Modified: Fri, 03 Sep 2021 02:21:56 GMT  
		Size: 55.2 MB (55154031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:f6c911ff12af5e812a96df5b24fc67cc7d2924c07d13d52f9d3ee90fc9f8b81c
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
$ docker pull buildpack-deps@sha256:9b65dde79ee2e03922f844db61fb0dd2e97297df7ab620ead878c347744f430c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295058728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6bab944fcaa224ed17b83c9812ae6117a5f28d269b0b0477135bb05e601420e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:31:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:32:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:34:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f9763e0efd7dcf980819e39cb728c9f11f3c3f7dd944e21177efba57f6fe3`  
		Last Modified: Fri, 03 Sep 2021 02:51:03 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95efca74ef694ced85d684e7faecd407beb97667568054d98e5e09166a32d88a`  
		Last Modified: Fri, 03 Sep 2021 02:51:05 GMT  
		Size: 10.6 MB (10570971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df2396712ed6cf1ebf81db19d8e162b1c621c3fca9971be211747d7e10bf8`  
		Last Modified: Fri, 03 Sep 2021 02:51:58 GMT  
		Size: 52.3 MB (52319329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0847f5ab2d0f284ff33db1f85872a599e314abb845aaab72c0e9a3e57a063c96`  
		Last Modified: Fri, 03 Sep 2021 02:54:01 GMT  
		Size: 174.6 MB (174643286 bytes)  
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
$ docker pull buildpack-deps@sha256:0eeacd7d46019ece9dda8918d9976ff85578d8108a73ac7ed44ff3cc3aa32fe1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327743866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6fcb7ffe5e59562a791d18986a198b675f7b171f4eeaa206755542198904057`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853d83532467d1599448d38360ea9d52789d7d10f30c6734e17728c98743435b`  
		Last Modified: Fri, 03 Sep 2021 01:19:38 GMT  
		Size: 5.3 MB (5282881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6935e9ec29feb2101753d15eca8fa2727e2b060c07d2f720f471c55fb344c2a4`  
		Last Modified: Fri, 03 Sep 2021 01:19:39 GMT  
		Size: 11.3 MB (11250633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf6b2b625a6c874fcfb0e659f71235906f8459aa36ce32066b8efe1daf7c855`  
		Last Modified: Fri, 03 Sep 2021 01:20:07 GMT  
		Size: 55.9 MB (55916333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626b405c2848d11cb9e5ff331bbdc4a25b3874bca022fb01d015d9cc9f417cc8`  
		Last Modified: Fri, 03 Sep 2021 01:21:03 GMT  
		Size: 199.4 MB (199363086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4cbe9b6745b5af922a656e1d62acd8a038f7fd8d380e564bbdb7b25b95595ace
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301401029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd513018a9e3b431230adc2461695e8f74bd2b65f6e8645e4509f58f77252e9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:46:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:48:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918f43385735f5455e955ef94ef61f2089c0caebab840605cb52e5dd7525cd4`  
		Last Modified: Fri, 03 Sep 2021 01:59:04 GMT  
		Size: 53.3 MB (53297975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65f346af31b808f018e37721ec5d0556c4de13c57d89116afa4b6828afe09c5`  
		Last Modified: Fri, 03 Sep 2021 02:01:15 GMT  
		Size: 178.9 MB (178937584 bytes)  
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
$ docker pull buildpack-deps@sha256:40197898caa51e4f5c2a304bd81d55820af4a1476de2a1a330d051d454943f57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295584326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af2f830a774ba7fd46337da52dbfe51265f7563bc6cce99f5c38ad75cf30c14`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:07:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f48d5133e49359781fde1a8e72c81879ba30ffcb5b6d759f0ecb28fe6bbbe8`  
		Last Modified: Fri, 03 Sep 2021 02:19:40 GMT  
		Size: 5.1 MB (5137216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab672e8b32c6e3623bde683097d4c5fe5a73090dcb963e9f5512dfc21c485f58`  
		Last Modified: Fri, 03 Sep 2021 02:19:41 GMT  
		Size: 10.8 MB (10761458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7068e3642fc5ba5e489f8857ba725ba64ef0ce4b28acbf1545d133584bae2`  
		Last Modified: Fri, 03 Sep 2021 02:19:59 GMT  
		Size: 54.1 MB (54050487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02058994960995fa08f9f85746bee63cac5d73869afec780cbf963e361fe892`  
		Last Modified: Fri, 03 Sep 2021 02:20:31 GMT  
		Size: 172.4 MB (172434011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:ae9619a5c3c818d5149c0130318f141746acf3f6a1a24b58383ff902654a83e8
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
$ docker pull buildpack-deps@sha256:c1bf509fa76457be540f8f2fb10d9d26aa4890c9a4346c713745b6206fdda4be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68096113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73cdc4ca1ff77a007de35ea79cc9c08626250d2979cb0558df1bac7e1abd8c70`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:31:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f9763e0efd7dcf980819e39cb728c9f11f3c3f7dd944e21177efba57f6fe3`  
		Last Modified: Fri, 03 Sep 2021 02:51:03 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95efca74ef694ced85d684e7faecd407beb97667568054d98e5e09166a32d88a`  
		Last Modified: Fri, 03 Sep 2021 02:51:05 GMT  
		Size: 10.6 MB (10570971 bytes)  
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
$ docker pull buildpack-deps@sha256:ca1f95f69b1217eedf8fd5df25b029787d2b20be1c3808d4b56a7809cfafb72e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72464447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5250d94db9c58649245be60756b66f56ad4035644a1d6f28e3abd1e9e21ec49a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853d83532467d1599448d38360ea9d52789d7d10f30c6734e17728c98743435b`  
		Last Modified: Fri, 03 Sep 2021 01:19:38 GMT  
		Size: 5.3 MB (5282881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6935e9ec29feb2101753d15eca8fa2727e2b060c07d2f720f471c55fb344c2a4`  
		Last Modified: Fri, 03 Sep 2021 01:19:39 GMT  
		Size: 11.3 MB (11250633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1a5a8c8829bff1d7a89f8d97006a6ea359c46bb260fe809df4e907b5afd30a91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69165470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e5a9049a5620e106a070b8340f0b607aa86268008ceffc8ca4c29af118cfa3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
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
$ docker pull buildpack-deps@sha256:28124d888ebc509c072830169a01df6f23dcbbc8d88409f6aa3510b89267f1e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69099828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4861250614c542c631365e5d324fc1d562da14639c4308cea90abf09db002747`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f48d5133e49359781fde1a8e72c81879ba30ffcb5b6d759f0ecb28fe6bbbe8`  
		Last Modified: Fri, 03 Sep 2021 02:19:40 GMT  
		Size: 5.1 MB (5137216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab672e8b32c6e3623bde683097d4c5fe5a73090dcb963e9f5512dfc21c485f58`  
		Last Modified: Fri, 03 Sep 2021 02:19:41 GMT  
		Size: 10.8 MB (10761458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:48885a657fa24cd5afeda8c2cbdf0574e118c803fa71d6222275d03343dd73fc
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
$ docker pull buildpack-deps@sha256:25400321d2573328a3a4a5ca398f3e0d11056d903e39f334939e80717fd8127d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120415442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c9ec9c2d5a6c44f4f20dee32d5687a7f6699b5ad60a5fd9da4530f37f0f010`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:31:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:32:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f9763e0efd7dcf980819e39cb728c9f11f3c3f7dd944e21177efba57f6fe3`  
		Last Modified: Fri, 03 Sep 2021 02:51:03 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95efca74ef694ced85d684e7faecd407beb97667568054d98e5e09166a32d88a`  
		Last Modified: Fri, 03 Sep 2021 02:51:05 GMT  
		Size: 10.6 MB (10570971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df2396712ed6cf1ebf81db19d8e162b1c621c3fca9971be211747d7e10bf8`  
		Last Modified: Fri, 03 Sep 2021 02:51:58 GMT  
		Size: 52.3 MB (52319329 bytes)  
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
$ docker pull buildpack-deps@sha256:ad88db1472e0c705f72cf52470e55fd98ca5e14e00e67cfa4c1ae2491f4b42ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128380780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f54f21a8eb6c7073aabdfbc66893ce44b6e77dbf73034a40c13c913bd246f5b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853d83532467d1599448d38360ea9d52789d7d10f30c6734e17728c98743435b`  
		Last Modified: Fri, 03 Sep 2021 01:19:38 GMT  
		Size: 5.3 MB (5282881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6935e9ec29feb2101753d15eca8fa2727e2b060c07d2f720f471c55fb344c2a4`  
		Last Modified: Fri, 03 Sep 2021 01:19:39 GMT  
		Size: 11.3 MB (11250633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf6b2b625a6c874fcfb0e659f71235906f8459aa36ce32066b8efe1daf7c855`  
		Last Modified: Fri, 03 Sep 2021 01:20:07 GMT  
		Size: 55.9 MB (55916333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6f7f0eda304eea56cad106a2326a1c13b9795bf40b8cb034bf22216101812a76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122463445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472a6e379480171cbaf23c6d657f64a0656a5f76461f1ee4e7b779f4d3d2e2da`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:46:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918f43385735f5455e955ef94ef61f2089c0caebab840605cb52e5dd7525cd4`  
		Last Modified: Fri, 03 Sep 2021 01:59:04 GMT  
		Size: 53.3 MB (53297975 bytes)  
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
$ docker pull buildpack-deps@sha256:485ac24b4b3a8b7585b955839727007d6a2758907be6a957c535027848236e2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aa3622158c598757cde789c4df5c79291a8281dfa04b2a762e7e95f1e603db9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f48d5133e49359781fde1a8e72c81879ba30ffcb5b6d759f0ecb28fe6bbbe8`  
		Last Modified: Fri, 03 Sep 2021 02:19:40 GMT  
		Size: 5.1 MB (5137216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab672e8b32c6e3623bde683097d4c5fe5a73090dcb963e9f5512dfc21c485f58`  
		Last Modified: Fri, 03 Sep 2021 02:19:41 GMT  
		Size: 10.8 MB (10761458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7068e3642fc5ba5e489f8857ba725ba64ef0ce4b28acbf1545d133584bae2`  
		Last Modified: Fri, 03 Sep 2021 02:19:59 GMT  
		Size: 54.1 MB (54050487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `buildpack-deps:stretch-curl`

```console
$ docker pull buildpack-deps@sha256:00ef0e1ed6ae3742f7b122d8218abd5ea6930bd68d52ea85fe28564fbacb8a1c
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
$ docker pull buildpack-deps@sha256:89a8e4c88902421a8ec8adc91e2cf9e808e860a68739a110c01aebe91b59c9e8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58603798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40c53b759346b2b704090e35da282424f48a13899669a6aff4084f8355de8a85`
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
$ docker pull buildpack-deps@sha256:f96c451143ba8ef2d97c78c62b8f2cfb2139be821eb01d2201714d40d0425257
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62015314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d634f6450bfc2871badaec2fe16a729b3acb4aaf7d10d46941b6f1b49dad976`
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

## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:e8bd06c9058b509c658bb6933521c295ad27e6bdf2876e4e2e801e8d302b1d57
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
$ docker pull buildpack-deps@sha256:04b27e881f1fd6778bbb2d8d0b731458d3000b2abe8f7e2259d97617f39b893c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106587812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f2d0d5fb01b8578c38085b55152fac616466476f7c3ccc7799c0082b32cdd4`
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
$ docker pull buildpack-deps@sha256:4b82ca05cfcc3d4db445a63e663876f11fadf48c6c04ff1efffa3cac11c5ebc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113280413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40551e8c31ce139ca23f251e1c53f664d21686d1c874cfc000837b7674b68dd2`
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

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:b7b4f0ece65b074c9d6465add20a3fd59f023956d8d1461b383b807416e92590
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
$ docker pull buildpack-deps@sha256:312dbc24fd48a99d2c8e324c03a5dfb7928284770bbd559ec47b2b4d8382fe18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (296977595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83104ea9971af673818cd9916722260c75af80d5d3520275340b764a3e2806d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:53:41 GMT
ADD file:9d67c83a2e727f33502861325786047b9c6034b490854b93efb2d59cf973e5b6 in / 
# Fri, 03 Sep 2021 00:53:42 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:39:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:41:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:43:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c25501d6a46457c5895808abc531a7dcd2b4008bc42a432fcd73b6325c3fdacf`  
		Last Modified: Fri, 03 Sep 2021 01:10:41 GMT  
		Size: 53.0 MB (52980070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca497a6979f627d04639faa5571c98e112e1c56465986fce9d78c17101a5ce`  
		Last Modified: Fri, 03 Sep 2021 02:57:25 GMT  
		Size: 5.1 MB (5077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eab0927e6f1d00c87c3eed02237eb8b36a819bc0188dabfab4074f096423576`  
		Last Modified: Fri, 03 Sep 2021 02:57:28 GMT  
		Size: 10.6 MB (10595736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab42f59e6f95fa1040561c411658a005c01b13425791de2b04eb66b15d32f5a3`  
		Last Modified: Fri, 03 Sep 2021 02:58:18 GMT  
		Size: 53.4 MB (53391660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbdab329b941eb9b5a0920dd09c0f3b52f5900994fd8ac2a79843340f1255b9`  
		Last Modified: Fri, 03 Sep 2021 03:00:17 GMT  
		Size: 174.9 MB (174932511 bytes)  
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
$ docker pull buildpack-deps@sha256:594eba6af483ca41e9233481be60cd814ba90398bf03737f2551e73e46ec5aa6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.9 MB (303910086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0161f0f77632a8b6b2d5ab1ff8176ab0b046cec405e4ba28c3715d712ff40ade`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:53:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:57:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8b578c68c33ad5ddf748ce7497de380f1903d441aee0c8b0b1af0471180e1`  
		Last Modified: Fri, 03 Sep 2021 02:04:43 GMT  
		Size: 5.1 MB (5132409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a57f2a02c7810a593cba16221fab32426c75881bc128a91ef728048538e53`  
		Last Modified: Fri, 03 Sep 2021 02:04:45 GMT  
		Size: 10.9 MB (10900458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a709b007930a1acd8d8ea50132cb0b6a34e4f6f470c1b917f467d1263256229`  
		Last Modified: Fri, 03 Sep 2021 02:05:35 GMT  
		Size: 54.5 MB (54506202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ca150cc0a0aa1d2beaafe2c77fbea8098752fad83a288ae3b3e886c8433967`  
		Last Modified: Fri, 03 Sep 2021 02:07:42 GMT  
		Size: 179.2 MB (179236012 bytes)  
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
$ docker pull buildpack-deps@sha256:69c71c75852870453dc0d1277edbeb9ea1c9c28f01aa1a9892dfc39e09d09476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.9 MB (330944138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d681c903dd19ca6ed2ae3d8c0ea14fec1b73199236d7bbc5ca7d54928999190`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:16:10 GMT
ADD file:22169a464bc792387d0c6cd4ca985b70527601306f274a47f7a26223b125d1b8 in / 
# Fri, 03 Sep 2021 01:16:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:59:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:14:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d209f64ed888c716b8fc1f768d766ccf831d8a034eb5e3ca12945873acb106f6`  
		Last Modified: Fri, 03 Sep 2021 01:32:35 GMT  
		Size: 51.3 MB (51289049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da873824fc3fcd77f59d7598fa94a4e0eef799c270584961cd61b0193ad259c`  
		Last Modified: Fri, 03 Sep 2021 02:39:12 GMT  
		Size: 5.0 MB (4986349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfba85c856d5ce39bea54898a8e2d95aa9c37df4c646386dfd0d1099c262561`  
		Last Modified: Fri, 03 Sep 2021 02:39:16 GMT  
		Size: 10.3 MB (10313344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4008dd868e4d390b41b3510374a17a33a9fe636188767c8e61b168424fb1ec02`  
		Last Modified: Fri, 03 Sep 2021 02:41:24 GMT  
		Size: 51.8 MB (51762819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b8ae83be84c8d55337208fb9000f1b2a330bfea5fa83da9bc2d1a3bd17a8d`  
		Last Modified: Fri, 03 Sep 2021 02:47:19 GMT  
		Size: 212.6 MB (212592577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ee6ec64674c7094ece69127d33fd409aca766bc90372c49929d9cde777eddfb3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297684388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564aabb2b94f791d5fcad3ec0a5a9cf9618560055a58e4cf9fa3934c331741a9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:46:03 GMT
ADD file:4dec873e9e3022f644e228769ed26be34f63fb2d9b0ddc10816af8c9eaa11a15 in / 
# Fri, 03 Sep 2021 00:46:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:11:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:12:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:15:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c1522cfd5f84804048a7cb823dfa679d77781943db2c6e71d872921d6d7542e`  
		Last Modified: Fri, 03 Sep 2021 00:54:32 GMT  
		Size: 53.8 MB (53772150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305bda156f1bbe0e441c40cfe1badc3590f18bfe3b1708ce8d2050c033c40ea2`  
		Last Modified: Fri, 03 Sep 2021 02:21:38 GMT  
		Size: 5.2 MB (5153859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac738bf714d2148f583c8c4ff6147a0840fc80305cf406c832bb05ad7eeaa9`  
		Last Modified: Fri, 03 Sep 2021 02:21:39 GMT  
		Size: 10.8 MB (10791081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d4c39e7ec2e00b89fdc841a618fe0f405052037f5cfe5c1660d4c10ca31846`  
		Last Modified: Fri, 03 Sep 2021 02:21:56 GMT  
		Size: 55.2 MB (55154031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f94cae41323c5342edb9cb4f876d2c8817d403218531980e3dd840ba496505`  
		Last Modified: Fri, 03 Sep 2021 02:22:25 GMT  
		Size: 172.8 MB (172813267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:160fb6732d0c7e61ee4d351ced056fb9a48cacb5d55b57a436d60b8f4526e88e
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
$ docker pull buildpack-deps@sha256:b9f458071c07c1922362c241070e5e92fcae56e600b5fba756c6c7f016a7b8dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68653424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e3b381e72d26f967883d0038a368254c7a7d6c8a34171e0360b55d6a190f08`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:53:41 GMT
ADD file:9d67c83a2e727f33502861325786047b9c6034b490854b93efb2d59cf973e5b6 in / 
# Fri, 03 Sep 2021 00:53:42 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:39:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c25501d6a46457c5895808abc531a7dcd2b4008bc42a432fcd73b6325c3fdacf`  
		Last Modified: Fri, 03 Sep 2021 01:10:41 GMT  
		Size: 53.0 MB (52980070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca497a6979f627d04639faa5571c98e112e1c56465986fce9d78c17101a5ce`  
		Last Modified: Fri, 03 Sep 2021 02:57:25 GMT  
		Size: 5.1 MB (5077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eab0927e6f1d00c87c3eed02237eb8b36a819bc0188dabfab4074f096423576`  
		Last Modified: Fri, 03 Sep 2021 02:57:28 GMT  
		Size: 10.6 MB (10595736 bytes)  
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
$ docker pull buildpack-deps@sha256:172f86014cfd23f8534f1d81a96c73a480f0fcf8f38814951938b8646bc3cf67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73100008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ceb13982ea1259ee29ad6b3ac68115fee570615ace45461936af7d9edd4e5f8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:36 GMT
ADD file:64515d15f0b2fac0544e320a88716de6bf306c10f7e9400a945fca420a730843 in / 
# Fri, 03 Sep 2021 00:41:37 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:965ebee0ec76f6f76a0d14e40b7923292e9028532546ec1a748a8fed8267c897`  
		Last Modified: Fri, 03 Sep 2021 00:51:22 GMT  
		Size: 56.5 MB (56525268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56089068afb291eba965e50fb15a03f5ae7c433295ed8d952822fe54d1c1dd97`  
		Last Modified: Fri, 03 Sep 2021 01:22:57 GMT  
		Size: 5.3 MB (5303864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab52954bb9b6200d56553ce69fb7dae734a92c479ff8e38af69fa29a7d28110c`  
		Last Modified: Fri, 03 Sep 2021 01:22:58 GMT  
		Size: 11.3 MB (11270876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0742b4ef0a1e6d36f6a1baf7431d7ce25444bf9575509f0ba031b8b243cf1251
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70167872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fac613c7b4b40ce813d10d55b6b0ad58587ca17e308844e5aa980796ab1392f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:53:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8b578c68c33ad5ddf748ce7497de380f1903d441aee0c8b0b1af0471180e1`  
		Last Modified: Fri, 03 Sep 2021 02:04:43 GMT  
		Size: 5.1 MB (5132409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a57f2a02c7810a593cba16221fab32426c75881bc128a91ef728048538e53`  
		Last Modified: Fri, 03 Sep 2021 02:04:45 GMT  
		Size: 10.9 MB (10900458 bytes)  
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
$ docker pull buildpack-deps@sha256:bedca7b6c6375e09dd1ffb3eec3b607a8b8b9a15dd142b77525579bde87a41b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66588742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183f6c97e7e26c4086f4b6cb32c3908d6b090e56eab64119950c4a699dca29b0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:16:10 GMT
ADD file:22169a464bc792387d0c6cd4ca985b70527601306f274a47f7a26223b125d1b8 in / 
# Fri, 03 Sep 2021 01:16:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:59:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d209f64ed888c716b8fc1f768d766ccf831d8a034eb5e3ca12945873acb106f6`  
		Last Modified: Fri, 03 Sep 2021 01:32:35 GMT  
		Size: 51.3 MB (51289049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da873824fc3fcd77f59d7598fa94a4e0eef799c270584961cd61b0193ad259c`  
		Last Modified: Fri, 03 Sep 2021 02:39:12 GMT  
		Size: 5.0 MB (4986349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfba85c856d5ce39bea54898a8e2d95aa9c37df4c646386dfd0d1099c262561`  
		Last Modified: Fri, 03 Sep 2021 02:39:16 GMT  
		Size: 10.3 MB (10313344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:91057d86526bc5e96ff66eeb074c812f9321e33bef9d4b0ced773e1083ae997c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69717090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66bb7f34fb2e0b2a3dd65188ea09c38f4c42f4f90fe3d73d760f0816a9dde63b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:46:03 GMT
ADD file:4dec873e9e3022f644e228769ed26be34f63fb2d9b0ddc10816af8c9eaa11a15 in / 
# Fri, 03 Sep 2021 00:46:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:11:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:12:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2c1522cfd5f84804048a7cb823dfa679d77781943db2c6e71d872921d6d7542e`  
		Last Modified: Fri, 03 Sep 2021 00:54:32 GMT  
		Size: 53.8 MB (53772150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305bda156f1bbe0e441c40cfe1badc3590f18bfe3b1708ce8d2050c033c40ea2`  
		Last Modified: Fri, 03 Sep 2021 02:21:38 GMT  
		Size: 5.2 MB (5153859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac738bf714d2148f583c8c4ff6147a0840fc80305cf406c832bb05ad7eeaa9`  
		Last Modified: Fri, 03 Sep 2021 02:21:39 GMT  
		Size: 10.8 MB (10791081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:468dabbed82f94098143cae8671e5332569a713921a0df9d9983b603374d71b8
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
$ docker pull buildpack-deps@sha256:f4d652abef61df48e9ffc5b9cfa0ff60275c7ece073c683f3470789e1ee2eae4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122045084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce452975c108df26a1608befc48d7763e67342afecc2dc1030811fa8f36585aa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:53:41 GMT
ADD file:9d67c83a2e727f33502861325786047b9c6034b490854b93efb2d59cf973e5b6 in / 
# Fri, 03 Sep 2021 00:53:42 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:39:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:41:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c25501d6a46457c5895808abc531a7dcd2b4008bc42a432fcd73b6325c3fdacf`  
		Last Modified: Fri, 03 Sep 2021 01:10:41 GMT  
		Size: 53.0 MB (52980070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca497a6979f627d04639faa5571c98e112e1c56465986fce9d78c17101a5ce`  
		Last Modified: Fri, 03 Sep 2021 02:57:25 GMT  
		Size: 5.1 MB (5077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eab0927e6f1d00c87c3eed02237eb8b36a819bc0188dabfab4074f096423576`  
		Last Modified: Fri, 03 Sep 2021 02:57:28 GMT  
		Size: 10.6 MB (10595736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab42f59e6f95fa1040561c411658a005c01b13425791de2b04eb66b15d32f5a3`  
		Last Modified: Fri, 03 Sep 2021 02:58:18 GMT  
		Size: 53.4 MB (53391660 bytes)  
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
$ docker pull buildpack-deps@sha256:5e902fe3e8b8a92742d88713fae4924948e30a80da779cbbb73d5209c94f20d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.2 MB (130210303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a489eac282dc42cf470be83be408afb4620ba4535365f52b1c9a23b11639610a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:36 GMT
ADD file:64515d15f0b2fac0544e320a88716de6bf306c10f7e9400a945fca420a730843 in / 
# Fri, 03 Sep 2021 00:41:37 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:15:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:965ebee0ec76f6f76a0d14e40b7923292e9028532546ec1a748a8fed8267c897`  
		Last Modified: Fri, 03 Sep 2021 00:51:22 GMT  
		Size: 56.5 MB (56525268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56089068afb291eba965e50fb15a03f5ae7c433295ed8d952822fe54d1c1dd97`  
		Last Modified: Fri, 03 Sep 2021 01:22:57 GMT  
		Size: 5.3 MB (5303864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab52954bb9b6200d56553ce69fb7dae734a92c479ff8e38af69fa29a7d28110c`  
		Last Modified: Fri, 03 Sep 2021 01:22:58 GMT  
		Size: 11.3 MB (11270876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e266a96f5269409185770fdf13c62fab48d43de3f82cf97cb0f93890ae2b4a2`  
		Last Modified: Fri, 03 Sep 2021 01:23:25 GMT  
		Size: 57.1 MB (57110295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e7bbed7ac5659c6cd1aececdfaa4dc4744c5e258ee5c650a8ec37b539fda309b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124674074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f801a22581fced8c27b30a1378a19368e58a491bf7f4c84d59eb7a011e8343`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:53:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8b578c68c33ad5ddf748ce7497de380f1903d441aee0c8b0b1af0471180e1`  
		Last Modified: Fri, 03 Sep 2021 02:04:43 GMT  
		Size: 5.1 MB (5132409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a57f2a02c7810a593cba16221fab32426c75881bc128a91ef728048538e53`  
		Last Modified: Fri, 03 Sep 2021 02:04:45 GMT  
		Size: 10.9 MB (10900458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a709b007930a1acd8d8ea50132cb0b6a34e4f6f470c1b917f467d1263256229`  
		Last Modified: Fri, 03 Sep 2021 02:05:35 GMT  
		Size: 54.5 MB (54506202 bytes)  
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
$ docker pull buildpack-deps@sha256:75dacb3d7efa37c55a2ee04f476c40809377e9cbe9f4873bbb31898f271409e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118351561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0997c4f2769ed1634128d9554d1a4e7dd0308c463b797eeb1c5b77933109c777`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:16:10 GMT
ADD file:22169a464bc792387d0c6cd4ca985b70527601306f274a47f7a26223b125d1b8 in / 
# Fri, 03 Sep 2021 01:16:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:59:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d209f64ed888c716b8fc1f768d766ccf831d8a034eb5e3ca12945873acb106f6`  
		Last Modified: Fri, 03 Sep 2021 01:32:35 GMT  
		Size: 51.3 MB (51289049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da873824fc3fcd77f59d7598fa94a4e0eef799c270584961cd61b0193ad259c`  
		Last Modified: Fri, 03 Sep 2021 02:39:12 GMT  
		Size: 5.0 MB (4986349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfba85c856d5ce39bea54898a8e2d95aa9c37df4c646386dfd0d1099c262561`  
		Last Modified: Fri, 03 Sep 2021 02:39:16 GMT  
		Size: 10.3 MB (10313344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4008dd868e4d390b41b3510374a17a33a9fe636188767c8e61b168424fb1ec02`  
		Last Modified: Fri, 03 Sep 2021 02:41:24 GMT  
		Size: 51.8 MB (51762819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:75558dfed6e9f5fec05b1fdb390d686321ea9d9e006fbe11632fd936473b5cd9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124871121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4667324b850550595dc9a21fae5846f605d83d5551da54cc420b955bdffabc72`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:46:03 GMT
ADD file:4dec873e9e3022f644e228769ed26be34f63fb2d9b0ddc10816af8c9eaa11a15 in / 
# Fri, 03 Sep 2021 00:46:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:11:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:12:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c1522cfd5f84804048a7cb823dfa679d77781943db2c6e71d872921d6d7542e`  
		Last Modified: Fri, 03 Sep 2021 00:54:32 GMT  
		Size: 53.8 MB (53772150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305bda156f1bbe0e441c40cfe1badc3590f18bfe3b1708ce8d2050c033c40ea2`  
		Last Modified: Fri, 03 Sep 2021 02:21:38 GMT  
		Size: 5.2 MB (5153859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac738bf714d2148f583c8c4ff6147a0840fc80305cf406c832bb05ad7eeaa9`  
		Last Modified: Fri, 03 Sep 2021 02:21:39 GMT  
		Size: 10.8 MB (10791081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d4c39e7ec2e00b89fdc841a618fe0f405052037f5cfe5c1660d4c10ca31846`  
		Last Modified: Fri, 03 Sep 2021 02:21:56 GMT  
		Size: 55.2 MB (55154031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:xenial`

```console
$ docker pull buildpack-deps@sha256:bc56e6f62d4937f18fcd8ec8096bda57cbf9fad4d09cc85d81852e56cf85ca4e
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
$ docker pull buildpack-deps@sha256:415c4103ddc94a0ba15cfc220a261f43f8000d0e8f6c7af73ded0c66e63e3a1b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.4 MB (236392015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a479dc2c011ea4707ab6e48b150b1f6917474987bb4289c17178263b7320b3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:07:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:10:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42950b703a06b97a939a480237f84b19002bdea7a18b13134adc765328699d4d`  
		Last Modified: Tue, 31 Aug 2021 03:16:13 GMT  
		Size: 7.8 MB (7790543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2a7ae66eff85a2438aa0ea3586e8d8d638e66d1b32fe7d59a510cde54c2813`  
		Last Modified: Tue, 31 Aug 2021 03:16:30 GMT  
		Size: 41.9 MB (41905682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f044f40748825a2563b5545ec79398c53a46efb78ed955f6ef280afc9c0403`  
		Last Modified: Tue, 31 Aug 2021 03:16:58 GMT  
		Size: 140.2 MB (140196687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e8113cd72df13ee9ce4ad8efaf0c36e43c6f793f51ce9ad969612d42496f041f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202399881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de0787c69d4b4ca6b9a184d1f1fda5a4239c6913664adffed916ca9d38228288`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:25:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:28:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0c65fb267d23c5dd58ee3a818a8932a3fd565b8db9f6536fe98737a4e08f7`  
		Last Modified: Tue, 31 Aug 2021 03:44:48 GMT  
		Size: 6.6 MB (6631655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ffada20ea8521b2262a77a6239d4fc025f8f59d675a86c60923a075fb73d9d`  
		Last Modified: Tue, 31 Aug 2021 03:45:29 GMT  
		Size: 38.2 MB (38162364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d06b32826b0508bf1815ded75b8923a806d38c71670df7781d94612a6d5ea1`  
		Last Modified: Tue, 31 Aug 2021 03:46:52 GMT  
		Size: 117.3 MB (117292079 bytes)  
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
$ docker pull buildpack-deps@sha256:1a757e119c1ef3b09b0dc43addfebc79a914cc96960ecb404ab95db783caedcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.5 MB (245531585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9528843f5a733b688829d36c8fa4ada566f73da0c5fbc2085afdb9940fdac7d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:44:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:02:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c6ecbb79c70d45fca469278bf60d5e429f108594e71179f4a564aa3531b2d5`  
		Last Modified: Tue, 31 Aug 2021 05:34:20 GMT  
		Size: 7.7 MB (7693285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ba12653da3d4e66d89f4d0e6e7f60832cda0b7b78d6a428c517d0479e4b892`  
		Last Modified: Tue, 31 Aug 2021 05:36:50 GMT  
		Size: 45.1 MB (45147268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf88dce27d7ee92c7e90ace2790c859e6af24fcee1524c43ef37a50718cafa9`  
		Last Modified: Tue, 31 Aug 2021 05:39:27 GMT  
		Size: 145.2 MB (145167399 bytes)  
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
$ docker pull buildpack-deps@sha256:8f59fc3d592604d5cf14967c6283ad74901aa8627db618151ffcb0c09eef7438
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
$ docker pull buildpack-deps@sha256:144843b79263f8392a7a29101e618153b8648d20b3ae167eb6f71299266c968d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54289646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7cbab26ac13f5ebd5488c56aa11bf50c91677879ea96874af2cea8de4ac7cf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42950b703a06b97a939a480237f84b19002bdea7a18b13134adc765328699d4d`  
		Last Modified: Tue, 31 Aug 2021 03:16:13 GMT  
		Size: 7.8 MB (7790543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6b8a933b45c85d87d19be1ed2af4f23e53ad900e83ec143c92ec8447adecd2e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46945438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc60af10bb23d073d0363faaaddde45e0816b07e906287177ec75dcf1b38971`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:25:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0c65fb267d23c5dd58ee3a818a8932a3fd565b8db9f6536fe98737a4e08f7`  
		Last Modified: Tue, 31 Aug 2021 03:44:48 GMT  
		Size: 6.6 MB (6631655 bytes)  
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
$ docker pull buildpack-deps@sha256:1ae02049c2770ff1a92e180affdc536ce7756801970085ef122bbc4f2b2e1275
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55216918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a04612f213ecd554c79419d611c43be61dd722d99a45cebb6d945e93f9b9ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:44:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c6ecbb79c70d45fca469278bf60d5e429f108594e71179f4a564aa3531b2d5`  
		Last Modified: Tue, 31 Aug 2021 05:34:20 GMT  
		Size: 7.7 MB (7693285 bytes)  
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
$ docker pull buildpack-deps@sha256:c5af11486ef7c62ee6881e25b65486423adc05dcbd588bb1957c852da5e0e459
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
$ docker pull buildpack-deps@sha256:bdffd3de9058b91bf7ca86dc5d7b9e0028b9d0d894e630f23ef3c283e9e254b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.2 MB (96195328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433417de2a1ffff8b6c87633942faa9c8645ec88f7cb7a47c9a1d5f56b7e96dc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:07:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42950b703a06b97a939a480237f84b19002bdea7a18b13134adc765328699d4d`  
		Last Modified: Tue, 31 Aug 2021 03:16:13 GMT  
		Size: 7.8 MB (7790543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2a7ae66eff85a2438aa0ea3586e8d8d638e66d1b32fe7d59a510cde54c2813`  
		Last Modified: Tue, 31 Aug 2021 03:16:30 GMT  
		Size: 41.9 MB (41905682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ca27f899fcaf5240abf6e29d84601c0c2def08b179b0441443c49d7d14f1f7a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85107802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49140e977ceeba1edff0140500feec7c945c1838c132e0dc78f30e976313320`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:25:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0c65fb267d23c5dd58ee3a818a8932a3fd565b8db9f6536fe98737a4e08f7`  
		Last Modified: Tue, 31 Aug 2021 03:44:48 GMT  
		Size: 6.6 MB (6631655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ffada20ea8521b2262a77a6239d4fc025f8f59d675a86c60923a075fb73d9d`  
		Last Modified: Tue, 31 Aug 2021 03:45:29 GMT  
		Size: 38.2 MB (38162364 bytes)  
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
$ docker pull buildpack-deps@sha256:b14a5fb51b5d1ab5613940dea0f744f8a26a25e8961fea9dba6e27f06fb42984
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100364186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d669cab791289e0af0fcec78a739743372399e8bea4102312cd5ca1d5f4af1af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:44:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c6ecbb79c70d45fca469278bf60d5e429f108594e71179f4a564aa3531b2d5`  
		Last Modified: Tue, 31 Aug 2021 05:34:20 GMT  
		Size: 7.7 MB (7693285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ba12653da3d4e66d89f4d0e6e7f60832cda0b7b78d6a428c517d0479e4b892`  
		Last Modified: Tue, 31 Aug 2021 05:36:50 GMT  
		Size: 45.1 MB (45147268 bytes)  
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
