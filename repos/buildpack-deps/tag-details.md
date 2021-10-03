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
$ docker pull buildpack-deps@sha256:df4ae151dd3b2a262ac789bf17f72249659c5896b065e55a0ae78dd098dff04f
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
$ docker pull buildpack-deps@sha256:3c0807515e128baced0d30bb957832be1e298498ab4ae27e19a9790933a98442
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221261333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3fc72df6ea346e4d81aac88ec7ea1d73ce5a1b4c228bd00daffd981222f849`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:02:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:06:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1404df7fbdef68bea55f7c051dbdb1aac1e564886ca277d1f8b1d0bf3fbe8e4`  
		Last Modified: Fri, 01 Oct 2021 03:17:56 GMT  
		Size: 6.6 MB (6643379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964552afca366bca79302ab79366a0528db0710e3db41a0a5c40e90d1b936c20`  
		Last Modified: Fri, 01 Oct 2021 03:17:55 GMT  
		Size: 3.0 MB (3022502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f547fe5b8db9e7e53004a6ebd2656feef7a91d529f9cb21c95b3bc8b108e19`  
		Last Modified: Fri, 01 Oct 2021 03:18:13 GMT  
		Size: 45.5 MB (45477448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d3bc1c26143d890a32399b1baeb259de8bf2f6b5f65036e6dbaca6547f8f`  
		Last Modified: Fri, 01 Oct 2021 03:18:43 GMT  
		Size: 139.4 MB (139412929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:97c8663ef94b6784716e35962fff55cb99ee462056102e3cda9be49001f993c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189465194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db87044597f36141e8a2573b7ece145ddc2ad4d736a3e55c32e4066919746419`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:17:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:17:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:20:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0514bc47630e4346d13917c20c9a52eb361c5077c2b17f804d305bb3aeeae1ec`  
		Last Modified: Sat, 02 Oct 2021 22:36:02 GMT  
		Size: 5.7 MB (5713518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43197d564770c4e86c4ec1c0d141238ad2a175e92bebfa12b212b729f581ae62`  
		Last Modified: Sat, 02 Oct 2021 22:36:00 GMT  
		Size: 2.6 MB (2584549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd05568a3d4d96e48d84348793a6345f8359538aed1403669bef0db7a6f026c`  
		Last Modified: Sat, 02 Oct 2021 22:36:42 GMT  
		Size: 40.7 MB (40670724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908028762c0e5308de465f408ec635ee851602976ce9a8884e0b9c1c3372bf64`  
		Last Modified: Sat, 02 Oct 2021 22:38:05 GMT  
		Size: 118.2 MB (118192099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bb8ee9051e7d4b54ae564f9b794edcb3d43512f0da2f32ffa6fff0b346fcc4ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205821969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b433afcd80444e75da56050c2f2fb8a3fcac5258832102e7dde4be0707285e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:15:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:15:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:16:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ae8f73d2b97ae6f304518bd244cd1e218386861b11878333a3e1704cd06fc4`  
		Last Modified: Fri, 01 Oct 2021 03:24:20 GMT  
		Size: 6.1 MB (6085031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc43f166dad077ef896c5d7e305f3a19ff7f4c0245159dede3adee91cf2fb17`  
		Last Modified: Fri, 01 Oct 2021 03:24:19 GMT  
		Size: 2.8 MB (2783140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a133bda1a844b0b9e9ac0284af4779d5ec158f5693b56511a1f27a5cbc8f541`  
		Last Modified: Fri, 01 Oct 2021 03:24:38 GMT  
		Size: 43.3 MB (43269968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba35ad1221e5859d39cb2b5e83e0f09f32a679b01ad0cf9bd7d43f755fce8ca`  
		Last Modified: Fri, 01 Oct 2021 03:25:08 GMT  
		Size: 130.0 MB (129956354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9f10a9ee18f6be60bfe5500c424c0125ad8e8b34ef076b08278d9a12cf826537
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.6 MB (218560267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419b39771048169c84a707f522a0987ffe42bf3349a0ab49e3abac9277252716`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:14:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 04:15:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:18:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89515178f4a354382498077df201d0c7296621351f651bf1d7bda94f1d499466`  
		Last Modified: Fri, 01 Oct 2021 04:21:07 GMT  
		Size: 6.9 MB (6932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99224216777e769a2c151c0c091ec4cda2a5d5f541c203e203683c71b6cb4a9f`  
		Last Modified: Fri, 01 Oct 2021 04:21:06 GMT  
		Size: 3.3 MB (3252987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8565053f61bc235064ba9f6560e2464bd101da6ba901ae2152a5198bac7f4e3`  
		Last Modified: Fri, 01 Oct 2021 04:21:29 GMT  
		Size: 47.1 MB (47065713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0502655b09b53ef4e834ca20300b20d019082bfbe8caad5e33e24676ce7aa8`  
		Last Modified: Fri, 01 Oct 2021 04:22:13 GMT  
		Size: 134.2 MB (134150425 bytes)  
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
$ docker pull buildpack-deps@sha256:5936655630734b659a06da22719a5788844863d57670778cb9d6bc1f79007ddb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.6 MB (205618219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ec7d1aadb3df4675c40b4a20c77c55defab1ae414d0cc9570efce58c897ac6a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:33:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:33:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f1e9a656ce747f09402ff405b881ebbce2041d0228e2373aac2dbfe9a23fd8`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 6.3 MB (6334289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe96b416a4fa4b5de3ab17b5e2b2b85bde2482559e7592284278d282da0c067`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 3.0 MB (2974970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6a10244fc86eb56eba2d1e8554fe9b23b582e56b7728fcb21fee59a9313d52`  
		Last Modified: Fri, 01 Oct 2021 02:41:34 GMT  
		Size: 45.0 MB (45016989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8108fe4f05569dd68d228c1be27552ed405fc79994a5cb6f78b8c142ff1ed6da`  
		Last Modified: Fri, 01 Oct 2021 02:41:57 GMT  
		Size: 125.9 MB (125929053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-curl`

```console
$ docker pull buildpack-deps@sha256:5325fe2efe7693bcef1ab64f89cfc05be2520bd07181e6671aef7eaac3e251d8
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
$ docker pull buildpack-deps@sha256:64e7d3f7a80ed2f1f95becd49baec3998ce6eb2c56d783ac2d1fc2fb85c6dc73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36370956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6fda0143b32371ab8b25a7e99a8957c2fe2207f5bd81e75e06bd1def8efa61f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:02:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1404df7fbdef68bea55f7c051dbdb1aac1e564886ca277d1f8b1d0bf3fbe8e4`  
		Last Modified: Fri, 01 Oct 2021 03:17:56 GMT  
		Size: 6.6 MB (6643379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964552afca366bca79302ab79366a0528db0710e3db41a0a5c40e90d1b936c20`  
		Last Modified: Fri, 01 Oct 2021 03:17:55 GMT  
		Size: 3.0 MB (3022502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3a63e143a2e16370a02a00761f4a94d18cb53969185afd48c00b69ad5d1909cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30602371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c8095f1395eb522f1177e72c5b745d6332913041081bbcc6a66c718a6179830`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:17:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:17:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0514bc47630e4346d13917c20c9a52eb361c5077c2b17f804d305bb3aeeae1ec`  
		Last Modified: Sat, 02 Oct 2021 22:36:02 GMT  
		Size: 5.7 MB (5713518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43197d564770c4e86c4ec1c0d141238ad2a175e92bebfa12b212b729f581ae62`  
		Last Modified: Sat, 02 Oct 2021 22:36:00 GMT  
		Size: 2.6 MB (2584549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:39ab1f63e4c0b3e09586c549569cabdb152a84d2506e7a763bb7073c51e17f49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32595647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5ce59175e5046b186b7c888fe1322f90eadd0eb2dbf8c78060b2bf4db8ab99b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:15:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:15:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ae8f73d2b97ae6f304518bd244cd1e218386861b11878333a3e1704cd06fc4`  
		Last Modified: Fri, 01 Oct 2021 03:24:20 GMT  
		Size: 6.1 MB (6085031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc43f166dad077ef896c5d7e305f3a19ff7f4c0245159dede3adee91cf2fb17`  
		Last Modified: Fri, 01 Oct 2021 03:24:19 GMT  
		Size: 2.8 MB (2783140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b6b5a071215a2d0e46fc410080e7957427beb8fb6444a95686284df0b0c2720d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37344129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2455fd5918f65a81c70a107effdaedc75df1f1ca4349cbc2e8051c0378cecf5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:14:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89515178f4a354382498077df201d0c7296621351f651bf1d7bda94f1d499466`  
		Last Modified: Fri, 01 Oct 2021 04:21:07 GMT  
		Size: 6.9 MB (6932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99224216777e769a2c151c0c091ec4cda2a5d5f541c203e203683c71b6cb4a9f`  
		Last Modified: Fri, 01 Oct 2021 04:21:06 GMT  
		Size: 3.3 MB (3252987 bytes)  
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
$ docker pull buildpack-deps@sha256:558995a4b832c433e78e0ac738c121aa35235fda0b38e00def4386e6a5d4676b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34672177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799be440f53410fdee2a74a842e6b7b7586547315f6a0aba25e8a343ff7e0fa5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:33:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f1e9a656ce747f09402ff405b881ebbce2041d0228e2373aac2dbfe9a23fd8`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 6.3 MB (6334289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe96b416a4fa4b5de3ab17b5e2b2b85bde2482559e7592284278d282da0c067`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 3.0 MB (2974970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-scm`

```console
$ docker pull buildpack-deps@sha256:4f0ee684a0e55ac502f98fdddd5138eabb1b95a33f6f2c7267484bfb35f3c46d
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
$ docker pull buildpack-deps@sha256:5e43b1ebcfe2b76e7912db780b8aac130c8578f962609f04f88de0e5abbb150c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81848404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2ce214211225c549bf9107a4c081cc04753411e5f7dc05e2fe18e780cb6807`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:02:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1404df7fbdef68bea55f7c051dbdb1aac1e564886ca277d1f8b1d0bf3fbe8e4`  
		Last Modified: Fri, 01 Oct 2021 03:17:56 GMT  
		Size: 6.6 MB (6643379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964552afca366bca79302ab79366a0528db0710e3db41a0a5c40e90d1b936c20`  
		Last Modified: Fri, 01 Oct 2021 03:17:55 GMT  
		Size: 3.0 MB (3022502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f547fe5b8db9e7e53004a6ebd2656feef7a91d529f9cb21c95b3bc8b108e19`  
		Last Modified: Fri, 01 Oct 2021 03:18:13 GMT  
		Size: 45.5 MB (45477448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:58947866db3f48fa361f7056b87a69b67ef6f4b3348e65f297ab297295dca8ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71273095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa26238d728f2e54ac4d6d4703e94f9750fa80cebe834eccf807a708e56ddd4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:17:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:17:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0514bc47630e4346d13917c20c9a52eb361c5077c2b17f804d305bb3aeeae1ec`  
		Last Modified: Sat, 02 Oct 2021 22:36:02 GMT  
		Size: 5.7 MB (5713518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43197d564770c4e86c4ec1c0d141238ad2a175e92bebfa12b212b729f581ae62`  
		Last Modified: Sat, 02 Oct 2021 22:36:00 GMT  
		Size: 2.6 MB (2584549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd05568a3d4d96e48d84348793a6345f8359538aed1403669bef0db7a6f026c`  
		Last Modified: Sat, 02 Oct 2021 22:36:42 GMT  
		Size: 40.7 MB (40670724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5da94e3b4e1ce6cd029b385bdd46bc85fdbd02dab217b66dd410c26f393fc219
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75865615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04215758cdb2f31d14432063ca393004a2b774b824c660ab4bd5870b9ae8d919`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:15:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:15:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ae8f73d2b97ae6f304518bd244cd1e218386861b11878333a3e1704cd06fc4`  
		Last Modified: Fri, 01 Oct 2021 03:24:20 GMT  
		Size: 6.1 MB (6085031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc43f166dad077ef896c5d7e305f3a19ff7f4c0245159dede3adee91cf2fb17`  
		Last Modified: Fri, 01 Oct 2021 03:24:19 GMT  
		Size: 2.8 MB (2783140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a133bda1a844b0b9e9ac0284af4779d5ec158f5693b56511a1f27a5cbc8f541`  
		Last Modified: Fri, 01 Oct 2021 03:24:38 GMT  
		Size: 43.3 MB (43269968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d9cab10f9ba15a4bf0183c6ef9ba2228cef5dcd289d8375067b643f7871634a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84409842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41a8d31955cc503b31fb1a846ae9d7a4ab19e619b95a661d1827f73e0e3ed711`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:14:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 04:15:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89515178f4a354382498077df201d0c7296621351f651bf1d7bda94f1d499466`  
		Last Modified: Fri, 01 Oct 2021 04:21:07 GMT  
		Size: 6.9 MB (6932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99224216777e769a2c151c0c091ec4cda2a5d5f541c203e203683c71b6cb4a9f`  
		Last Modified: Fri, 01 Oct 2021 04:21:06 GMT  
		Size: 3.3 MB (3252987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8565053f61bc235064ba9f6560e2464bd101da6ba901ae2152a5198bac7f4e3`  
		Last Modified: Fri, 01 Oct 2021 04:21:29 GMT  
		Size: 47.1 MB (47065713 bytes)  
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
$ docker pull buildpack-deps@sha256:4e8170c2f8d92780b4d06eb93b8653189f5ce8da2287d75ae8e6d231d825bdaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79689166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ca7a0f2efa94efec7d8ce8eb0e04a949e4acdb537896a432f28ecc1c1e1232`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:33:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:33:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f1e9a656ce747f09402ff405b881ebbce2041d0228e2373aac2dbfe9a23fd8`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 6.3 MB (6334289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe96b416a4fa4b5de3ab17b5e2b2b85bde2482559e7592284278d282da0c067`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 3.0 MB (2974970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6a10244fc86eb56eba2d1e8554fe9b23b582e56b7728fcb21fee59a9313d52`  
		Last Modified: Fri, 01 Oct 2021 02:41:34 GMT  
		Size: 45.0 MB (45016989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:aede609912cf5648b0bf72f5e266a0ac6ce81e358ef51330832e33d3ef3806f6
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
$ docker pull buildpack-deps@sha256:fbb84e6535f83fd99ac792ae04a5951548a06772d975566a58cbf2d4b5aa3a23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241790873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dd92b1441e82e0931e46cb77542405e6fa9fc22ef0ad2431f5eab57e3d2f1f8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:06:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:07:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:10:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4774ed347ee7aae0f4029cf9fcdc82fb078d2849f5379c2b3cd0d78fac5608ef`  
		Last Modified: Fri, 01 Oct 2021 03:18:54 GMT  
		Size: 7.8 MB (7770752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f807ec5dd5b51b82a425eb00c21aff5367e6944b5d689b16480bb86b55eeba`  
		Last Modified: Fri, 01 Oct 2021 03:18:53 GMT  
		Size: 3.6 MB (3624639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250b71bd9a093349f8995026b169a3c6ac13ec9deca245d216b4293d68de144`  
		Last Modified: Fri, 01 Oct 2021 03:19:13 GMT  
		Size: 60.7 MB (60718964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6324cfcaab7eb21672073d745766ea088056ec005d6cbf1a733f7ec3aa1c0f5b`  
		Last Modified: Fri, 01 Oct 2021 03:19:43 GMT  
		Size: 141.1 MB (141107604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9234b134ea076c6574d39c3dbe0cde67242fdf2417245afea087c5ef706babb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207217146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2311fdf25f2e903d826aaaa6846da6841c4d1a7b341f5886f8272a1b89ecae8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:20:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:21:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:22:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:23:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ab467c7f452a8e5cb76b5ed3c9cbce43f7cb04f7024c6478ca446f92e399b`  
		Last Modified: Sat, 02 Oct 2021 22:38:21 GMT  
		Size: 6.8 MB (6766828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d36dec707683a0afbc780af0a45ca17744ac7a0f640d578af3195478d90621`  
		Last Modified: Sat, 02 Oct 2021 22:38:18 GMT  
		Size: 3.1 MB (3103932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035a89a55aa2f31698e17865b0d77f83527531ba06367f3a102622156308cc19`  
		Last Modified: Sat, 02 Oct 2021 22:39:13 GMT  
		Size: 55.5 MB (55450855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318206d0235667fb1d2d144a55607944970fa31e7dd0505f9181f42585c87653`  
		Last Modified: Sat, 02 Oct 2021 22:40:36 GMT  
		Size: 117.8 MB (117828313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e90ebfc849475dadd4dbdb12bd6fb07dff77c72547c4dd3135d681b3e302ca04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231928586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b447be8ba7595e18d9b365577069b4e6a6b472eb3e1dfd9dfb2e86f0d35eb5b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:17:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:17:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:18:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689db6ff62963b3e4aae6a2abb554c5d5882b06774174e624ba845094921121b`  
		Last Modified: Fri, 01 Oct 2021 03:25:21 GMT  
		Size: 7.6 MB (7635218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f06ec2d3b194d9726a65c75b82d7339dc700bc20d923f047e02a735a78925`  
		Last Modified: Fri, 01 Oct 2021 03:25:20 GMT  
		Size: 3.6 MB (3600459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab6b6364c13aa6082dc2050a10d5035c25a02706281100e29c0ad568f624b29`  
		Last Modified: Fri, 01 Oct 2021 03:25:43 GMT  
		Size: 60.8 MB (60767677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299cf52c5a3ea41921e5ca4a9a5f00842be4e17c0767d58216a6bcf50d8fa4b5`  
		Last Modified: Fri, 01 Oct 2021 03:26:15 GMT  
		Size: 132.8 MB (132752827 bytes)  
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
$ docker pull buildpack-deps@sha256:80597b385ccb4649fffd750d5dba51880eff9b05435f128142afa465727f9b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222631286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3dbdfb7bb408340ec0b5b0ac6676da0dd3c7139f8422c9992e4ce3aaeb762c3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:34:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:35:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:35:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6fa25b21a93cb1d9a61a6d35cabe2d161b63a3706869aeb57c0df4be4472b4`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 7.4 MB (7427440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a836aa79819738132b60bb1aa2d42907d593dc879d3785ca6afff3f6adda654`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 3.5 MB (3542126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651550a9a41cdd82a572e95f64a221b84cd8e9d72e164544f480714afe537054`  
		Last Modified: Fri, 01 Oct 2021 02:42:21 GMT  
		Size: 60.0 MB (60020560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2ff4661bb90141a8840a1627abe3deede20a3beadc896129a3764974793aa7`  
		Last Modified: Fri, 01 Oct 2021 02:42:44 GMT  
		Size: 124.5 MB (124518250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:4a9add1dae34360ec3f686c6f822a907a5b6490a998fe1d9b297cda065cf3db0
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
$ docker pull buildpack-deps@sha256:696b974b81ccbecfc40803f879228a8259edc1c8b5c098ccefdd1f35437bcfe1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39964305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357a312644cce18c08e5ce216006fa4089442dec9b94fd3c5f84a01df0d9c747`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:06:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4774ed347ee7aae0f4029cf9fcdc82fb078d2849f5379c2b3cd0d78fac5608ef`  
		Last Modified: Fri, 01 Oct 2021 03:18:54 GMT  
		Size: 7.8 MB (7770752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f807ec5dd5b51b82a425eb00c21aff5367e6944b5d689b16480bb86b55eeba`  
		Last Modified: Fri, 01 Oct 2021 03:18:53 GMT  
		Size: 3.6 MB (3624639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:96fc46fd8428121f4cba8731f07c3d2b0477826da21811e89ba2facff69b90c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a44a4a803282848534fb0e2b5a618208d8f0fcfaa6918c8c5021e765bc45ea6c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:20:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:21:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ab467c7f452a8e5cb76b5ed3c9cbce43f7cb04f7024c6478ca446f92e399b`  
		Last Modified: Sat, 02 Oct 2021 22:38:21 GMT  
		Size: 6.8 MB (6766828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d36dec707683a0afbc780af0a45ca17744ac7a0f640d578af3195478d90621`  
		Last Modified: Sat, 02 Oct 2021 22:38:18 GMT  
		Size: 3.1 MB (3103932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2fb36e233ead75cc8b3a9e8a7feaa46b31ce507f9666246b82975f177db2bb7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38408082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da02243d8b4488513cd7351f2ebc075c8db8b4098ee398a79e228a8f2a72b20f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:17:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689db6ff62963b3e4aae6a2abb554c5d5882b06774174e624ba845094921121b`  
		Last Modified: Fri, 01 Oct 2021 03:25:21 GMT  
		Size: 7.6 MB (7635218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f06ec2d3b194d9726a65c75b82d7339dc700bc20d923f047e02a735a78925`  
		Last Modified: Fri, 01 Oct 2021 03:25:20 GMT  
		Size: 3.6 MB (3600459 bytes)  
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
$ docker pull buildpack-deps@sha256:6fc23eff56764bfacf3643338fbed63a7b9a96aa22a7cb7da40e7c2388ca1d73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34119703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3afa654267fc7f48a4a8c50432c7addb0a16401799d27cfab2b9743babcdd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:14:48 GMT
ADD file:a8b9aeb23e8f47568ef8ea33a80fee0c676db7c4c9ec9210abf75217a8f329fb in / 
# Fri, 01 Oct 2021 01:14:49 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:08:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:91a226dd2b609e6bc3e70f7621380def71f05b74e75fa1a2f0421795a8904f10`  
		Last Modified: Fri, 01 Oct 2021 01:37:38 GMT  
		Size: 24.2 MB (24227267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9183300d5640e2467c23128b3e3557a975761a04b458b806535ec6ce8e89ae2f`  
		Last Modified: Fri, 01 Oct 2021 02:49:29 GMT  
		Size: 6.7 MB (6747990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e44b67d1b1ccde3826142f95cdc6cd6e379bbfbeda24c6253df084db75344f`  
		Last Modified: Fri, 01 Oct 2021 02:49:24 GMT  
		Size: 3.1 MB (3144446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b9766200c0f8abda5cc5c3085a6a3c22fb41ee8132e5ead08fa6542aa15e148c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38092476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97ee38d1e83342696caace4f46cf69a402659c84d853a06591a6f59a5503d96`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:34:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6fa25b21a93cb1d9a61a6d35cabe2d161b63a3706869aeb57c0df4be4472b4`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 7.4 MB (7427440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a836aa79819738132b60bb1aa2d42907d593dc879d3785ca6afff3f6adda654`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 3.5 MB (3542126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:4465794cf302f98968f6b677b0a61c97abe78aa1f75135e493c6b614690f6192
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
$ docker pull buildpack-deps@sha256:7ad91f5bc79abd012aa84bf3ae64f626eb7eeb8e711e57f9bd2f163d2eac7de6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100683269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5457e36bff271ad9896846715e324a195c4083d4749034159d0029d47252df`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:06:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:07:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4774ed347ee7aae0f4029cf9fcdc82fb078d2849f5379c2b3cd0d78fac5608ef`  
		Last Modified: Fri, 01 Oct 2021 03:18:54 GMT  
		Size: 7.8 MB (7770752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f807ec5dd5b51b82a425eb00c21aff5367e6944b5d689b16480bb86b55eeba`  
		Last Modified: Fri, 01 Oct 2021 03:18:53 GMT  
		Size: 3.6 MB (3624639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250b71bd9a093349f8995026b169a3c6ac13ec9deca245d216b4293d68de144`  
		Last Modified: Fri, 01 Oct 2021 03:19:13 GMT  
		Size: 60.7 MB (60718964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3a61d944bb68e7c20853916e0ebf65b59600c6691ad38bc20026e8860da4a59c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89388833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768431def83a292eefc32a7aebb536b9aacdd6fb88a516d63ef547131dddadef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:20:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:21:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:22:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ab467c7f452a8e5cb76b5ed3c9cbce43f7cb04f7024c6478ca446f92e399b`  
		Last Modified: Sat, 02 Oct 2021 22:38:21 GMT  
		Size: 6.8 MB (6766828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d36dec707683a0afbc780af0a45ca17744ac7a0f640d578af3195478d90621`  
		Last Modified: Sat, 02 Oct 2021 22:38:18 GMT  
		Size: 3.1 MB (3103932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035a89a55aa2f31698e17865b0d77f83527531ba06367f3a102622156308cc19`  
		Last Modified: Sat, 02 Oct 2021 22:39:13 GMT  
		Size: 55.5 MB (55450855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:696e75f38cfed35972c462e702a6009c506e6e349401bf8287ab1c1a75bc00a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99175759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3c038017047e55e8000b4e31fac47994fdb7740f8bd392338795912c12ca9f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:17:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:17:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689db6ff62963b3e4aae6a2abb554c5d5882b06774174e624ba845094921121b`  
		Last Modified: Fri, 01 Oct 2021 03:25:21 GMT  
		Size: 7.6 MB (7635218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f06ec2d3b194d9726a65c75b82d7339dc700bc20d923f047e02a735a78925`  
		Last Modified: Fri, 01 Oct 2021 03:25:20 GMT  
		Size: 3.6 MB (3600459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab6b6364c13aa6082dc2050a10d5035c25a02706281100e29c0ad568f624b29`  
		Last Modified: Fri, 01 Oct 2021 03:25:43 GMT  
		Size: 60.8 MB (60767677 bytes)  
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
$ docker pull buildpack-deps@sha256:ab12db445536d99cc55a13c70085c271777f232dfbd09ac2056e5c0c7d30350a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98113036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:403e51f1da78f84c9ef754ad1f475ec1078f576d75597b0aa4b8edb22af9801d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:34:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:35:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6fa25b21a93cb1d9a61a6d35cabe2d161b63a3706869aeb57c0df4be4472b4`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 7.4 MB (7427440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a836aa79819738132b60bb1aa2d42907d593dc879d3785ca6afff3f6adda654`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 3.5 MB (3542126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651550a9a41cdd82a572e95f64a221b84cd8e9d72e164544f480714afe537054`  
		Last Modified: Fri, 01 Oct 2021 02:42:21 GMT  
		Size: 60.0 MB (60020560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.04`

```console
$ docker pull buildpack-deps@sha256:b7fce989935172004b910ccbe7a55549cfa21057baac705dfdaa5765933768a7
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
$ docker pull buildpack-deps@sha256:d0b1bc965e6285f5b580fed802c86c2609554e159bce1fbc68420f19c6e8bbc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248825494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab7ad9ebdf1c606e7a98f7ceb37be67b63bb2979f28a43c567471357f6c0479b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:12:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:12:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e61e03c60557bda70bf3cc9a2dd5562bdd9f66442dd9a5b33f393f7f610ca9`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 5.4 MB (5429421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1701598239c3ba301af98cdbdc4c053cff70425e0102d03a0a0a660b68520b35`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 3.7 MB (3662530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bdc834e59f4ded456cfe6c6f10cc62573219101f62812b9e6aa4fcb1724d6d`  
		Last Modified: Fri, 01 Oct 2021 03:20:11 GMT  
		Size: 43.5 MB (43542401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8935876bd7c602a9726de718b80206366568ebdb6230210377b10bf2a0e35d0b`  
		Last Modified: Fri, 01 Oct 2021 03:20:44 GMT  
		Size: 164.5 MB (164486846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6750601f1fd76063f80245bfe8db26d1a96853abfc6dfb02fb16188a458ea329
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.0 MB (208963298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fe4c7546b306b1c82069e56220df647071c462704250c3ea210b3f3e657061`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:24:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:25:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:27:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8944eff0f4815cf5a70868ad5afaed083de9f7ead5a73bc97fa5dc147a04f9`  
		Last Modified: Sat, 02 Oct 2021 22:40:51 GMT  
		Size: 4.9 MB (4858463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bed8cb9d9d7259532d0d30040f4f46ba30d3dedae6e7d37d51c4bf9f60bc54a`  
		Last Modified: Sat, 02 Oct 2021 22:40:50 GMT  
		Size: 3.1 MB (3139002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8efec2f84a292f59a270ac67ccb130692e15a90a3105f135600dd1ee32bed4`  
		Last Modified: Sat, 02 Oct 2021 22:41:32 GMT  
		Size: 40.0 MB (39953431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfb48b1577ca4abe64edeb74c9898c20c84b004d5bc4a66957c2de97d6af5f`  
		Last Modified: Sat, 02 Oct 2021 22:43:03 GMT  
		Size: 134.2 MB (134152915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b3cfe5018bd7d3a98817ee81a7622ca088182ce526cda8e1ca95f94d12185024
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239588979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f87ff4d2d7f7f612af485bab800828d06486c37417992be439eee282e9a06d4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:18:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:18:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:19:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:19:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22e5e9de7272c5e4544f153bf2aeeb8c118ac5a3ccdea10a7d6a6c996c3575c`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 5.4 MB (5400844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c320e18b5848a613875caa1714ab609c4840c23b41f7eb20a8d3dc34193f53d`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 3.6 MB (3638468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47cb72d2d39bf513d49bbb200478599434e3db9569aef12f56685039732f370`  
		Last Modified: Fri, 01 Oct 2021 03:26:46 GMT  
		Size: 43.5 MB (43526154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78e0bd1f0df4b31c75564b204eafde9e2ed9270dfa01bc2ddb56f50bfef7e3c`  
		Last Modified: Fri, 01 Oct 2021 03:27:21 GMT  
		Size: 156.8 MB (156849350 bytes)  
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
$ docker pull buildpack-deps@sha256:a445bb89dc4ad3e2a546446073c778792b1cf88762d78ac04fd3a8fd9286c6a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.9 MB (257925643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f10e0dd936c1a9ddadab2ba100ffe9ed2f196a160e87e4f254b27baf58e8c693`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:10:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:11:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:20:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747535e5ca63ea5be385acb70aaca4311fe2b78f1e44463cbfce298800f9f33b`  
		Last Modified: Fri, 01 Oct 2021 02:50:40 GMT  
		Size: 4.9 MB (4944581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0facf6815c035133c1d22c89659eabcd14838fa24ff638d7a2f822c2d42d795a`  
		Last Modified: Fri, 01 Oct 2021 02:50:37 GMT  
		Size: 3.2 MB (3177915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f4c1d69caf6add02d4549d216e9e00fdaae087f4d280cea93bbd3f8b3ec48a`  
		Last Modified: Fri, 01 Oct 2021 02:52:36 GMT  
		Size: 40.3 MB (40329415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4eb085d1eb115177f17b87572f40735eff638aa6135e73b357a2e48048b803`  
		Last Modified: Fri, 01 Oct 2021 02:58:07 GMT  
		Size: 182.3 MB (182331851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f27299270693081b87ff3db0f81ca0b487eadf97ab498fd4138daa4bf57b8540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241445352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1baf0cfdef466aacd2bc2dbb6e3ac9fc116c3f801fa511931eab79565035b41`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:36:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:36:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:37:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a99a5951692580021e948472804dab0a010b074b1163b603e4f5cfda6382bf4`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 5.8 MB (5801664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fa544ba88c98b23feadb6ad914d8da1debe080907cb082ad2b8d8046e6c5da`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 4.2 MB (4185318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f556cc2020b283f43fb541b48641c7dd9e20e8d7d40de1a098420d28dbe5b70d`  
		Last Modified: Fri, 01 Oct 2021 02:43:07 GMT  
		Size: 47.4 MB (47399802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b33a1445de22d945dee33648fd8863fb8b89b557a88fdde39b8d2f87fbde44`  
		Last Modified: Fri, 01 Oct 2021 02:43:33 GMT  
		Size: 151.6 MB (151553029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.04-curl`

```console
$ docker pull buildpack-deps@sha256:d9f00aea588cf3f87f60a3ce0c9e17dbb4a13580ef6b7509135dce7072ee15af
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
$ docker pull buildpack-deps@sha256:9061f7ef082ae113348351460f7c072b43192180e25e675fbde68bebab046851
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40796247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e96cc49ca9401fa96ae12c1ffb5e5c840591f3a502977d7bc750b9223e3a4d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:12:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e61e03c60557bda70bf3cc9a2dd5562bdd9f66442dd9a5b33f393f7f610ca9`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 5.4 MB (5429421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1701598239c3ba301af98cdbdc4c053cff70425e0102d03a0a0a660b68520b35`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 3.7 MB (3662530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2d230394b683fdf5e3e856d2c6d7b0c95ab49ce823d7a6c8cf63be67907666a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34856952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe84b73356152b7afd8fc8c78dd430cbfa28f4a3eb076c34c16c26d3579a2c8c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:24:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8944eff0f4815cf5a70868ad5afaed083de9f7ead5a73bc97fa5dc147a04f9`  
		Last Modified: Sat, 02 Oct 2021 22:40:51 GMT  
		Size: 4.9 MB (4858463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bed8cb9d9d7259532d0d30040f4f46ba30d3dedae6e7d37d51c4bf9f60bc54a`  
		Last Modified: Sat, 02 Oct 2021 22:40:50 GMT  
		Size: 3.1 MB (3139002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e97fb51e07261b6a8213a306321408eaab25c98dd81802fa5c3466d01585e297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39213475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea936eb6321870111adf4892e07b9dd6a92b42c9be055e57c581219867d1d64`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:18:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:18:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22e5e9de7272c5e4544f153bf2aeeb8c118ac5a3ccdea10a7d6a6c996c3575c`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 5.4 MB (5400844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c320e18b5848a613875caa1714ab609c4840c23b41f7eb20a8d3dc34193f53d`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 3.6 MB (3638468 bytes)  
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
$ docker pull buildpack-deps@sha256:6f18fc0d3ddcc7a1fc4421df4e73d1bc7c8bfa9bcb096d4d55eef355576c40bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35264377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01fdd529f701fb77c03d0bbb3433871ae8b6285adebd0a80f552a4b1421c913`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:10:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:11:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747535e5ca63ea5be385acb70aaca4311fe2b78f1e44463cbfce298800f9f33b`  
		Last Modified: Fri, 01 Oct 2021 02:50:40 GMT  
		Size: 4.9 MB (4944581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0facf6815c035133c1d22c89659eabcd14838fa24ff638d7a2f822c2d42d795a`  
		Last Modified: Fri, 01 Oct 2021 02:50:37 GMT  
		Size: 3.2 MB (3177915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d4fb0f8ba2a1371a25956f327c4583b4177f6a08669243e2cc644487ef42db54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42492521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769764cfa8002921bd1badc5e585535ccf1ce621970e3950a8757da9733976e3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:36:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:36:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a99a5951692580021e948472804dab0a010b074b1163b603e4f5cfda6382bf4`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 5.8 MB (5801664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fa544ba88c98b23feadb6ad914d8da1debe080907cb082ad2b8d8046e6c5da`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 4.2 MB (4185318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.04-scm`

```console
$ docker pull buildpack-deps@sha256:540342c46d76db22368d7efc404214fac6390ffd4fd3971b2be2b498a251e3bf
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
$ docker pull buildpack-deps@sha256:e4b34d9ecd5c159571e7c4aa5a92e5f59021eae78e6b03e1619fad1216f46a17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.3 MB (84338648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a3cb2eb560e049b85cb7c014a687b3aae9ce86dadd0640b986879a2d7f70cf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:12:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:12:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e61e03c60557bda70bf3cc9a2dd5562bdd9f66442dd9a5b33f393f7f610ca9`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 5.4 MB (5429421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1701598239c3ba301af98cdbdc4c053cff70425e0102d03a0a0a660b68520b35`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 3.7 MB (3662530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bdc834e59f4ded456cfe6c6f10cc62573219101f62812b9e6aa4fcb1724d6d`  
		Last Modified: Fri, 01 Oct 2021 03:20:11 GMT  
		Size: 43.5 MB (43542401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9804a4fd9b159a2bf14e2e9fecfafd454b98c57b208e9f1cd046c5367321421e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74810383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa57e9ca19a6490459f1d1b27fc9522ba5af6d70e5bf5de22e6d43365e578599`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:24:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:25:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8944eff0f4815cf5a70868ad5afaed083de9f7ead5a73bc97fa5dc147a04f9`  
		Last Modified: Sat, 02 Oct 2021 22:40:51 GMT  
		Size: 4.9 MB (4858463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bed8cb9d9d7259532d0d30040f4f46ba30d3dedae6e7d37d51c4bf9f60bc54a`  
		Last Modified: Sat, 02 Oct 2021 22:40:50 GMT  
		Size: 3.1 MB (3139002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8efec2f84a292f59a270ac67ccb130692e15a90a3105f135600dd1ee32bed4`  
		Last Modified: Sat, 02 Oct 2021 22:41:32 GMT  
		Size: 40.0 MB (39953431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d9446fb751659cac97fe4602a547a07c488b2e551c439846879acfe1d17fd7f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82739629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c6cb7af054be1655c285f42e5dc616e5c700b2145d26cfab1540f6fcf5034dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:18:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:18:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:19:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22e5e9de7272c5e4544f153bf2aeeb8c118ac5a3ccdea10a7d6a6c996c3575c`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 5.4 MB (5400844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c320e18b5848a613875caa1714ab609c4840c23b41f7eb20a8d3dc34193f53d`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 3.6 MB (3638468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47cb72d2d39bf513d49bbb200478599434e3db9569aef12f56685039732f370`  
		Last Modified: Fri, 01 Oct 2021 03:26:46 GMT  
		Size: 43.5 MB (43526154 bytes)  
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
$ docker pull buildpack-deps@sha256:f65fa8029821604824f633737c48c72f705393e217b105f05b5b0666541fe3d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75593792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b647358b6ce20b1f16ee3cba013956f23773270e2ad5c14a3acf32d1f3d7f1b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:10:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:11:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747535e5ca63ea5be385acb70aaca4311fe2b78f1e44463cbfce298800f9f33b`  
		Last Modified: Fri, 01 Oct 2021 02:50:40 GMT  
		Size: 4.9 MB (4944581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0facf6815c035133c1d22c89659eabcd14838fa24ff638d7a2f822c2d42d795a`  
		Last Modified: Fri, 01 Oct 2021 02:50:37 GMT  
		Size: 3.2 MB (3177915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f4c1d69caf6add02d4549d216e9e00fdaae087f4d280cea93bbd3f8b3ec48a`  
		Last Modified: Fri, 01 Oct 2021 02:52:36 GMT  
		Size: 40.3 MB (40329415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d25b90928f781d816d02bea7d8f54221a35b29730fd84d0a00243b3b8bdb3e73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89892323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f73f0b59e7117c44cb5c0f23df871f926492ee7502ad7028f57ca74fe86c8cae`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:36:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:36:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a99a5951692580021e948472804dab0a010b074b1163b603e4f5cfda6382bf4`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 5.8 MB (5801664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fa544ba88c98b23feadb6ad914d8da1debe080907cb082ad2b8d8046e6c5da`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 4.2 MB (4185318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f556cc2020b283f43fb541b48641c7dd9e20e8d7d40de1a098420d28dbe5b70d`  
		Last Modified: Fri, 01 Oct 2021 02:43:07 GMT  
		Size: 47.4 MB (47399802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.10`

```console
$ docker pull buildpack-deps@sha256:7fbd1e542ffae01b709d0aee632c4405890505d79fd7331d8c75c847398e19a0
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
$ docker pull buildpack-deps@sha256:f6678c935da21dcc51c2272f514ae95e68946b6e94206470cfa7e0d3c84f3f33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371066555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f07948a9b90cd3d03abd58a6ebacbaa26c4f20e9a3ce2cd987bd465f4ed3965`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:27:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:28:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:30:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf1a9d4fbdb8bcdea8da245690e0e7b0d7f42cd7b7480dd3f9866881a1da2c`  
		Last Modified: Sat, 02 Oct 2021 22:43:19 GMT  
		Size: 3.4 MB (3448048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfa76bdfd39c414c299c1e02cf75c9b579b3aa69ca8e1abf9eb876765fcc9ab`  
		Last Modified: Sat, 02 Oct 2021 22:43:18 GMT  
		Size: 3.7 MB (3742516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360154fa07ad953713f7e71f7feffabf9f868fa69562aeb598e60ebd881ede16`  
		Last Modified: Sat, 02 Oct 2021 22:43:59 GMT  
		Size: 40.3 MB (40285193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb0c2a0ca1287f5644704ab6ae1dbfd650eeae5b8ce48ee335e46a1a2bd068`  
		Last Modified: Sat, 02 Oct 2021 22:46:58 GMT  
		Size: 296.7 MB (296673806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:173282a68ed3c7d434e0a049630d7ee47e5ff9b0937c87e24de80c41032b44f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.8 MB (399753642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c681f790e2c9ad75fe348a46f94492c9e4e2a4cf1c6e08b36b18048884d41020`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:20:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:21:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e1bb6cc21d9aa99ea2365d91ca737ff33423cf8eef3ac6d444f9264ecf62c`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.7 MB (3680866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44384e90f77381715996a06f1aef553b1ffe6e32cd9f467350b914746ba678eb`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.5 MB (3533741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc1cb90f475d191407aa41ee7d90ffd845371c604e65fedf778556ba48612f`  
		Last Modified: Fri, 01 Oct 2021 03:27:51 GMT  
		Size: 38.0 MB (38028253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fd4f9a27c5ce4d91f6bfc6770ad8a8b894911d0d94e7e683e9c34844be1c22`  
		Last Modified: Fri, 01 Oct 2021 03:28:51 GMT  
		Size: 325.5 MB (325462804 bytes)  
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
$ docker pull buildpack-deps@sha256:4b22a884a0b2e518316ae5bca5a1d25a68152cbcd931d8334e80136baac33ec5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.5 MB (266483053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad71d8370638795c9aa2a2d157409cd2ca60b36e0d78e0577c61ffd4d3c3dbd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:22:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:26:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70e1ff9e0960442ac8e0ed27318b8f50e84d12cbedd17b4f36bfa157115adc7`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.5 MB (3490761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2050b829842e591df4469c3681081a8cf61654b45f11d26e6953e514d6869b93`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.8 MB (3803189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c488cbe594d2cf170d43a86c8cde4efc13bd529cf61fd3b9acb9ff640aa8b617`  
		Last Modified: Fri, 01 Oct 2021 03:01:12 GMT  
		Size: 40.8 MB (40766562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f040e257abcc701d46bbbbe741df280b9aad1f553176cb2cffa3942dcd9f8`  
		Last Modified: Fri, 01 Oct 2021 03:06:53 GMT  
		Size: 191.2 MB (191212371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5d93cb79d0be2d3b6dac44f7bee954e47d7ab6d8d36f720c33ae06bd99f4169d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **368.6 MB (368601732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4cb7d0c0fad2b9c9cc6a8a2ab173d8b458b98e9846a12911c9774f79387c4d6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:37:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:38:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b6878da56179520aa932c74d47a6c136df51a8b1637756607aa579385b2746`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 3.8 MB (3772798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0073edd8de7859cbb99a9c2b5013c571d603c0c9095297840395b0e5e932a`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 4.0 MB (3962742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9b7e9f35321824c609d7b2bb42e9070012f04eaa33b52f09bb9a38035d69b`  
		Last Modified: Fri, 01 Oct 2021 02:43:53 GMT  
		Size: 38.5 MB (38465117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faacb0872b812a99e17e5d5540d296d9b05d9c300e5fdb801f95c6f65f30a5bb`  
		Last Modified: Fri, 01 Oct 2021 02:44:34 GMT  
		Size: 291.6 MB (291631034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.10-curl`

```console
$ docker pull buildpack-deps@sha256:c53ef4db48421b2adf8683f1b54765147b1541a3ee77786cce257a30d7b6618a
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
$ docker pull buildpack-deps@sha256:6f1b35544a0f47df6f3c77730b3abce82ab8f874d64ea57a6318bfe3886ea43c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34107556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65f89e7cb018e5ef861aac53d03ef2134aad620b25c5ba3ae9e97bd532d3afa2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:27:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf1a9d4fbdb8bcdea8da245690e0e7b0d7f42cd7b7480dd3f9866881a1da2c`  
		Last Modified: Sat, 02 Oct 2021 22:43:19 GMT  
		Size: 3.4 MB (3448048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfa76bdfd39c414c299c1e02cf75c9b579b3aa69ca8e1abf9eb876765fcc9ab`  
		Last Modified: Sat, 02 Oct 2021 22:43:18 GMT  
		Size: 3.7 MB (3742516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7704b5aa6e272ae4a82b3c66c9225a8d696accdedfb151a8681c4cdab189613e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36262585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd4a61178d340fd4853667bbd899f1369ee072493c1af28b3ed5e3be47647e15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:20:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e1bb6cc21d9aa99ea2365d91ca737ff33423cf8eef3ac6d444f9264ecf62c`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.7 MB (3680866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44384e90f77381715996a06f1aef553b1ffe6e32cd9f467350b914746ba678eb`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.5 MB (3533741 bytes)  
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
$ docker pull buildpack-deps@sha256:6a154a1ef63633b46544bec5933e9dbe4d3157815ff444ebe0934ebe303649af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34504120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebba9aeb40f4e46a40589114f0d4d5c25be4b7f994275697a4fffce0cc11bb6a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:22:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70e1ff9e0960442ac8e0ed27318b8f50e84d12cbedd17b4f36bfa157115adc7`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.5 MB (3490761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2050b829842e591df4469c3681081a8cf61654b45f11d26e6953e514d6869b93`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.8 MB (3803189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3a462412b2ea7abd320c5cd6f0aa28db8d7e8d792e1e76d9b0fe3be5a140fe34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.5 MB (38505581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28fe7943e40f4cf73087bf161365c6df15f51d6944635b2ea3db8fbb265b8cc6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b6878da56179520aa932c74d47a6c136df51a8b1637756607aa579385b2746`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 3.8 MB (3772798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0073edd8de7859cbb99a9c2b5013c571d603c0c9095297840395b0e5e932a`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 4.0 MB (3962742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:21.10-scm`

```console
$ docker pull buildpack-deps@sha256:3277805f61b64f42f04803682a5eaf665546adb4c686e862a908154390d13afe
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
$ docker pull buildpack-deps@sha256:02dfe5f7d0812d54877e010ea6b4e17b3b364a652ddf0a774618e2ac5b340d3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74392749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c35e1202679199aba724b66d88d092b202ce0a720f1fbc4774055a08a40372d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:27:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:28:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf1a9d4fbdb8bcdea8da245690e0e7b0d7f42cd7b7480dd3f9866881a1da2c`  
		Last Modified: Sat, 02 Oct 2021 22:43:19 GMT  
		Size: 3.4 MB (3448048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfa76bdfd39c414c299c1e02cf75c9b579b3aa69ca8e1abf9eb876765fcc9ab`  
		Last Modified: Sat, 02 Oct 2021 22:43:18 GMT  
		Size: 3.7 MB (3742516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360154fa07ad953713f7e71f7feffabf9f868fa69562aeb598e60ebd881ede16`  
		Last Modified: Sat, 02 Oct 2021 22:43:59 GMT  
		Size: 40.3 MB (40285193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c8f600d722b8fef5ba12089908ede3d8e42a8ae5775432fa2c949724d0b39b60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74290838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ffdc048016e92cdb4284d1e4093a42af66850bc50f54b2d70eb68e9e2ddd9e6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:20:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e1bb6cc21d9aa99ea2365d91ca737ff33423cf8eef3ac6d444f9264ecf62c`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.7 MB (3680866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44384e90f77381715996a06f1aef553b1ffe6e32cd9f467350b914746ba678eb`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.5 MB (3533741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc1cb90f475d191407aa41ee7d90ffd845371c604e65fedf778556ba48612f`  
		Last Modified: Fri, 01 Oct 2021 03:27:51 GMT  
		Size: 38.0 MB (38028253 bytes)  
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
$ docker pull buildpack-deps@sha256:ade44386814b1fbd659c00f2a3d39aaf1f5e74fec0ea0a0978930664ac2d0756
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75270682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4655c550ee38a21c24aed852af8cc275584e860f253b1ad2927e749aed931a12`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:22:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:26:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70e1ff9e0960442ac8e0ed27318b8f50e84d12cbedd17b4f36bfa157115adc7`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.5 MB (3490761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2050b829842e591df4469c3681081a8cf61654b45f11d26e6953e514d6869b93`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.8 MB (3803189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c488cbe594d2cf170d43a86c8cde4efc13bd529cf61fd3b9acb9ff640aa8b617`  
		Last Modified: Fri, 01 Oct 2021 03:01:12 GMT  
		Size: 40.8 MB (40766562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:21.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ecfa20db4ba0c46a95b9062c544043b189956610ad948cd4c5aea2ab12d6b551
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76970698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd7e97f3e90d1d954fd5d7177fa80b54889084f4747a02d4d86c8892a60f46e1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:37:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b6878da56179520aa932c74d47a6c136df51a8b1637756607aa579385b2746`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 3.8 MB (3772798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0073edd8de7859cbb99a9c2b5013c571d603c0c9095297840395b0e5e932a`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 4.0 MB (3962742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9b7e9f35321824c609d7b2bb42e9070012f04eaa33b52f09bb9a38035d69b`  
		Last Modified: Fri, 01 Oct 2021 02:43:53 GMT  
		Size: 38.5 MB (38465117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:df4ae151dd3b2a262ac789bf17f72249659c5896b065e55a0ae78dd098dff04f
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
$ docker pull buildpack-deps@sha256:3c0807515e128baced0d30bb957832be1e298498ab4ae27e19a9790933a98442
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221261333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3fc72df6ea346e4d81aac88ec7ea1d73ce5a1b4c228bd00daffd981222f849`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:02:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:06:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1404df7fbdef68bea55f7c051dbdb1aac1e564886ca277d1f8b1d0bf3fbe8e4`  
		Last Modified: Fri, 01 Oct 2021 03:17:56 GMT  
		Size: 6.6 MB (6643379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964552afca366bca79302ab79366a0528db0710e3db41a0a5c40e90d1b936c20`  
		Last Modified: Fri, 01 Oct 2021 03:17:55 GMT  
		Size: 3.0 MB (3022502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f547fe5b8db9e7e53004a6ebd2656feef7a91d529f9cb21c95b3bc8b108e19`  
		Last Modified: Fri, 01 Oct 2021 03:18:13 GMT  
		Size: 45.5 MB (45477448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d3bc1c26143d890a32399b1baeb259de8bf2f6b5f65036e6dbaca6547f8f`  
		Last Modified: Fri, 01 Oct 2021 03:18:43 GMT  
		Size: 139.4 MB (139412929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:97c8663ef94b6784716e35962fff55cb99ee462056102e3cda9be49001f993c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189465194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db87044597f36141e8a2573b7ece145ddc2ad4d736a3e55c32e4066919746419`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:17:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:17:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:20:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0514bc47630e4346d13917c20c9a52eb361c5077c2b17f804d305bb3aeeae1ec`  
		Last Modified: Sat, 02 Oct 2021 22:36:02 GMT  
		Size: 5.7 MB (5713518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43197d564770c4e86c4ec1c0d141238ad2a175e92bebfa12b212b729f581ae62`  
		Last Modified: Sat, 02 Oct 2021 22:36:00 GMT  
		Size: 2.6 MB (2584549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd05568a3d4d96e48d84348793a6345f8359538aed1403669bef0db7a6f026c`  
		Last Modified: Sat, 02 Oct 2021 22:36:42 GMT  
		Size: 40.7 MB (40670724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908028762c0e5308de465f408ec635ee851602976ce9a8884e0b9c1c3372bf64`  
		Last Modified: Sat, 02 Oct 2021 22:38:05 GMT  
		Size: 118.2 MB (118192099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bb8ee9051e7d4b54ae564f9b794edcb3d43512f0da2f32ffa6fff0b346fcc4ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205821969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b433afcd80444e75da56050c2f2fb8a3fcac5258832102e7dde4be0707285e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:15:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:15:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:16:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ae8f73d2b97ae6f304518bd244cd1e218386861b11878333a3e1704cd06fc4`  
		Last Modified: Fri, 01 Oct 2021 03:24:20 GMT  
		Size: 6.1 MB (6085031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc43f166dad077ef896c5d7e305f3a19ff7f4c0245159dede3adee91cf2fb17`  
		Last Modified: Fri, 01 Oct 2021 03:24:19 GMT  
		Size: 2.8 MB (2783140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a133bda1a844b0b9e9ac0284af4779d5ec158f5693b56511a1f27a5cbc8f541`  
		Last Modified: Fri, 01 Oct 2021 03:24:38 GMT  
		Size: 43.3 MB (43269968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba35ad1221e5859d39cb2b5e83e0f09f32a679b01ad0cf9bd7d43f755fce8ca`  
		Last Modified: Fri, 01 Oct 2021 03:25:08 GMT  
		Size: 130.0 MB (129956354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9f10a9ee18f6be60bfe5500c424c0125ad8e8b34ef076b08278d9a12cf826537
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.6 MB (218560267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419b39771048169c84a707f522a0987ffe42bf3349a0ab49e3abac9277252716`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:14:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 04:15:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:18:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89515178f4a354382498077df201d0c7296621351f651bf1d7bda94f1d499466`  
		Last Modified: Fri, 01 Oct 2021 04:21:07 GMT  
		Size: 6.9 MB (6932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99224216777e769a2c151c0c091ec4cda2a5d5f541c203e203683c71b6cb4a9f`  
		Last Modified: Fri, 01 Oct 2021 04:21:06 GMT  
		Size: 3.3 MB (3252987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8565053f61bc235064ba9f6560e2464bd101da6ba901ae2152a5198bac7f4e3`  
		Last Modified: Fri, 01 Oct 2021 04:21:29 GMT  
		Size: 47.1 MB (47065713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0502655b09b53ef4e834ca20300b20d019082bfbe8caad5e33e24676ce7aa8`  
		Last Modified: Fri, 01 Oct 2021 04:22:13 GMT  
		Size: 134.2 MB (134150425 bytes)  
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
$ docker pull buildpack-deps@sha256:5936655630734b659a06da22719a5788844863d57670778cb9d6bc1f79007ddb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.6 MB (205618219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ec7d1aadb3df4675c40b4a20c77c55defab1ae414d0cc9570efce58c897ac6a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:33:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:33:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f1e9a656ce747f09402ff405b881ebbce2041d0228e2373aac2dbfe9a23fd8`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 6.3 MB (6334289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe96b416a4fa4b5de3ab17b5e2b2b85bde2482559e7592284278d282da0c067`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 3.0 MB (2974970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6a10244fc86eb56eba2d1e8554fe9b23b582e56b7728fcb21fee59a9313d52`  
		Last Modified: Fri, 01 Oct 2021 02:41:34 GMT  
		Size: 45.0 MB (45016989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8108fe4f05569dd68d228c1be27552ed405fc79994a5cb6f78b8c142ff1ed6da`  
		Last Modified: Fri, 01 Oct 2021 02:41:57 GMT  
		Size: 125.9 MB (125929053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:5325fe2efe7693bcef1ab64f89cfc05be2520bd07181e6671aef7eaac3e251d8
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
$ docker pull buildpack-deps@sha256:64e7d3f7a80ed2f1f95becd49baec3998ce6eb2c56d783ac2d1fc2fb85c6dc73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36370956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6fda0143b32371ab8b25a7e99a8957c2fe2207f5bd81e75e06bd1def8efa61f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:02:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1404df7fbdef68bea55f7c051dbdb1aac1e564886ca277d1f8b1d0bf3fbe8e4`  
		Last Modified: Fri, 01 Oct 2021 03:17:56 GMT  
		Size: 6.6 MB (6643379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964552afca366bca79302ab79366a0528db0710e3db41a0a5c40e90d1b936c20`  
		Last Modified: Fri, 01 Oct 2021 03:17:55 GMT  
		Size: 3.0 MB (3022502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3a63e143a2e16370a02a00761f4a94d18cb53969185afd48c00b69ad5d1909cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30602371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c8095f1395eb522f1177e72c5b745d6332913041081bbcc6a66c718a6179830`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:17:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:17:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0514bc47630e4346d13917c20c9a52eb361c5077c2b17f804d305bb3aeeae1ec`  
		Last Modified: Sat, 02 Oct 2021 22:36:02 GMT  
		Size: 5.7 MB (5713518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43197d564770c4e86c4ec1c0d141238ad2a175e92bebfa12b212b729f581ae62`  
		Last Modified: Sat, 02 Oct 2021 22:36:00 GMT  
		Size: 2.6 MB (2584549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:39ab1f63e4c0b3e09586c549569cabdb152a84d2506e7a763bb7073c51e17f49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32595647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5ce59175e5046b186b7c888fe1322f90eadd0eb2dbf8c78060b2bf4db8ab99b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:15:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:15:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ae8f73d2b97ae6f304518bd244cd1e218386861b11878333a3e1704cd06fc4`  
		Last Modified: Fri, 01 Oct 2021 03:24:20 GMT  
		Size: 6.1 MB (6085031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc43f166dad077ef896c5d7e305f3a19ff7f4c0245159dede3adee91cf2fb17`  
		Last Modified: Fri, 01 Oct 2021 03:24:19 GMT  
		Size: 2.8 MB (2783140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b6b5a071215a2d0e46fc410080e7957427beb8fb6444a95686284df0b0c2720d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37344129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2455fd5918f65a81c70a107effdaedc75df1f1ca4349cbc2e8051c0378cecf5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:14:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89515178f4a354382498077df201d0c7296621351f651bf1d7bda94f1d499466`  
		Last Modified: Fri, 01 Oct 2021 04:21:07 GMT  
		Size: 6.9 MB (6932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99224216777e769a2c151c0c091ec4cda2a5d5f541c203e203683c71b6cb4a9f`  
		Last Modified: Fri, 01 Oct 2021 04:21:06 GMT  
		Size: 3.3 MB (3252987 bytes)  
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
$ docker pull buildpack-deps@sha256:558995a4b832c433e78e0ac738c121aa35235fda0b38e00def4386e6a5d4676b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34672177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799be440f53410fdee2a74a842e6b7b7586547315f6a0aba25e8a343ff7e0fa5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:33:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f1e9a656ce747f09402ff405b881ebbce2041d0228e2373aac2dbfe9a23fd8`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 6.3 MB (6334289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe96b416a4fa4b5de3ab17b5e2b2b85bde2482559e7592284278d282da0c067`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 3.0 MB (2974970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:4f0ee684a0e55ac502f98fdddd5138eabb1b95a33f6f2c7267484bfb35f3c46d
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
$ docker pull buildpack-deps@sha256:5e43b1ebcfe2b76e7912db780b8aac130c8578f962609f04f88de0e5abbb150c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81848404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2ce214211225c549bf9107a4c081cc04753411e5f7dc05e2fe18e780cb6807`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:02:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1404df7fbdef68bea55f7c051dbdb1aac1e564886ca277d1f8b1d0bf3fbe8e4`  
		Last Modified: Fri, 01 Oct 2021 03:17:56 GMT  
		Size: 6.6 MB (6643379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964552afca366bca79302ab79366a0528db0710e3db41a0a5c40e90d1b936c20`  
		Last Modified: Fri, 01 Oct 2021 03:17:55 GMT  
		Size: 3.0 MB (3022502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f547fe5b8db9e7e53004a6ebd2656feef7a91d529f9cb21c95b3bc8b108e19`  
		Last Modified: Fri, 01 Oct 2021 03:18:13 GMT  
		Size: 45.5 MB (45477448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:58947866db3f48fa361f7056b87a69b67ef6f4b3348e65f297ab297295dca8ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71273095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa26238d728f2e54ac4d6d4703e94f9750fa80cebe834eccf807a708e56ddd4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:17:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:17:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0514bc47630e4346d13917c20c9a52eb361c5077c2b17f804d305bb3aeeae1ec`  
		Last Modified: Sat, 02 Oct 2021 22:36:02 GMT  
		Size: 5.7 MB (5713518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43197d564770c4e86c4ec1c0d141238ad2a175e92bebfa12b212b729f581ae62`  
		Last Modified: Sat, 02 Oct 2021 22:36:00 GMT  
		Size: 2.6 MB (2584549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd05568a3d4d96e48d84348793a6345f8359538aed1403669bef0db7a6f026c`  
		Last Modified: Sat, 02 Oct 2021 22:36:42 GMT  
		Size: 40.7 MB (40670724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5da94e3b4e1ce6cd029b385bdd46bc85fdbd02dab217b66dd410c26f393fc219
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75865615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04215758cdb2f31d14432063ca393004a2b774b824c660ab4bd5870b9ae8d919`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:15:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:15:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ae8f73d2b97ae6f304518bd244cd1e218386861b11878333a3e1704cd06fc4`  
		Last Modified: Fri, 01 Oct 2021 03:24:20 GMT  
		Size: 6.1 MB (6085031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc43f166dad077ef896c5d7e305f3a19ff7f4c0245159dede3adee91cf2fb17`  
		Last Modified: Fri, 01 Oct 2021 03:24:19 GMT  
		Size: 2.8 MB (2783140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a133bda1a844b0b9e9ac0284af4779d5ec158f5693b56511a1f27a5cbc8f541`  
		Last Modified: Fri, 01 Oct 2021 03:24:38 GMT  
		Size: 43.3 MB (43269968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d9cab10f9ba15a4bf0183c6ef9ba2228cef5dcd289d8375067b643f7871634a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84409842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41a8d31955cc503b31fb1a846ae9d7a4ab19e619b95a661d1827f73e0e3ed711`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:14:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 04:15:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89515178f4a354382498077df201d0c7296621351f651bf1d7bda94f1d499466`  
		Last Modified: Fri, 01 Oct 2021 04:21:07 GMT  
		Size: 6.9 MB (6932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99224216777e769a2c151c0c091ec4cda2a5d5f541c203e203683c71b6cb4a9f`  
		Last Modified: Fri, 01 Oct 2021 04:21:06 GMT  
		Size: 3.3 MB (3252987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8565053f61bc235064ba9f6560e2464bd101da6ba901ae2152a5198bac7f4e3`  
		Last Modified: Fri, 01 Oct 2021 04:21:29 GMT  
		Size: 47.1 MB (47065713 bytes)  
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
$ docker pull buildpack-deps@sha256:4e8170c2f8d92780b4d06eb93b8653189f5ce8da2287d75ae8e6d231d825bdaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79689166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ca7a0f2efa94efec7d8ce8eb0e04a949e4acdb537896a432f28ecc1c1e1232`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:33:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:33:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f1e9a656ce747f09402ff405b881ebbce2041d0228e2373aac2dbfe9a23fd8`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 6.3 MB (6334289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe96b416a4fa4b5de3ab17b5e2b2b85bde2482559e7592284278d282da0c067`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 3.0 MB (2974970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6a10244fc86eb56eba2d1e8554fe9b23b582e56b7728fcb21fee59a9313d52`  
		Last Modified: Fri, 01 Oct 2021 02:41:34 GMT  
		Size: 45.0 MB (45016989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:e54ae211c5b7f7bef56152bd3004a28989c31d88a6a12e104ba91e715194af2a
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
$ docker pull buildpack-deps@sha256:dc426fff2922e74aa6934ccd1df91e1298cb3ccde18c2f1835f12e70f6220371
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (321969341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:714418fd1dff72d98cd2a7fe82a6a4636418db789278fba59735ebda645e9b27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8e6af58ed3a502f0c3c15dce636d9d362a742eb5b67770d0cfcb72f3a9884`  
		Last Modified: Tue, 28 Sep 2021 01:58:51 GMT  
		Size: 196.4 MB (196449829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7123e9831bb45f888b6806417d2dfe1f180e62e19c677b0d09abb7f80c311de8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295057178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6fd0cb97521cc96a0089159a684d52da508f86d751d5ccb9fa131a6b417689`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb5b710639fb53421f19a58b60a1a0cf28eea33da972ad7bcbab6628ed94797`  
		Last Modified: Tue, 28 Sep 2021 03:08:48 GMT  
		Size: 52.3 MB (52318852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff0c2fb11e77b1bab4e3d2c8b9ff79d5a4bfa2a4c81e291370227cdcf5eae2f`  
		Last Modified: Tue, 28 Sep 2021 03:10:48 GMT  
		Size: 174.6 MB (174640957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:337edfa1be8e16858eddd085e94b6742ba6d116a6e3734497043b26664d576a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282490296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d74011c8e2e7e4542e3f3cd14eafdc2eaff461a41a64d1cef541a8c4b30b501`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:32:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beba146f18f8bf327bfc67faba4e70c717e79ccc563c8b535e44e9c14c2edfc`  
		Last Modified: Fri, 01 Oct 2021 05:53:47 GMT  
		Size: 50.3 MB (50328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd4233acc34086e6db32b75d876bd6ea7538de484ea9b48c9ddd1907aa74ca0`  
		Last Modified: Fri, 01 Oct 2021 05:55:36 GMT  
		Size: 166.9 MB (166894450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3609418ae510b339d73ab6f19ba3a82c8e0bdc171f50df8949f0a3735de06667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313636281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a992d40e6a046b86ed17052793e80b837e5266c1a03f3261b2c558ddd77837f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7e4e85949ee45bae139f288bc1cd85a740b408abdefaaba118c4c4626b021e`  
		Last Modified: Tue, 28 Sep 2021 02:25:03 GMT  
		Size: 54.7 MB (54669786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69e7bcc0bc59e0f5c70e40bc8adebeb94f60240a71e7f8add74d8b9146bbc16`  
		Last Modified: Tue, 28 Sep 2021 02:25:44 GMT  
		Size: 189.3 MB (189337402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:777672fe2d3733ca92041d6bf3fe878cb1f5fdacc449e71e2217750a840bcdf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327745828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be8f244a554fc912c1932f609263329ff9b3d7bcabed8cb7ed0d6d657f5787f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9148b01e8bbfb04fa59f44e2af070eb74a8797213877fc7df3be0467115b9`  
		Last Modified: Tue, 28 Sep 2021 02:24:24 GMT  
		Size: 5.3 MB (5282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda7eaf6b4240f872ceef86fce4f8a87bdad74da3484b9605cb3b2b52cbbf20`  
		Last Modified: Tue, 28 Sep 2021 02:24:25 GMT  
		Size: 11.3 MB (11250636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50bcbe9fc6f4b839121363d75b4325536a717823ee2b2881b0247afe12fd6909`  
		Last Modified: Tue, 28 Sep 2021 02:24:58 GMT  
		Size: 55.9 MB (55916372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3de1989e93fff2054295962d5bbfbfb11bfa4533ad691aaa17c9a52e3a8a22b`  
		Last Modified: Tue, 28 Sep 2021 02:26:07 GMT  
		Size: 199.4 MB (199363599 bytes)  
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
$ docker pull buildpack-deps@sha256:decae382d4f56e845e9800f3b79f315daccccfb47340e44c9f09f0310e8b98d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330495335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c4c1fd57c37be3803887ab8eee646176344caa36226b3c0131b4cd932867afd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 05:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:13:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708d04ed929be54f33cfa94416648dcac9edd8c01746ecc6e250ce046aa54ac0`  
		Last Modified: Fri, 03 Sep 2021 07:09:38 GMT  
		Size: 58.8 MB (58849139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287624e1f6e58d3860703363b792d02bb699c973abd9dadfa2db8495b51ceb93`  
		Last Modified: Fri, 03 Sep 2021 07:12:15 GMT  
		Size: 195.8 MB (195799046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:51e14eaab3cc2825279677ba4a729da747e7686e4de1df8f933005cf8f8bc13b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295585571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa2779752696eb6bfd10f0076125e41a51fad44a72ed6a636d376f337c439375`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:08:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:08:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f5b44618c39b6606db01fa6d460b6b7e1415b3a9c5a0b2f8b179c9b2c3fcfe`  
		Last Modified: Tue, 28 Sep 2021 02:16:05 GMT  
		Size: 54.0 MB (54049595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6589c0454003c1deeaf24f87ae908e9816d7cb9a945148cf89e75038aba3c8`  
		Last Modified: Tue, 28 Sep 2021 02:16:32 GMT  
		Size: 172.4 MB (172435364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:8f4b29031e8204331606d488fb6290f99bc6ccc7f50623272e1e76a966487520
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
$ docker pull buildpack-deps@sha256:6d3bd0093dc57538be1da3cda96a80f944ab167c2f9fcff321db397d15923754
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70952632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f020ab5dd0cef2c0b20ded3f290546ae4b2a84986d4e02446879a72cf0d1cbd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:151b67336eac36e8c7376d2f603965b3d613b838a8c6c00df65ecb6b81ebb7e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68097369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecfe7b5c5061f7480a7a1a7306e93ea2082b63b6b9d1f29c9b01b70d4ae129e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:96c3837335e336493dd4ec502568a24fb8a0f808d15ed1a844c573d738b99ff4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65267580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feef68d841ccaedfa1bae704efe715b0f162812c549f94539d335e6784b6a512`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d685bcbd37d39eab77c65ae1e04e72d35d3ae193256f074d84a5c87d59842bf2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69629093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990cb9bf14263220789cdd25eb191d564fb567f94c522c1494a07737584426c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d4f08dbf769815a4db9592b6f8911b61ada4280051f115b8b5bf88c9ae6d6e18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72465857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f109721ea809e5ae6fcfd2a47160b846d943350a073e5e431b4bbbf9688d9d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9148b01e8bbfb04fa59f44e2af070eb74a8797213877fc7df3be0467115b9`  
		Last Modified: Tue, 28 Sep 2021 02:24:24 GMT  
		Size: 5.3 MB (5282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda7eaf6b4240f872ceef86fce4f8a87bdad74da3484b9605cb3b2b52cbbf20`  
		Last Modified: Tue, 28 Sep 2021 02:24:25 GMT  
		Size: 11.3 MB (11250636 bytes)  
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
$ docker pull buildpack-deps@sha256:e645211432960dea9563d3ce20b165c647ec21f29d3bc873e80e417076f5b108
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75847150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b9a35d2eb70c2fbc27b4c72a127f42b6b685425398b8ead7a2283f10e32ac5c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:076601aae27650f44b4dbe20132157de742e741af9d5fc796db9032604ab6cf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69100612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73dbb50e50b5a3c5d39455f73ca943eb867aba4106eb831077daf48cee43647a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:aff21a12bf0addfb7d8e7ec0a44f9ab92b3584123f7c53f9fe6cc389cc8937b5
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
$ docker pull buildpack-deps@sha256:7b5d4f456f733f3b3edd7ed483335144b45a696e113345e0de17d68282da6b9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125519512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86feaac141dee4502631bb241160217b3a0ab6ae94d3b92cac8e497122a21bd4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:538c56184e9c046dbf00c862d346eaf338eb52d01e0893de7465ddfad38a8fca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120416221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194745ae83d6667c4aaa0274aa16f19bda1548ec9df3d0f4a31cbaf1cac33cc4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb5b710639fb53421f19a58b60a1a0cf28eea33da972ad7bcbab6628ed94797`  
		Last Modified: Tue, 28 Sep 2021 03:08:48 GMT  
		Size: 52.3 MB (52318852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8ba983722fda8c96eea16075c06ea7ba1d31db604469814964d231058e89a7b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115595846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fca1b7d9db700c661f89b9b85208e186b5102852ed2a757bee9a93d693df7f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:32:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beba146f18f8bf327bfc67faba4e70c717e79ccc563c8b535e44e9c14c2edfc`  
		Last Modified: Fri, 01 Oct 2021 05:53:47 GMT  
		Size: 50.3 MB (50328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ea086e8562101d3a3394d2405d80f211ec6792aed4ddbd25b5e52076e46fabce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124298879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd9f391f5d78e3aaeae0ee78fa5ce45069ef631e2579ddbdcb8873a48c73d44`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7e4e85949ee45bae139f288bc1cd85a740b408abdefaaba118c4c4626b021e`  
		Last Modified: Tue, 28 Sep 2021 02:25:03 GMT  
		Size: 54.7 MB (54669786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:46af4ece25d50f83819e2b897da064fd307a295d2770db9f80951a93e899a26f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128382229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca69ee284e3152e65f20eb98f1ae6c36fbc3ff0127b68c6e8d0d13550e9f6147`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9148b01e8bbfb04fa59f44e2af070eb74a8797213877fc7df3be0467115b9`  
		Last Modified: Tue, 28 Sep 2021 02:24:24 GMT  
		Size: 5.3 MB (5282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda7eaf6b4240f872ceef86fce4f8a87bdad74da3484b9605cb3b2b52cbbf20`  
		Last Modified: Tue, 28 Sep 2021 02:24:25 GMT  
		Size: 11.3 MB (11250636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50bcbe9fc6f4b839121363d75b4325536a717823ee2b2881b0247afe12fd6909`  
		Last Modified: Tue, 28 Sep 2021 02:24:58 GMT  
		Size: 55.9 MB (55916372 bytes)  
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
$ docker pull buildpack-deps@sha256:0079fcd37f046fdbc47f73c68e3301b7cb70947b2a248d6c3fc28008143759bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134696289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a755e8f1b32b86a7e3c3eb1702fb2c523aacade98b66f54fdbd1dc1631465c0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 05:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708d04ed929be54f33cfa94416648dcac9edd8c01746ecc6e250ce046aa54ac0`  
		Last Modified: Fri, 03 Sep 2021 07:09:38 GMT  
		Size: 58.8 MB (58849139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cc8ac782325035a5a46cf050e7b6611363ec94c8185f01f0b41b2d32a65f1720
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ee600655618ac729e88fc65d35e10aa6b00c909cee23ef5ab5b3c92ceee8f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:08:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f5b44618c39b6606db01fa6d460b6b7e1415b3a9c5a0b2f8b179c9b2c3fcfe`  
		Last Modified: Tue, 28 Sep 2021 02:16:05 GMT  
		Size: 54.0 MB (54049595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:df00248c216c6ee635cfe9ab3ef070aadd0a58d5ac3da08ed2e4273d4800e54d
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
$ docker pull buildpack-deps@sha256:a8b925ea43a7c8274883997d8d99f17e04a538f4341922bf932e568159e77792
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312503548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83822a8b0862d52f928785e1b80bcb435ba149468c258ffc02f097a8328f717c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:52:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4689f0588c1ba01108f5c6d33943d3d542ae339fd526390d07c7a00ded6473`  
		Last Modified: Tue, 28 Sep 2021 02:00:03 GMT  
		Size: 192.4 MB (192395236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cb5619367c2bf980f5783130cb7d9980a7d349cb5cc1812120b21cdc6ffddfdb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286124998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c41bb4eeaabaad7b56074bae8da8102422bde45f973b2122d9133d93ab014a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:08 GMT
ADD file:f4b6a4e04436efee878ec0804c89afd419015b881385db438e7374e421f7609f in / 
# Tue, 28 Sep 2021 01:51:09 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:52:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:52:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:56:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:860bc9b218abb92e3ca4715f45696ea7ad7927f9c74dfc2d5ab04672145effb2`  
		Last Modified: Tue, 28 Sep 2021 02:07:23 GMT  
		Size: 48.2 MB (48153768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a08133922bd88680cb57f3f77cf4659368c851186070f4bde20308826e0e1`  
		Last Modified: Tue, 28 Sep 2021 03:11:09 GMT  
		Size: 7.4 MB (7376971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a684cac2ccf5e45585c1c543d29c97343bdc822cfe2771bef89eec53404dfe3`  
		Last Modified: Tue, 28 Sep 2021 03:11:10 GMT  
		Size: 9.7 MB (9687508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d864b5875ad7a90124a6af2aa184ef6d85c03e202f11334ee9801d1f33f723d7`  
		Last Modified: Tue, 28 Sep 2021 03:11:56 GMT  
		Size: 49.6 MB (49575651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e43481adfc889d8fe3a14c88589e95ac235c7d707521011521cf627d755b5c5`  
		Last Modified: Tue, 28 Sep 2021 03:13:51 GMT  
		Size: 171.3 MB (171331100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:86a29bffda8650549c1ec9c5ea4561d583afd59ff450fceffd9f33aa37a4f318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278335461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b011fe4ff66214904a51adbf9f81990a976446dc90b77a373eea263f4cc173b6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:34 GMT
ADD file:da3730d9c05fab2433637063dc9d51b2505bb6023c391d606419bc9a0874c131 in / 
# Thu, 30 Sep 2021 18:03:35 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:35:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:35:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:38:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d333743b3b21fdfd6ba3f4a0624204b620b72c3d0eb2c3dd9e39d23f3a87e9c`  
		Last Modified: Thu, 30 Sep 2021 18:20:10 GMT  
		Size: 45.9 MB (45917880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d8928e133ca4adc2e7f254a958f120743ac165e45332c8f2713144cf1e1c5`  
		Last Modified: Fri, 01 Oct 2021 05:55:55 GMT  
		Size: 7.1 MB (7124916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a975074459ff1f9c6b99644b138401f840f49a4dc1ef138661e138db9cd00038`  
		Last Modified: Fri, 01 Oct 2021 05:55:56 GMT  
		Size: 9.3 MB (9343736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a11c276eb14e33bd12beadc8185183d0805aee55492c4f89cf581d75ed1b203`  
		Last Modified: Fri, 01 Oct 2021 05:56:40 GMT  
		Size: 47.4 MB (47356508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee394d962f6e270a45df67b6ef4d987de06705c8153be2c5302e564b810af80e`  
		Last Modified: Fri, 01 Oct 2021 05:58:23 GMT  
		Size: 168.6 MB (168592421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37f7f9b7c6198c73db5e169b3bbace227726da55023379ade00652a258056d3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (303046386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb4108496fbc1d39b4a0ff45e7eeda902949c41b35102034c821e37329d5374c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619d0551980848579ec373733f2fb35c7deddf13e6e56747ddf13dedc6ddbf6b`  
		Last Modified: Tue, 28 Sep 2021 02:26:20 GMT  
		Size: 52.2 MB (52167859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2577d89b67b3c6b82eba3af07fcab6fb023276c144328ee678f9ef6cc14d174f`  
		Last Modified: Tue, 28 Sep 2021 02:26:57 GMT  
		Size: 184.0 MB (183975976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7114ff8bb18a281e793d91a8769338f67b1e7a43c815ca8541ec569688236589
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321917223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d3efff9249d5395fa5f207bff8d4204af1201dd7f77de39ca8f554cf61d58c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:28 GMT
ADD file:f0e83dd2590d6bd2d3726ebb3ebb5bfc0c2a52fe9feaeecd60b036c8eff69788 in / 
# Tue, 28 Sep 2021 01:40:28 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6f6f4e486b0370ea7bec101a3770e19279a47ffd7d20a9c48000fe3e63917bc`  
		Last Modified: Tue, 28 Sep 2021 01:49:34 GMT  
		Size: 51.2 MB (51207376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcad00d036c37c4de05381481665b986170717ee59000d1a49fa9e0d73ef484`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 8.0 MB (8000034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f546ea183fd0e99a89120a49252894e7056ddf33329190affa0efa1b5de5d929`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 10.3 MB (10340144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b68564816940e410e66659fa680b3832e7c4d11ee4e50beaf82cacad47ea57`  
		Last Modified: Tue, 28 Sep 2021 02:26:52 GMT  
		Size: 53.4 MB (53438192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60d099a705a23b8d0a57ed92ee5a3d6d96aca2e11c16c06dda6e309641a1a0f`  
		Last Modified: Tue, 28 Sep 2021 02:27:46 GMT  
		Size: 198.9 MB (198931477 bytes)  
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
$ docker pull buildpack-deps@sha256:5368ed059494735fb5715f20cc76c3167ddb776165acde462451e82148dcd4b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333924815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fba6d1a245467d4791c8fdd942cb667cd733fa9d04603f955d2a1b4e47e6a1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:41 GMT
ADD file:1f8eebd902d2881786014a1e5db3cd6f0bab3a55e23befcd6cb6e4d91b9e6d79 in / 
# Fri, 03 Sep 2021 01:23:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:17:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:42:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:20ef04c157f9b9866c6408757e7ba2534608600e6cadbb759175572efc03f830`  
		Last Modified: Fri, 03 Sep 2021 01:38:28 GMT  
		Size: 54.2 MB (54182653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6474492bb0f747d1f925e9a2e0ed1d7b0bd0fdaa043e1fb2e892dde4313615`  
		Last Modified: Fri, 03 Sep 2021 07:12:35 GMT  
		Size: 8.3 MB (8272834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e098e859433301d306293ed680efa3bdc7d574613acc0d17fd90c09e854f779`  
		Last Modified: Fri, 03 Sep 2021 07:12:38 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0210891d190261ad1963160b64e1e7e13a3b1e4b1ac8f297c5280432fa730`  
		Last Modified: Fri, 03 Sep 2021 07:13:03 GMT  
		Size: 57.5 MB (57457148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a2531ea29e5d6a6e910840570189332f132c3c99c3ca0ce21f40c4311be87`  
		Last Modified: Fri, 03 Sep 2021 07:13:52 GMT  
		Size: 203.3 MB (203284346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:de1ca69c22fd69b717ca75b737f12832a22bd0b4a11ca5a232c08569d2486ac8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294546359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c6959dfb787c69963ab5d333eb3409ae0add59a3b30b7b078345761c3c3132`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:11 GMT
ADD file:9eb47cd6584ec05371051b5cae96c24e6f03e66328173f27a9f30d46b8bce760 in / 
# Tue, 28 Sep 2021 01:43:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:09:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:10:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1481e22e2c9526464f32062da733ce595a9491b1e48870f085365fb7f9e8b60c`  
		Last Modified: Tue, 28 Sep 2021 01:49:17 GMT  
		Size: 49.0 MB (49004320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe83b756a24fd473ce558a06ee5b580a63605b4d9d74817e2e1d1289f54fb7f`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 7.4 MB (7400854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ed278d1f7ac1eb211375face0ceb4605c67610e32fce9d7601efdda86b1fc7`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 9.9 MB (9883204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9675b3feffe472a443ef929f8e972471bd03506cf0ad31270751bfaad5feca5d`  
		Last Modified: Tue, 28 Sep 2021 02:16:56 GMT  
		Size: 51.4 MB (51380496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36130191b2129cf0a0e3c1befece18304ff6e2ad271d3d2a846b4bcb4fbea3fb`  
		Last Modified: Tue, 28 Sep 2021 02:17:23 GMT  
		Size: 176.9 MB (176877485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:207f50e59fabb88d78c4176003fe96ac785480475b5cfe356ef8808abd41701d
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
$ docker pull buildpack-deps@sha256:edb926861a9d4f502a93284830ab70dd511f10dba22d427145e7cef74971a4bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68267001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd96ac6c32156cf1a1c658177b9a3ee1c76550262bb5f66ea623755636e8df5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:614551a10c9ad7fccd0189f174cbf1fb15ea6db182f9158bcb7d472e7d0ec87c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65218247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d956c4cef36a85f57f008f68da4d1e02c289909cd4607c52fe1bcfe63079b6a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:08 GMT
ADD file:f4b6a4e04436efee878ec0804c89afd419015b881385db438e7374e421f7609f in / 
# Tue, 28 Sep 2021 01:51:09 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:52:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:52:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:860bc9b218abb92e3ca4715f45696ea7ad7927f9c74dfc2d5ab04672145effb2`  
		Last Modified: Tue, 28 Sep 2021 02:07:23 GMT  
		Size: 48.2 MB (48153768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a08133922bd88680cb57f3f77cf4659368c851186070f4bde20308826e0e1`  
		Last Modified: Tue, 28 Sep 2021 03:11:09 GMT  
		Size: 7.4 MB (7376971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a684cac2ccf5e45585c1c543d29c97343bdc822cfe2771bef89eec53404dfe3`  
		Last Modified: Tue, 28 Sep 2021 03:11:10 GMT  
		Size: 9.7 MB (9687508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f6bf363f70c4023252f05afb24e47707d679a7228fa239d8cab73aa597b22b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62386532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5a3989375ad180ece61400975a554ee45480a60a4f7f27a3815e180bc6edf6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:34 GMT
ADD file:da3730d9c05fab2433637063dc9d51b2505bb6023c391d606419bc9a0874c131 in / 
# Thu, 30 Sep 2021 18:03:35 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:35:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:35:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2d333743b3b21fdfd6ba3f4a0624204b620b72c3d0eb2c3dd9e39d23f3a87e9c`  
		Last Modified: Thu, 30 Sep 2021 18:20:10 GMT  
		Size: 45.9 MB (45917880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d8928e133ca4adc2e7f254a958f120743ac165e45332c8f2713144cf1e1c5`  
		Last Modified: Fri, 01 Oct 2021 05:55:55 GMT  
		Size: 7.1 MB (7124916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a975074459ff1f9c6b99644b138401f840f49a4dc1ef138661e138db9cd00038`  
		Last Modified: Fri, 01 Oct 2021 05:55:56 GMT  
		Size: 9.3 MB (9343736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2616077fc9c85155a8638e3e522d8f64954d4729c41f266ab5c08725865e3863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66902551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd63debe5398b56ac201dd8e696edba5a4ebfbc032935e65f2a77a0697f1785f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bd063e941f2bd56c9767dc264c9725a8aad4b1cb540589077951538b80e08cd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69547554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8221d1cae77e18f41dcecbcf9a45df7f68f7964a3fcd54081714b98ea6f1b9db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:28 GMT
ADD file:f0e83dd2590d6bd2d3726ebb3ebb5bfc0c2a52fe9feaeecd60b036c8eff69788 in / 
# Tue, 28 Sep 2021 01:40:28 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6f6f4e486b0370ea7bec101a3770e19279a47ffd7d20a9c48000fe3e63917bc`  
		Last Modified: Tue, 28 Sep 2021 01:49:34 GMT  
		Size: 51.2 MB (51207376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcad00d036c37c4de05381481665b986170717ee59000d1a49fa9e0d73ef484`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 8.0 MB (8000034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f546ea183fd0e99a89120a49252894e7056ddf33329190affa0efa1b5de5d929`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 10.3 MB (10340144 bytes)  
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
$ docker pull buildpack-deps@sha256:06acd573d66fccb4d006a69d7299464eade5f43cf3257765ff58cfdd52e9c505
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73183321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7c2ade806dee7826b8dc1619005e756a05fc525d79818df01e1bd6779cb8b15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:41 GMT
ADD file:1f8eebd902d2881786014a1e5db3cd6f0bab3a55e23befcd6cb6e4d91b9e6d79 in / 
# Fri, 03 Sep 2021 01:23:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:17:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:20ef04c157f9b9866c6408757e7ba2534608600e6cadbb759175572efc03f830`  
		Last Modified: Fri, 03 Sep 2021 01:38:28 GMT  
		Size: 54.2 MB (54182653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6474492bb0f747d1f925e9a2e0ed1d7b0bd0fdaa043e1fb2e892dde4313615`  
		Last Modified: Fri, 03 Sep 2021 07:12:35 GMT  
		Size: 8.3 MB (8272834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e098e859433301d306293ed680efa3bdc7d574613acc0d17fd90c09e854f779`  
		Last Modified: Fri, 03 Sep 2021 07:12:38 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a0a905bf7ea807b467faf44795dd9bc40297712a3c86f2f4871bc6e031a23f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66288378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7636bb61ce8f549e8684021e135baf9a7a29dfb066c765ef9068fc2e83ac9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:11 GMT
ADD file:9eb47cd6584ec05371051b5cae96c24e6f03e66328173f27a9f30d46b8bce760 in / 
# Tue, 28 Sep 2021 01:43:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:09:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1481e22e2c9526464f32062da733ce595a9491b1e48870f085365fb7f9e8b60c`  
		Last Modified: Tue, 28 Sep 2021 01:49:17 GMT  
		Size: 49.0 MB (49004320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe83b756a24fd473ce558a06ee5b580a63605b4d9d74817e2e1d1289f54fb7f`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 7.4 MB (7400854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ed278d1f7ac1eb211375face0ceb4605c67610e32fce9d7601efdda86b1fc7`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 9.9 MB (9883204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:058827d111a2b33f792842da87bc23c3d158cbb1d8136296a2207890d374c640
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
$ docker pull buildpack-deps@sha256:67148e57c764d3a2c77564eb20f0bb6962c638e6f6466bf95acdacba0767f308
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120108312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9dc095a964929680f2a54eed2cb176fc1d653e640e643055e1f3cb1ed4d2636`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:38ee065e9b6ab25e9c6982fbbb963624343bd3f535f29bdea9904a8de690f9fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114793898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18f8633cc1c6c59527e9f5187fe319343106249601e7853ad38af3bee6a2869`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:08 GMT
ADD file:f4b6a4e04436efee878ec0804c89afd419015b881385db438e7374e421f7609f in / 
# Tue, 28 Sep 2021 01:51:09 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:52:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:52:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:860bc9b218abb92e3ca4715f45696ea7ad7927f9c74dfc2d5ab04672145effb2`  
		Last Modified: Tue, 28 Sep 2021 02:07:23 GMT  
		Size: 48.2 MB (48153768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a08133922bd88680cb57f3f77cf4659368c851186070f4bde20308826e0e1`  
		Last Modified: Tue, 28 Sep 2021 03:11:09 GMT  
		Size: 7.4 MB (7376971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a684cac2ccf5e45585c1c543d29c97343bdc822cfe2771bef89eec53404dfe3`  
		Last Modified: Tue, 28 Sep 2021 03:11:10 GMT  
		Size: 9.7 MB (9687508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d864b5875ad7a90124a6af2aa184ef6d85c03e202f11334ee9801d1f33f723d7`  
		Last Modified: Tue, 28 Sep 2021 03:11:56 GMT  
		Size: 49.6 MB (49575651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:524f675f694d3c2ecebf0781610fb0ff3e9095192bacf31a0306c7d10ba6c006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109743040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e42e135b01508bd6da66e6686e929d2ed404d2eafeceb8d40e88e23eafef828`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:34 GMT
ADD file:da3730d9c05fab2433637063dc9d51b2505bb6023c391d606419bc9a0874c131 in / 
# Thu, 30 Sep 2021 18:03:35 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:35:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:35:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d333743b3b21fdfd6ba3f4a0624204b620b72c3d0eb2c3dd9e39d23f3a87e9c`  
		Last Modified: Thu, 30 Sep 2021 18:20:10 GMT  
		Size: 45.9 MB (45917880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d8928e133ca4adc2e7f254a958f120743ac165e45332c8f2713144cf1e1c5`  
		Last Modified: Fri, 01 Oct 2021 05:55:55 GMT  
		Size: 7.1 MB (7124916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a975074459ff1f9c6b99644b138401f840f49a4dc1ef138661e138db9cd00038`  
		Last Modified: Fri, 01 Oct 2021 05:55:56 GMT  
		Size: 9.3 MB (9343736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a11c276eb14e33bd12beadc8185183d0805aee55492c4f89cf581d75ed1b203`  
		Last Modified: Fri, 01 Oct 2021 05:56:40 GMT  
		Size: 47.4 MB (47356508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d9567bd2ccf65136c5af5acded3e7cdeb838531c568ff7a33d5ba1a79469f8d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119070410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fa755f8feca4fb8f1c0c45b89d5998448e31303d2a27657f0f05620996c49f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619d0551980848579ec373733f2fb35c7deddf13e6e56747ddf13dedc6ddbf6b`  
		Last Modified: Tue, 28 Sep 2021 02:26:20 GMT  
		Size: 52.2 MB (52167859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f443841afa6578a2062b06c2d45fbbc181c3c2de553f11d0ac93d9dfc070564d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122985746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e542cc9c79fc3e2ec84798dde3789f0b5fc87f754322e41e7064016e05111cfa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:28 GMT
ADD file:f0e83dd2590d6bd2d3726ebb3ebb5bfc0c2a52fe9feaeecd60b036c8eff69788 in / 
# Tue, 28 Sep 2021 01:40:28 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6f6f4e486b0370ea7bec101a3770e19279a47ffd7d20a9c48000fe3e63917bc`  
		Last Modified: Tue, 28 Sep 2021 01:49:34 GMT  
		Size: 51.2 MB (51207376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcad00d036c37c4de05381481665b986170717ee59000d1a49fa9e0d73ef484`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 8.0 MB (8000034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f546ea183fd0e99a89120a49252894e7056ddf33329190affa0efa1b5de5d929`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 10.3 MB (10340144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b68564816940e410e66659fa680b3832e7c4d11ee4e50beaf82cacad47ea57`  
		Last Modified: Tue, 28 Sep 2021 02:26:52 GMT  
		Size: 53.4 MB (53438192 bytes)  
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
$ docker pull buildpack-deps@sha256:1c8fe95ec981148f1ff039c2319960a221ef986fb127fb37dcae1509e86fda14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130640469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2803b76ec4155b1b5c867fdd64df393b905c116605a8ebf0dd2f213cb99aff17`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:41 GMT
ADD file:1f8eebd902d2881786014a1e5db3cd6f0bab3a55e23befcd6cb6e4d91b9e6d79 in / 
# Fri, 03 Sep 2021 01:23:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:17:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:20ef04c157f9b9866c6408757e7ba2534608600e6cadbb759175572efc03f830`  
		Last Modified: Fri, 03 Sep 2021 01:38:28 GMT  
		Size: 54.2 MB (54182653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6474492bb0f747d1f925e9a2e0ed1d7b0bd0fdaa043e1fb2e892dde4313615`  
		Last Modified: Fri, 03 Sep 2021 07:12:35 GMT  
		Size: 8.3 MB (8272834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e098e859433301d306293ed680efa3bdc7d574613acc0d17fd90c09e854f779`  
		Last Modified: Fri, 03 Sep 2021 07:12:38 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0210891d190261ad1963160b64e1e7e13a3b1e4b1ac8f297c5280432fa730`  
		Last Modified: Fri, 03 Sep 2021 07:13:03 GMT  
		Size: 57.5 MB (57457148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e8a003f034fe144cf84bba783847c2ee4935327acbf51351c152745374668b17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117668874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e805d98391dca367564ea9a17b1e0f8f91f5029a586670ab3629dd1ed0206cbe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:11 GMT
ADD file:9eb47cd6584ec05371051b5cae96c24e6f03e66328173f27a9f30d46b8bce760 in / 
# Tue, 28 Sep 2021 01:43:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:09:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1481e22e2c9526464f32062da733ce595a9491b1e48870f085365fb7f9e8b60c`  
		Last Modified: Tue, 28 Sep 2021 01:49:17 GMT  
		Size: 49.0 MB (49004320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe83b756a24fd473ce558a06ee5b580a63605b4d9d74817e2e1d1289f54fb7f`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 7.4 MB (7400854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ed278d1f7ac1eb211375face0ceb4605c67610e32fce9d7601efdda86b1fc7`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 9.9 MB (9883204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9675b3feffe472a443ef929f8e972471bd03506cf0ad31270751bfaad5feca5d`  
		Last Modified: Tue, 28 Sep 2021 02:16:56 GMT  
		Size: 51.4 MB (51380496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:8f4b29031e8204331606d488fb6290f99bc6ccc7f50623272e1e76a966487520
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
$ docker pull buildpack-deps@sha256:6d3bd0093dc57538be1da3cda96a80f944ab167c2f9fcff321db397d15923754
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70952632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f020ab5dd0cef2c0b20ded3f290546ae4b2a84986d4e02446879a72cf0d1cbd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:151b67336eac36e8c7376d2f603965b3d613b838a8c6c00df65ecb6b81ebb7e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68097369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecfe7b5c5061f7480a7a1a7306e93ea2082b63b6b9d1f29c9b01b70d4ae129e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:96c3837335e336493dd4ec502568a24fb8a0f808d15ed1a844c573d738b99ff4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65267580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feef68d841ccaedfa1bae704efe715b0f162812c549f94539d335e6784b6a512`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d685bcbd37d39eab77c65ae1e04e72d35d3ae193256f074d84a5c87d59842bf2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69629093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990cb9bf14263220789cdd25eb191d564fb567f94c522c1494a07737584426c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d4f08dbf769815a4db9592b6f8911b61ada4280051f115b8b5bf88c9ae6d6e18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72465857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f109721ea809e5ae6fcfd2a47160b846d943350a073e5e431b4bbbf9688d9d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9148b01e8bbfb04fa59f44e2af070eb74a8797213877fc7df3be0467115b9`  
		Last Modified: Tue, 28 Sep 2021 02:24:24 GMT  
		Size: 5.3 MB (5282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda7eaf6b4240f872ceef86fce4f8a87bdad74da3484b9605cb3b2b52cbbf20`  
		Last Modified: Tue, 28 Sep 2021 02:24:25 GMT  
		Size: 11.3 MB (11250636 bytes)  
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
$ docker pull buildpack-deps@sha256:e645211432960dea9563d3ce20b165c647ec21f29d3bc873e80e417076f5b108
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75847150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b9a35d2eb70c2fbc27b4c72a127f42b6b685425398b8ead7a2283f10e32ac5c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:076601aae27650f44b4dbe20132157de742e741af9d5fc796db9032604ab6cf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69100612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73dbb50e50b5a3c5d39455f73ca943eb867aba4106eb831077daf48cee43647a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:aede609912cf5648b0bf72f5e266a0ac6ce81e358ef51330832e33d3ef3806f6
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
$ docker pull buildpack-deps@sha256:fbb84e6535f83fd99ac792ae04a5951548a06772d975566a58cbf2d4b5aa3a23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241790873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dd92b1441e82e0931e46cb77542405e6fa9fc22ef0ad2431f5eab57e3d2f1f8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:06:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:07:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:10:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4774ed347ee7aae0f4029cf9fcdc82fb078d2849f5379c2b3cd0d78fac5608ef`  
		Last Modified: Fri, 01 Oct 2021 03:18:54 GMT  
		Size: 7.8 MB (7770752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f807ec5dd5b51b82a425eb00c21aff5367e6944b5d689b16480bb86b55eeba`  
		Last Modified: Fri, 01 Oct 2021 03:18:53 GMT  
		Size: 3.6 MB (3624639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250b71bd9a093349f8995026b169a3c6ac13ec9deca245d216b4293d68de144`  
		Last Modified: Fri, 01 Oct 2021 03:19:13 GMT  
		Size: 60.7 MB (60718964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6324cfcaab7eb21672073d745766ea088056ec005d6cbf1a733f7ec3aa1c0f5b`  
		Last Modified: Fri, 01 Oct 2021 03:19:43 GMT  
		Size: 141.1 MB (141107604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9234b134ea076c6574d39c3dbe0cde67242fdf2417245afea087c5ef706babb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207217146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2311fdf25f2e903d826aaaa6846da6841c4d1a7b341f5886f8272a1b89ecae8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:20:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:21:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:22:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:23:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ab467c7f452a8e5cb76b5ed3c9cbce43f7cb04f7024c6478ca446f92e399b`  
		Last Modified: Sat, 02 Oct 2021 22:38:21 GMT  
		Size: 6.8 MB (6766828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d36dec707683a0afbc780af0a45ca17744ac7a0f640d578af3195478d90621`  
		Last Modified: Sat, 02 Oct 2021 22:38:18 GMT  
		Size: 3.1 MB (3103932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035a89a55aa2f31698e17865b0d77f83527531ba06367f3a102622156308cc19`  
		Last Modified: Sat, 02 Oct 2021 22:39:13 GMT  
		Size: 55.5 MB (55450855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318206d0235667fb1d2d144a55607944970fa31e7dd0505f9181f42585c87653`  
		Last Modified: Sat, 02 Oct 2021 22:40:36 GMT  
		Size: 117.8 MB (117828313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e90ebfc849475dadd4dbdb12bd6fb07dff77c72547c4dd3135d681b3e302ca04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231928586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b447be8ba7595e18d9b365577069b4e6a6b472eb3e1dfd9dfb2e86f0d35eb5b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:17:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:17:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:18:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689db6ff62963b3e4aae6a2abb554c5d5882b06774174e624ba845094921121b`  
		Last Modified: Fri, 01 Oct 2021 03:25:21 GMT  
		Size: 7.6 MB (7635218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f06ec2d3b194d9726a65c75b82d7339dc700bc20d923f047e02a735a78925`  
		Last Modified: Fri, 01 Oct 2021 03:25:20 GMT  
		Size: 3.6 MB (3600459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab6b6364c13aa6082dc2050a10d5035c25a02706281100e29c0ad568f624b29`  
		Last Modified: Fri, 01 Oct 2021 03:25:43 GMT  
		Size: 60.8 MB (60767677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299cf52c5a3ea41921e5ca4a9a5f00842be4e17c0767d58216a6bcf50d8fa4b5`  
		Last Modified: Fri, 01 Oct 2021 03:26:15 GMT  
		Size: 132.8 MB (132752827 bytes)  
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
$ docker pull buildpack-deps@sha256:80597b385ccb4649fffd750d5dba51880eff9b05435f128142afa465727f9b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222631286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3dbdfb7bb408340ec0b5b0ac6676da0dd3c7139f8422c9992e4ce3aaeb762c3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:34:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:35:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:35:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6fa25b21a93cb1d9a61a6d35cabe2d161b63a3706869aeb57c0df4be4472b4`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 7.4 MB (7427440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a836aa79819738132b60bb1aa2d42907d593dc879d3785ca6afff3f6adda654`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 3.5 MB (3542126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651550a9a41cdd82a572e95f64a221b84cd8e9d72e164544f480714afe537054`  
		Last Modified: Fri, 01 Oct 2021 02:42:21 GMT  
		Size: 60.0 MB (60020560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2ff4661bb90141a8840a1627abe3deede20a3beadc896129a3764974793aa7`  
		Last Modified: Fri, 01 Oct 2021 02:42:44 GMT  
		Size: 124.5 MB (124518250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:4a9add1dae34360ec3f686c6f822a907a5b6490a998fe1d9b297cda065cf3db0
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
$ docker pull buildpack-deps@sha256:696b974b81ccbecfc40803f879228a8259edc1c8b5c098ccefdd1f35437bcfe1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39964305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357a312644cce18c08e5ce216006fa4089442dec9b94fd3c5f84a01df0d9c747`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:06:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4774ed347ee7aae0f4029cf9fcdc82fb078d2849f5379c2b3cd0d78fac5608ef`  
		Last Modified: Fri, 01 Oct 2021 03:18:54 GMT  
		Size: 7.8 MB (7770752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f807ec5dd5b51b82a425eb00c21aff5367e6944b5d689b16480bb86b55eeba`  
		Last Modified: Fri, 01 Oct 2021 03:18:53 GMT  
		Size: 3.6 MB (3624639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:96fc46fd8428121f4cba8731f07c3d2b0477826da21811e89ba2facff69b90c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a44a4a803282848534fb0e2b5a618208d8f0fcfaa6918c8c5021e765bc45ea6c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:20:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:21:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ab467c7f452a8e5cb76b5ed3c9cbce43f7cb04f7024c6478ca446f92e399b`  
		Last Modified: Sat, 02 Oct 2021 22:38:21 GMT  
		Size: 6.8 MB (6766828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d36dec707683a0afbc780af0a45ca17744ac7a0f640d578af3195478d90621`  
		Last Modified: Sat, 02 Oct 2021 22:38:18 GMT  
		Size: 3.1 MB (3103932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2fb36e233ead75cc8b3a9e8a7feaa46b31ce507f9666246b82975f177db2bb7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38408082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da02243d8b4488513cd7351f2ebc075c8db8b4098ee398a79e228a8f2a72b20f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:17:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689db6ff62963b3e4aae6a2abb554c5d5882b06774174e624ba845094921121b`  
		Last Modified: Fri, 01 Oct 2021 03:25:21 GMT  
		Size: 7.6 MB (7635218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f06ec2d3b194d9726a65c75b82d7339dc700bc20d923f047e02a735a78925`  
		Last Modified: Fri, 01 Oct 2021 03:25:20 GMT  
		Size: 3.6 MB (3600459 bytes)  
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
$ docker pull buildpack-deps@sha256:6fc23eff56764bfacf3643338fbed63a7b9a96aa22a7cb7da40e7c2388ca1d73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34119703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3afa654267fc7f48a4a8c50432c7addb0a16401799d27cfab2b9743babcdd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:14:48 GMT
ADD file:a8b9aeb23e8f47568ef8ea33a80fee0c676db7c4c9ec9210abf75217a8f329fb in / 
# Fri, 01 Oct 2021 01:14:49 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:08:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:91a226dd2b609e6bc3e70f7621380def71f05b74e75fa1a2f0421795a8904f10`  
		Last Modified: Fri, 01 Oct 2021 01:37:38 GMT  
		Size: 24.2 MB (24227267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9183300d5640e2467c23128b3e3557a975761a04b458b806535ec6ce8e89ae2f`  
		Last Modified: Fri, 01 Oct 2021 02:49:29 GMT  
		Size: 6.7 MB (6747990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e44b67d1b1ccde3826142f95cdc6cd6e379bbfbeda24c6253df084db75344f`  
		Last Modified: Fri, 01 Oct 2021 02:49:24 GMT  
		Size: 3.1 MB (3144446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b9766200c0f8abda5cc5c3085a6a3c22fb41ee8132e5ead08fa6542aa15e148c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38092476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97ee38d1e83342696caace4f46cf69a402659c84d853a06591a6f59a5503d96`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:34:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6fa25b21a93cb1d9a61a6d35cabe2d161b63a3706869aeb57c0df4be4472b4`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 7.4 MB (7427440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a836aa79819738132b60bb1aa2d42907d593dc879d3785ca6afff3f6adda654`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 3.5 MB (3542126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:4465794cf302f98968f6b677b0a61c97abe78aa1f75135e493c6b614690f6192
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
$ docker pull buildpack-deps@sha256:7ad91f5bc79abd012aa84bf3ae64f626eb7eeb8e711e57f9bd2f163d2eac7de6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100683269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5457e36bff271ad9896846715e324a195c4083d4749034159d0029d47252df`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:06:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:07:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4774ed347ee7aae0f4029cf9fcdc82fb078d2849f5379c2b3cd0d78fac5608ef`  
		Last Modified: Fri, 01 Oct 2021 03:18:54 GMT  
		Size: 7.8 MB (7770752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f807ec5dd5b51b82a425eb00c21aff5367e6944b5d689b16480bb86b55eeba`  
		Last Modified: Fri, 01 Oct 2021 03:18:53 GMT  
		Size: 3.6 MB (3624639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250b71bd9a093349f8995026b169a3c6ac13ec9deca245d216b4293d68de144`  
		Last Modified: Fri, 01 Oct 2021 03:19:13 GMT  
		Size: 60.7 MB (60718964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3a61d944bb68e7c20853916e0ebf65b59600c6691ad38bc20026e8860da4a59c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89388833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768431def83a292eefc32a7aebb536b9aacdd6fb88a516d63ef547131dddadef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:20:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:21:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:22:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ab467c7f452a8e5cb76b5ed3c9cbce43f7cb04f7024c6478ca446f92e399b`  
		Last Modified: Sat, 02 Oct 2021 22:38:21 GMT  
		Size: 6.8 MB (6766828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d36dec707683a0afbc780af0a45ca17744ac7a0f640d578af3195478d90621`  
		Last Modified: Sat, 02 Oct 2021 22:38:18 GMT  
		Size: 3.1 MB (3103932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035a89a55aa2f31698e17865b0d77f83527531ba06367f3a102622156308cc19`  
		Last Modified: Sat, 02 Oct 2021 22:39:13 GMT  
		Size: 55.5 MB (55450855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:696e75f38cfed35972c462e702a6009c506e6e349401bf8287ab1c1a75bc00a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99175759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3c038017047e55e8000b4e31fac47994fdb7740f8bd392338795912c12ca9f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:17:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:17:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689db6ff62963b3e4aae6a2abb554c5d5882b06774174e624ba845094921121b`  
		Last Modified: Fri, 01 Oct 2021 03:25:21 GMT  
		Size: 7.6 MB (7635218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f06ec2d3b194d9726a65c75b82d7339dc700bc20d923f047e02a735a78925`  
		Last Modified: Fri, 01 Oct 2021 03:25:20 GMT  
		Size: 3.6 MB (3600459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab6b6364c13aa6082dc2050a10d5035c25a02706281100e29c0ad568f624b29`  
		Last Modified: Fri, 01 Oct 2021 03:25:43 GMT  
		Size: 60.8 MB (60767677 bytes)  
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
$ docker pull buildpack-deps@sha256:ab12db445536d99cc55a13c70085c271777f232dfbd09ac2056e5c0c7d30350a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98113036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:403e51f1da78f84c9ef754ad1f475ec1078f576d75597b0aa4b8edb22af9801d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:34:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:35:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6fa25b21a93cb1d9a61a6d35cabe2d161b63a3706869aeb57c0df4be4472b4`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 7.4 MB (7427440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a836aa79819738132b60bb1aa2d42907d593dc879d3785ca6afff3f6adda654`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 3.5 MB (3542126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651550a9a41cdd82a572e95f64a221b84cd8e9d72e164544f480714afe537054`  
		Last Modified: Fri, 01 Oct 2021 02:42:21 GMT  
		Size: 60.0 MB (60020560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:hirsute`

```console
$ docker pull buildpack-deps@sha256:b7fce989935172004b910ccbe7a55549cfa21057baac705dfdaa5765933768a7
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
$ docker pull buildpack-deps@sha256:d0b1bc965e6285f5b580fed802c86c2609554e159bce1fbc68420f19c6e8bbc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248825494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab7ad9ebdf1c606e7a98f7ceb37be67b63bb2979f28a43c567471357f6c0479b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:12:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:12:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e61e03c60557bda70bf3cc9a2dd5562bdd9f66442dd9a5b33f393f7f610ca9`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 5.4 MB (5429421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1701598239c3ba301af98cdbdc4c053cff70425e0102d03a0a0a660b68520b35`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 3.7 MB (3662530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bdc834e59f4ded456cfe6c6f10cc62573219101f62812b9e6aa4fcb1724d6d`  
		Last Modified: Fri, 01 Oct 2021 03:20:11 GMT  
		Size: 43.5 MB (43542401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8935876bd7c602a9726de718b80206366568ebdb6230210377b10bf2a0e35d0b`  
		Last Modified: Fri, 01 Oct 2021 03:20:44 GMT  
		Size: 164.5 MB (164486846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6750601f1fd76063f80245bfe8db26d1a96853abfc6dfb02fb16188a458ea329
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.0 MB (208963298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fe4c7546b306b1c82069e56220df647071c462704250c3ea210b3f3e657061`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:24:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:25:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:27:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8944eff0f4815cf5a70868ad5afaed083de9f7ead5a73bc97fa5dc147a04f9`  
		Last Modified: Sat, 02 Oct 2021 22:40:51 GMT  
		Size: 4.9 MB (4858463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bed8cb9d9d7259532d0d30040f4f46ba30d3dedae6e7d37d51c4bf9f60bc54a`  
		Last Modified: Sat, 02 Oct 2021 22:40:50 GMT  
		Size: 3.1 MB (3139002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8efec2f84a292f59a270ac67ccb130692e15a90a3105f135600dd1ee32bed4`  
		Last Modified: Sat, 02 Oct 2021 22:41:32 GMT  
		Size: 40.0 MB (39953431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecfb48b1577ca4abe64edeb74c9898c20c84b004d5bc4a66957c2de97d6af5f`  
		Last Modified: Sat, 02 Oct 2021 22:43:03 GMT  
		Size: 134.2 MB (134152915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b3cfe5018bd7d3a98817ee81a7622ca088182ce526cda8e1ca95f94d12185024
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239588979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f87ff4d2d7f7f612af485bab800828d06486c37417992be439eee282e9a06d4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:18:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:18:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:19:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:19:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22e5e9de7272c5e4544f153bf2aeeb8c118ac5a3ccdea10a7d6a6c996c3575c`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 5.4 MB (5400844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c320e18b5848a613875caa1714ab609c4840c23b41f7eb20a8d3dc34193f53d`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 3.6 MB (3638468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47cb72d2d39bf513d49bbb200478599434e3db9569aef12f56685039732f370`  
		Last Modified: Fri, 01 Oct 2021 03:26:46 GMT  
		Size: 43.5 MB (43526154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78e0bd1f0df4b31c75564b204eafde9e2ed9270dfa01bc2ddb56f50bfef7e3c`  
		Last Modified: Fri, 01 Oct 2021 03:27:21 GMT  
		Size: 156.8 MB (156849350 bytes)  
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
$ docker pull buildpack-deps@sha256:a445bb89dc4ad3e2a546446073c778792b1cf88762d78ac04fd3a8fd9286c6a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.9 MB (257925643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f10e0dd936c1a9ddadab2ba100ffe9ed2f196a160e87e4f254b27baf58e8c693`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:10:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:11:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:20:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747535e5ca63ea5be385acb70aaca4311fe2b78f1e44463cbfce298800f9f33b`  
		Last Modified: Fri, 01 Oct 2021 02:50:40 GMT  
		Size: 4.9 MB (4944581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0facf6815c035133c1d22c89659eabcd14838fa24ff638d7a2f822c2d42d795a`  
		Last Modified: Fri, 01 Oct 2021 02:50:37 GMT  
		Size: 3.2 MB (3177915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f4c1d69caf6add02d4549d216e9e00fdaae087f4d280cea93bbd3f8b3ec48a`  
		Last Modified: Fri, 01 Oct 2021 02:52:36 GMT  
		Size: 40.3 MB (40329415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4eb085d1eb115177f17b87572f40735eff638aa6135e73b357a2e48048b803`  
		Last Modified: Fri, 01 Oct 2021 02:58:07 GMT  
		Size: 182.3 MB (182331851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f27299270693081b87ff3db0f81ca0b487eadf97ab498fd4138daa4bf57b8540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241445352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1baf0cfdef466aacd2bc2dbb6e3ac9fc116c3f801fa511931eab79565035b41`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:36:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:36:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:37:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a99a5951692580021e948472804dab0a010b074b1163b603e4f5cfda6382bf4`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 5.8 MB (5801664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fa544ba88c98b23feadb6ad914d8da1debe080907cb082ad2b8d8046e6c5da`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 4.2 MB (4185318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f556cc2020b283f43fb541b48641c7dd9e20e8d7d40de1a098420d28dbe5b70d`  
		Last Modified: Fri, 01 Oct 2021 02:43:07 GMT  
		Size: 47.4 MB (47399802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b33a1445de22d945dee33648fd8863fb8b89b557a88fdde39b8d2f87fbde44`  
		Last Modified: Fri, 01 Oct 2021 02:43:33 GMT  
		Size: 151.6 MB (151553029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:hirsute-curl`

```console
$ docker pull buildpack-deps@sha256:d9f00aea588cf3f87f60a3ce0c9e17dbb4a13580ef6b7509135dce7072ee15af
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
$ docker pull buildpack-deps@sha256:9061f7ef082ae113348351460f7c072b43192180e25e675fbde68bebab046851
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40796247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e96cc49ca9401fa96ae12c1ffb5e5c840591f3a502977d7bc750b9223e3a4d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:12:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e61e03c60557bda70bf3cc9a2dd5562bdd9f66442dd9a5b33f393f7f610ca9`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 5.4 MB (5429421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1701598239c3ba301af98cdbdc4c053cff70425e0102d03a0a0a660b68520b35`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 3.7 MB (3662530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2d230394b683fdf5e3e856d2c6d7b0c95ab49ce823d7a6c8cf63be67907666a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34856952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe84b73356152b7afd8fc8c78dd430cbfa28f4a3eb076c34c16c26d3579a2c8c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:24:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8944eff0f4815cf5a70868ad5afaed083de9f7ead5a73bc97fa5dc147a04f9`  
		Last Modified: Sat, 02 Oct 2021 22:40:51 GMT  
		Size: 4.9 MB (4858463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bed8cb9d9d7259532d0d30040f4f46ba30d3dedae6e7d37d51c4bf9f60bc54a`  
		Last Modified: Sat, 02 Oct 2021 22:40:50 GMT  
		Size: 3.1 MB (3139002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e97fb51e07261b6a8213a306321408eaab25c98dd81802fa5c3466d01585e297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39213475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea936eb6321870111adf4892e07b9dd6a92b42c9be055e57c581219867d1d64`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:18:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:18:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22e5e9de7272c5e4544f153bf2aeeb8c118ac5a3ccdea10a7d6a6c996c3575c`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 5.4 MB (5400844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c320e18b5848a613875caa1714ab609c4840c23b41f7eb20a8d3dc34193f53d`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 3.6 MB (3638468 bytes)  
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
$ docker pull buildpack-deps@sha256:6f18fc0d3ddcc7a1fc4421df4e73d1bc7c8bfa9bcb096d4d55eef355576c40bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35264377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01fdd529f701fb77c03d0bbb3433871ae8b6285adebd0a80f552a4b1421c913`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:10:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:11:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747535e5ca63ea5be385acb70aaca4311fe2b78f1e44463cbfce298800f9f33b`  
		Last Modified: Fri, 01 Oct 2021 02:50:40 GMT  
		Size: 4.9 MB (4944581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0facf6815c035133c1d22c89659eabcd14838fa24ff638d7a2f822c2d42d795a`  
		Last Modified: Fri, 01 Oct 2021 02:50:37 GMT  
		Size: 3.2 MB (3177915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d4fb0f8ba2a1371a25956f327c4583b4177f6a08669243e2cc644487ef42db54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42492521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769764cfa8002921bd1badc5e585535ccf1ce621970e3950a8757da9733976e3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:36:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:36:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a99a5951692580021e948472804dab0a010b074b1163b603e4f5cfda6382bf4`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 5.8 MB (5801664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fa544ba88c98b23feadb6ad914d8da1debe080907cb082ad2b8d8046e6c5da`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 4.2 MB (4185318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:hirsute-scm`

```console
$ docker pull buildpack-deps@sha256:540342c46d76db22368d7efc404214fac6390ffd4fd3971b2be2b498a251e3bf
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
$ docker pull buildpack-deps@sha256:e4b34d9ecd5c159571e7c4aa5a92e5f59021eae78e6b03e1619fad1216f46a17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.3 MB (84338648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a3cb2eb560e049b85cb7c014a687b3aae9ce86dadd0640b986879a2d7f70cf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:12:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:12:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e61e03c60557bda70bf3cc9a2dd5562bdd9f66442dd9a5b33f393f7f610ca9`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 5.4 MB (5429421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1701598239c3ba301af98cdbdc4c053cff70425e0102d03a0a0a660b68520b35`  
		Last Modified: Fri, 01 Oct 2021 03:19:53 GMT  
		Size: 3.7 MB (3662530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bdc834e59f4ded456cfe6c6f10cc62573219101f62812b9e6aa4fcb1724d6d`  
		Last Modified: Fri, 01 Oct 2021 03:20:11 GMT  
		Size: 43.5 MB (43542401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9804a4fd9b159a2bf14e2e9fecfafd454b98c57b208e9f1cd046c5367321421e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74810383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa57e9ca19a6490459f1d1b27fc9522ba5af6d70e5bf5de22e6d43365e578599`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:24:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:25:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8944eff0f4815cf5a70868ad5afaed083de9f7ead5a73bc97fa5dc147a04f9`  
		Last Modified: Sat, 02 Oct 2021 22:40:51 GMT  
		Size: 4.9 MB (4858463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bed8cb9d9d7259532d0d30040f4f46ba30d3dedae6e7d37d51c4bf9f60bc54a`  
		Last Modified: Sat, 02 Oct 2021 22:40:50 GMT  
		Size: 3.1 MB (3139002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8efec2f84a292f59a270ac67ccb130692e15a90a3105f135600dd1ee32bed4`  
		Last Modified: Sat, 02 Oct 2021 22:41:32 GMT  
		Size: 40.0 MB (39953431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d9446fb751659cac97fe4602a547a07c488b2e551c439846879acfe1d17fd7f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82739629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c6cb7af054be1655c285f42e5dc616e5c700b2145d26cfab1540f6fcf5034dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:18:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:18:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:19:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22e5e9de7272c5e4544f153bf2aeeb8c118ac5a3ccdea10a7d6a6c996c3575c`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 5.4 MB (5400844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c320e18b5848a613875caa1714ab609c4840c23b41f7eb20a8d3dc34193f53d`  
		Last Modified: Fri, 01 Oct 2021 03:26:27 GMT  
		Size: 3.6 MB (3638468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47cb72d2d39bf513d49bbb200478599434e3db9569aef12f56685039732f370`  
		Last Modified: Fri, 01 Oct 2021 03:26:46 GMT  
		Size: 43.5 MB (43526154 bytes)  
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
$ docker pull buildpack-deps@sha256:f65fa8029821604824f633737c48c72f705393e217b105f05b5b0666541fe3d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75593792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b647358b6ce20b1f16ee3cba013956f23773270e2ad5c14a3acf32d1f3d7f1b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:10:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:11:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747535e5ca63ea5be385acb70aaca4311fe2b78f1e44463cbfce298800f9f33b`  
		Last Modified: Fri, 01 Oct 2021 02:50:40 GMT  
		Size: 4.9 MB (4944581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0facf6815c035133c1d22c89659eabcd14838fa24ff638d7a2f822c2d42d795a`  
		Last Modified: Fri, 01 Oct 2021 02:50:37 GMT  
		Size: 3.2 MB (3177915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f4c1d69caf6add02d4549d216e9e00fdaae087f4d280cea93bbd3f8b3ec48a`  
		Last Modified: Fri, 01 Oct 2021 02:52:36 GMT  
		Size: 40.3 MB (40329415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d25b90928f781d816d02bea7d8f54221a35b29730fd84d0a00243b3b8bdb3e73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89892323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f73f0b59e7117c44cb5c0f23df871f926492ee7502ad7028f57ca74fe86c8cae`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:36:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:36:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a99a5951692580021e948472804dab0a010b074b1163b603e4f5cfda6382bf4`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 5.8 MB (5801664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fa544ba88c98b23feadb6ad914d8da1debe080907cb082ad2b8d8046e6c5da`  
		Last Modified: Fri, 01 Oct 2021 02:42:52 GMT  
		Size: 4.2 MB (4185318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f556cc2020b283f43fb541b48641c7dd9e20e8d7d40de1a098420d28dbe5b70d`  
		Last Modified: Fri, 01 Oct 2021 02:43:07 GMT  
		Size: 47.4 MB (47399802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:impish`

```console
$ docker pull buildpack-deps@sha256:7fbd1e542ffae01b709d0aee632c4405890505d79fd7331d8c75c847398e19a0
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
$ docker pull buildpack-deps@sha256:f6678c935da21dcc51c2272f514ae95e68946b6e94206470cfa7e0d3c84f3f33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371066555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f07948a9b90cd3d03abd58a6ebacbaa26c4f20e9a3ce2cd987bd465f4ed3965`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:27:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:28:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:30:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf1a9d4fbdb8bcdea8da245690e0e7b0d7f42cd7b7480dd3f9866881a1da2c`  
		Last Modified: Sat, 02 Oct 2021 22:43:19 GMT  
		Size: 3.4 MB (3448048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfa76bdfd39c414c299c1e02cf75c9b579b3aa69ca8e1abf9eb876765fcc9ab`  
		Last Modified: Sat, 02 Oct 2021 22:43:18 GMT  
		Size: 3.7 MB (3742516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360154fa07ad953713f7e71f7feffabf9f868fa69562aeb598e60ebd881ede16`  
		Last Modified: Sat, 02 Oct 2021 22:43:59 GMT  
		Size: 40.3 MB (40285193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb0c2a0ca1287f5644704ab6ae1dbfd650eeae5b8ce48ee335e46a1a2bd068`  
		Last Modified: Sat, 02 Oct 2021 22:46:58 GMT  
		Size: 296.7 MB (296673806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:173282a68ed3c7d434e0a049630d7ee47e5ff9b0937c87e24de80c41032b44f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.8 MB (399753642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c681f790e2c9ad75fe348a46f94492c9e4e2a4cf1c6e08b36b18048884d41020`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:20:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:21:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e1bb6cc21d9aa99ea2365d91ca737ff33423cf8eef3ac6d444f9264ecf62c`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.7 MB (3680866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44384e90f77381715996a06f1aef553b1ffe6e32cd9f467350b914746ba678eb`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.5 MB (3533741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc1cb90f475d191407aa41ee7d90ffd845371c604e65fedf778556ba48612f`  
		Last Modified: Fri, 01 Oct 2021 03:27:51 GMT  
		Size: 38.0 MB (38028253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fd4f9a27c5ce4d91f6bfc6770ad8a8b894911d0d94e7e683e9c34844be1c22`  
		Last Modified: Fri, 01 Oct 2021 03:28:51 GMT  
		Size: 325.5 MB (325462804 bytes)  
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
$ docker pull buildpack-deps@sha256:4b22a884a0b2e518316ae5bca5a1d25a68152cbcd931d8334e80136baac33ec5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.5 MB (266483053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad71d8370638795c9aa2a2d157409cd2ca60b36e0d78e0577c61ffd4d3c3dbd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:22:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:26:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70e1ff9e0960442ac8e0ed27318b8f50e84d12cbedd17b4f36bfa157115adc7`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.5 MB (3490761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2050b829842e591df4469c3681081a8cf61654b45f11d26e6953e514d6869b93`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.8 MB (3803189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c488cbe594d2cf170d43a86c8cde4efc13bd529cf61fd3b9acb9ff640aa8b617`  
		Last Modified: Fri, 01 Oct 2021 03:01:12 GMT  
		Size: 40.8 MB (40766562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f040e257abcc701d46bbbbe741df280b9aad1f553176cb2cffa3942dcd9f8`  
		Last Modified: Fri, 01 Oct 2021 03:06:53 GMT  
		Size: 191.2 MB (191212371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5d93cb79d0be2d3b6dac44f7bee954e47d7ab6d8d36f720c33ae06bd99f4169d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **368.6 MB (368601732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4cb7d0c0fad2b9c9cc6a8a2ab173d8b458b98e9846a12911c9774f79387c4d6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:37:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:38:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b6878da56179520aa932c74d47a6c136df51a8b1637756607aa579385b2746`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 3.8 MB (3772798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0073edd8de7859cbb99a9c2b5013c571d603c0c9095297840395b0e5e932a`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 4.0 MB (3962742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9b7e9f35321824c609d7b2bb42e9070012f04eaa33b52f09bb9a38035d69b`  
		Last Modified: Fri, 01 Oct 2021 02:43:53 GMT  
		Size: 38.5 MB (38465117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faacb0872b812a99e17e5d5540d296d9b05d9c300e5fdb801f95c6f65f30a5bb`  
		Last Modified: Fri, 01 Oct 2021 02:44:34 GMT  
		Size: 291.6 MB (291631034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:c53ef4db48421b2adf8683f1b54765147b1541a3ee77786cce257a30d7b6618a
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
$ docker pull buildpack-deps@sha256:6f1b35544a0f47df6f3c77730b3abce82ab8f874d64ea57a6318bfe3886ea43c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34107556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65f89e7cb018e5ef861aac53d03ef2134aad620b25c5ba3ae9e97bd532d3afa2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:27:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf1a9d4fbdb8bcdea8da245690e0e7b0d7f42cd7b7480dd3f9866881a1da2c`  
		Last Modified: Sat, 02 Oct 2021 22:43:19 GMT  
		Size: 3.4 MB (3448048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfa76bdfd39c414c299c1e02cf75c9b579b3aa69ca8e1abf9eb876765fcc9ab`  
		Last Modified: Sat, 02 Oct 2021 22:43:18 GMT  
		Size: 3.7 MB (3742516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7704b5aa6e272ae4a82b3c66c9225a8d696accdedfb151a8681c4cdab189613e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36262585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd4a61178d340fd4853667bbd899f1369ee072493c1af28b3ed5e3be47647e15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:20:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e1bb6cc21d9aa99ea2365d91ca737ff33423cf8eef3ac6d444f9264ecf62c`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.7 MB (3680866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44384e90f77381715996a06f1aef553b1ffe6e32cd9f467350b914746ba678eb`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.5 MB (3533741 bytes)  
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
$ docker pull buildpack-deps@sha256:6a154a1ef63633b46544bec5933e9dbe4d3157815ff444ebe0934ebe303649af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34504120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebba9aeb40f4e46a40589114f0d4d5c25be4b7f994275697a4fffce0cc11bb6a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:22:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70e1ff9e0960442ac8e0ed27318b8f50e84d12cbedd17b4f36bfa157115adc7`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.5 MB (3490761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2050b829842e591df4469c3681081a8cf61654b45f11d26e6953e514d6869b93`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.8 MB (3803189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3a462412b2ea7abd320c5cd6f0aa28db8d7e8d792e1e76d9b0fe3be5a140fe34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.5 MB (38505581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28fe7943e40f4cf73087bf161365c6df15f51d6944635b2ea3db8fbb265b8cc6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b6878da56179520aa932c74d47a6c136df51a8b1637756607aa579385b2746`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 3.8 MB (3772798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0073edd8de7859cbb99a9c2b5013c571d603c0c9095297840395b0e5e932a`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 4.0 MB (3962742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:impish-scm`

```console
$ docker pull buildpack-deps@sha256:3277805f61b64f42f04803682a5eaf665546adb4c686e862a908154390d13afe
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
$ docker pull buildpack-deps@sha256:02dfe5f7d0812d54877e010ea6b4e17b3b364a652ddf0a774618e2ac5b340d3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74392749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c35e1202679199aba724b66d88d092b202ce0a720f1fbc4774055a08a40372d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:27:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:28:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf1a9d4fbdb8bcdea8da245690e0e7b0d7f42cd7b7480dd3f9866881a1da2c`  
		Last Modified: Sat, 02 Oct 2021 22:43:19 GMT  
		Size: 3.4 MB (3448048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfa76bdfd39c414c299c1e02cf75c9b579b3aa69ca8e1abf9eb876765fcc9ab`  
		Last Modified: Sat, 02 Oct 2021 22:43:18 GMT  
		Size: 3.7 MB (3742516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360154fa07ad953713f7e71f7feffabf9f868fa69562aeb598e60ebd881ede16`  
		Last Modified: Sat, 02 Oct 2021 22:43:59 GMT  
		Size: 40.3 MB (40285193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c8f600d722b8fef5ba12089908ede3d8e42a8ae5775432fa2c949724d0b39b60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74290838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ffdc048016e92cdb4284d1e4093a42af66850bc50f54b2d70eb68e9e2ddd9e6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:20:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e1bb6cc21d9aa99ea2365d91ca737ff33423cf8eef3ac6d444f9264ecf62c`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.7 MB (3680866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44384e90f77381715996a06f1aef553b1ffe6e32cd9f467350b914746ba678eb`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.5 MB (3533741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc1cb90f475d191407aa41ee7d90ffd845371c604e65fedf778556ba48612f`  
		Last Modified: Fri, 01 Oct 2021 03:27:51 GMT  
		Size: 38.0 MB (38028253 bytes)  
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
$ docker pull buildpack-deps@sha256:ade44386814b1fbd659c00f2a3d39aaf1f5e74fec0ea0a0978930664ac2d0756
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75270682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4655c550ee38a21c24aed852af8cc275584e860f253b1ad2927e749aed931a12`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:22:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:26:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70e1ff9e0960442ac8e0ed27318b8f50e84d12cbedd17b4f36bfa157115adc7`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.5 MB (3490761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2050b829842e591df4469c3681081a8cf61654b45f11d26e6953e514d6869b93`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.8 MB (3803189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c488cbe594d2cf170d43a86c8cde4efc13bd529cf61fd3b9acb9ff640aa8b617`  
		Last Modified: Fri, 01 Oct 2021 03:01:12 GMT  
		Size: 40.8 MB (40766562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ecfa20db4ba0c46a95b9062c544043b189956610ad948cd4c5aea2ab12d6b551
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76970698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd7e97f3e90d1d954fd5d7177fa80b54889084f4747a02d4d86c8892a60f46e1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:37:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b6878da56179520aa932c74d47a6c136df51a8b1637756607aa579385b2746`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 3.8 MB (3772798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0073edd8de7859cbb99a9c2b5013c571d603c0c9095297840395b0e5e932a`  
		Last Modified: Fri, 01 Oct 2021 02:43:41 GMT  
		Size: 4.0 MB (3962742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9b7e9f35321824c609d7b2bb42e9070012f04eaa33b52f09bb9a38035d69b`  
		Last Modified: Fri, 01 Oct 2021 02:43:53 GMT  
		Size: 38.5 MB (38465117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:e54ae211c5b7f7bef56152bd3004a28989c31d88a6a12e104ba91e715194af2a
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
$ docker pull buildpack-deps@sha256:dc426fff2922e74aa6934ccd1df91e1298cb3ccde18c2f1835f12e70f6220371
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (321969341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:714418fd1dff72d98cd2a7fe82a6a4636418db789278fba59735ebda645e9b27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8e6af58ed3a502f0c3c15dce636d9d362a742eb5b67770d0cfcb72f3a9884`  
		Last Modified: Tue, 28 Sep 2021 01:58:51 GMT  
		Size: 196.4 MB (196449829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7123e9831bb45f888b6806417d2dfe1f180e62e19c677b0d09abb7f80c311de8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295057178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6fd0cb97521cc96a0089159a684d52da508f86d751d5ccb9fa131a6b417689`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb5b710639fb53421f19a58b60a1a0cf28eea33da972ad7bcbab6628ed94797`  
		Last Modified: Tue, 28 Sep 2021 03:08:48 GMT  
		Size: 52.3 MB (52318852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff0c2fb11e77b1bab4e3d2c8b9ff79d5a4bfa2a4c81e291370227cdcf5eae2f`  
		Last Modified: Tue, 28 Sep 2021 03:10:48 GMT  
		Size: 174.6 MB (174640957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:337edfa1be8e16858eddd085e94b6742ba6d116a6e3734497043b26664d576a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282490296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d74011c8e2e7e4542e3f3cd14eafdc2eaff461a41a64d1cef541a8c4b30b501`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:32:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beba146f18f8bf327bfc67faba4e70c717e79ccc563c8b535e44e9c14c2edfc`  
		Last Modified: Fri, 01 Oct 2021 05:53:47 GMT  
		Size: 50.3 MB (50328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd4233acc34086e6db32b75d876bd6ea7538de484ea9b48c9ddd1907aa74ca0`  
		Last Modified: Fri, 01 Oct 2021 05:55:36 GMT  
		Size: 166.9 MB (166894450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3609418ae510b339d73ab6f19ba3a82c8e0bdc171f50df8949f0a3735de06667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313636281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a992d40e6a046b86ed17052793e80b837e5266c1a03f3261b2c558ddd77837f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7e4e85949ee45bae139f288bc1cd85a740b408abdefaaba118c4c4626b021e`  
		Last Modified: Tue, 28 Sep 2021 02:25:03 GMT  
		Size: 54.7 MB (54669786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69e7bcc0bc59e0f5c70e40bc8adebeb94f60240a71e7f8add74d8b9146bbc16`  
		Last Modified: Tue, 28 Sep 2021 02:25:44 GMT  
		Size: 189.3 MB (189337402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:777672fe2d3733ca92041d6bf3fe878cb1f5fdacc449e71e2217750a840bcdf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327745828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be8f244a554fc912c1932f609263329ff9b3d7bcabed8cb7ed0d6d657f5787f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9148b01e8bbfb04fa59f44e2af070eb74a8797213877fc7df3be0467115b9`  
		Last Modified: Tue, 28 Sep 2021 02:24:24 GMT  
		Size: 5.3 MB (5282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda7eaf6b4240f872ceef86fce4f8a87bdad74da3484b9605cb3b2b52cbbf20`  
		Last Modified: Tue, 28 Sep 2021 02:24:25 GMT  
		Size: 11.3 MB (11250636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50bcbe9fc6f4b839121363d75b4325536a717823ee2b2881b0247afe12fd6909`  
		Last Modified: Tue, 28 Sep 2021 02:24:58 GMT  
		Size: 55.9 MB (55916372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3de1989e93fff2054295962d5bbfbfb11bfa4533ad691aaa17c9a52e3a8a22b`  
		Last Modified: Tue, 28 Sep 2021 02:26:07 GMT  
		Size: 199.4 MB (199363599 bytes)  
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
$ docker pull buildpack-deps@sha256:decae382d4f56e845e9800f3b79f315daccccfb47340e44c9f09f0310e8b98d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330495335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c4c1fd57c37be3803887ab8eee646176344caa36226b3c0131b4cd932867afd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 05:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:13:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708d04ed929be54f33cfa94416648dcac9edd8c01746ecc6e250ce046aa54ac0`  
		Last Modified: Fri, 03 Sep 2021 07:09:38 GMT  
		Size: 58.8 MB (58849139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287624e1f6e58d3860703363b792d02bb699c973abd9dadfa2db8495b51ceb93`  
		Last Modified: Fri, 03 Sep 2021 07:12:15 GMT  
		Size: 195.8 MB (195799046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:51e14eaab3cc2825279677ba4a729da747e7686e4de1df8f933005cf8f8bc13b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295585571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa2779752696eb6bfd10f0076125e41a51fad44a72ed6a636d376f337c439375`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:08:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:08:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f5b44618c39b6606db01fa6d460b6b7e1415b3a9c5a0b2f8b179c9b2c3fcfe`  
		Last Modified: Tue, 28 Sep 2021 02:16:05 GMT  
		Size: 54.0 MB (54049595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6589c0454003c1deeaf24f87ae908e9816d7cb9a945148cf89e75038aba3c8`  
		Last Modified: Tue, 28 Sep 2021 02:16:32 GMT  
		Size: 172.4 MB (172435364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:57d5d14748554b31c75a2e95e63c51e8cdfb24393e33c1431982123b7d0c2280
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
$ docker pull buildpack-deps@sha256:2b296bf57a668992a939c1ec7142f5988a567efef9697b95b16feb7259883bcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.2 MB (325213629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44762cca409b0b11184b876627c74da895f48b6035cf6876eeb55505ae5cf300`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:56:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fee6a1847b07f4933116726f66b9218dde8c59d1f7b94de92f9f0683571a362`  
		Last Modified: Tue, 28 Sep 2021 02:01:42 GMT  
		Size: 49.8 MB (49761752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cce3519052443b6eb66426edcfd7b395d8b97913e15256b77924964e8e6291`  
		Last Modified: Tue, 28 Sep 2021 02:02:22 GMT  
		Size: 214.4 MB (214431930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ef3ae3980658ba40e4a7d978df8752ee3c378406892f6b43418c56a6d6e7dc23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309141024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b006505cf9416d4acaf813ebff5a91b4d95ea360736beb0b6c213465a61fdd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:05 GMT
ADD file:f294a28ee9da17e8a289348f6b85aa865b9f1925aebadee96124e1d4a81c8401 in / 
# Tue, 28 Sep 2021 01:56:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 03:01:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:01:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:05:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a237f80116468b0593b0195bd02cdb78fb8bea8e44f206ec86fd61a9377d7a06`  
		Last Modified: Tue, 28 Sep 2021 02:13:48 GMT  
		Size: 44.1 MB (44091934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ebbdc0a8d4cc096a5c44b4a13000717d6e8dfeb21442b4b375e5d1b9327935`  
		Last Modified: Tue, 28 Sep 2021 03:17:12 GMT  
		Size: 10.4 MB (10350664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa304c7ee32783cf53bf48ea782d989a9874bd108e27ddae6d1adfb8b2eb3f`  
		Last Modified: Tue, 28 Sep 2021 03:17:09 GMT  
		Size: 4.2 MB (4161453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e7d03d992607295ece45259f5362cdffa8e3620933d03ee8100e7b58f2ced9`  
		Last Modified: Tue, 28 Sep 2021 03:17:59 GMT  
		Size: 48.0 MB (47984206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b03b8461331cb46d4d7d615cb7070035da816499bb75244a0b92e0c380dc2`  
		Last Modified: Tue, 28 Sep 2021 03:20:12 GMT  
		Size: 202.6 MB (202552767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7b8e69331b0f73e2b60e38a8cc2ac0918ed47b74b0c31b042fa9a56ebb89aa9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.2 MB (297172181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28f85dbdcf266bfca7d7f5f0acbce80a8946aeff5603bf47a8a765c08f73b697`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:46:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a914caeb151e7903d0d778c1ae44d420945c84af10ba750a5abfda6b9a99f65`  
		Last Modified: Fri, 01 Oct 2021 06:02:16 GMT  
		Size: 46.1 MB (46125924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed5634f1108d505f7a942e1c9e9129321f15004050ed21d2bf392b54e802feb`  
		Last Modified: Fri, 01 Oct 2021 06:04:17 GMT  
		Size: 195.0 MB (195049802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f5181b80a371eb18c642363bf22573aa28f809712d3eb9d52fdd8cd73b497a5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (306986243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9ca4a29cf7dc0349ab14654efaedcd290d15587838b9d2f6d7a5607be0625d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:21:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65cdaa18192aee6f9c254882a3a7f4e57f28681ee263e9fd155fefcd6d9a7e7f`  
		Last Modified: Tue, 28 Sep 2021 02:28:40 GMT  
		Size: 47.7 MB (47737758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445c016c41e0197a8c0587a7bdc804370e31412e49c9bd80ba6baa0b67074d1c`  
		Last Modified: Tue, 28 Sep 2021 02:29:20 GMT  
		Size: 201.8 MB (201758610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bb880314f7580d50f63ff28c7e3c47e3a1fd1b79cd10885c4280d567a8bd7a8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332749683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c905aaccf431950e830a05cc74895c752a57081f68d45d5dc7657bca959b1f3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:20 GMT
ADD file:489732b99c09023c7c1cf27548ad2ed82fd8c8411b95a4e155ebcae7546e563e in / 
# Tue, 28 Sep 2021 01:43:21 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:19:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:19:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:21:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:436d1bdb32419bd787d72deddc5b6a490ad25f93d42a585923767fae7698cb58`  
		Last Modified: Tue, 28 Sep 2021 01:53:31 GMT  
		Size: 46.1 MB (46097052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f065d2d31786c9f8f0c16da4c76f7636dd71179a92f3ee06802d878377006`  
		Last Modified: Tue, 28 Sep 2021 02:29:48 GMT  
		Size: 11.4 MB (11356018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eefa63906ef252cd12ee512cc28f58ea12d2b0854ad1f13b11af78ea5faff7d`  
		Last Modified: Tue, 28 Sep 2021 02:29:46 GMT  
		Size: 4.6 MB (4565007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2732564fa295ede3b01575a13f6d43177972b7e85de3a1f4f41866c7d611c04`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.3 MB (51265101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff272836df0bfc90314e2f8fb0eb0085d5ed17686bb6bcd7479e69073cabade0`  
		Last Modified: Tue, 28 Sep 2021 02:31:23 GMT  
		Size: 219.5 MB (219466505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:8c1faeb579deafbc6a453a0ccf4788be816da27ddd3f09bc7c63fddd1811172d
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
$ docker pull buildpack-deps@sha256:7f14fa6118ddab254eb9584f9d6464f97308059eef313f8aa2d9332de370f6e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61019947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026f5a52486111dfd84569e20d902d7cb134f2239af648ee071cef3502b4a2f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9bfdf437f588dd9ff11dd21891f40d3b70cf9cb234f71da1f7f6cd735ed586d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58604051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4c90ab387c8c56dbfafed822b87fe3193450d8635bd0c9247cb4500cea0030`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:05 GMT
ADD file:f294a28ee9da17e8a289348f6b85aa865b9f1925aebadee96124e1d4a81c8401 in / 
# Tue, 28 Sep 2021 01:56:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 03:01:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:01:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a237f80116468b0593b0195bd02cdb78fb8bea8e44f206ec86fd61a9377d7a06`  
		Last Modified: Tue, 28 Sep 2021 02:13:48 GMT  
		Size: 44.1 MB (44091934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ebbdc0a8d4cc096a5c44b4a13000717d6e8dfeb21442b4b375e5d1b9327935`  
		Last Modified: Tue, 28 Sep 2021 03:17:12 GMT  
		Size: 10.4 MB (10350664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa304c7ee32783cf53bf48ea782d989a9874bd108e27ddae6d1adfb8b2eb3f`  
		Last Modified: Tue, 28 Sep 2021 03:17:09 GMT  
		Size: 4.2 MB (4161453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:caea6201c9ee83e004d3dc8ac457f9d6029f0fe6a70188e5d719188022c4f519
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55996455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c023407259091d6cc756cfbdf78d84a1f5476a85ac967e8c55457a244eb9a824`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:954e54995ba061f8f12a7b1c5a3d352e8445cb1379b5dee8e3b61aead89ba056
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57489875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:410f50617ef6056fa47e2f6f85769a3ea11e18612c2e00c549e7eb7f5a75651e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:46ef012bbfc060f6c02c30dab11fbff22c64146722df2452c42c2d31ac5afc26
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62018077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd9a8ed29e31095fa7217eb4a4f4bced6b0f3751904e15d227fb5c9b7dff8083`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:20 GMT
ADD file:489732b99c09023c7c1cf27548ad2ed82fd8c8411b95a4e155ebcae7546e563e in / 
# Tue, 28 Sep 2021 01:43:21 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:19:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:19:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:436d1bdb32419bd787d72deddc5b6a490ad25f93d42a585923767fae7698cb58`  
		Last Modified: Tue, 28 Sep 2021 01:53:31 GMT  
		Size: 46.1 MB (46097052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f065d2d31786c9f8f0c16da4c76f7636dd71179a92f3ee06802d878377006`  
		Last Modified: Tue, 28 Sep 2021 02:29:48 GMT  
		Size: 11.4 MB (11356018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eefa63906ef252cd12ee512cc28f58ea12d2b0854ad1f13b11af78ea5faff7d`  
		Last Modified: Tue, 28 Sep 2021 02:29:46 GMT  
		Size: 4.6 MB (4565007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:1da383fbe3812219a3b9632c5c973b9ad46c6b560b45ded8c101352f886f6668
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
$ docker pull buildpack-deps@sha256:e042672f1de31e5ecc5bbf7df2a9eac7d1cc012a5a620ec3b0b5aa0ccae9e610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110781699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49daeb05d0974f360f43581a6691f08a5b169f1813fcc867a41293f40e7e4b5e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fee6a1847b07f4933116726f66b9218dde8c59d1f7b94de92f9f0683571a362`  
		Last Modified: Tue, 28 Sep 2021 02:01:42 GMT  
		Size: 49.8 MB (49761752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6a816944d99fd57824326754aafd407ee856c330276eb41194f40c7ad02ada82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106588257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf701630150bd83ffd677ef202986223117afacb24dc86cc90592ff66cefd33c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:05 GMT
ADD file:f294a28ee9da17e8a289348f6b85aa865b9f1925aebadee96124e1d4a81c8401 in / 
# Tue, 28 Sep 2021 01:56:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 03:01:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:01:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a237f80116468b0593b0195bd02cdb78fb8bea8e44f206ec86fd61a9377d7a06`  
		Last Modified: Tue, 28 Sep 2021 02:13:48 GMT  
		Size: 44.1 MB (44091934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ebbdc0a8d4cc096a5c44b4a13000717d6e8dfeb21442b4b375e5d1b9327935`  
		Last Modified: Tue, 28 Sep 2021 03:17:12 GMT  
		Size: 10.4 MB (10350664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa304c7ee32783cf53bf48ea782d989a9874bd108e27ddae6d1adfb8b2eb3f`  
		Last Modified: Tue, 28 Sep 2021 03:17:09 GMT  
		Size: 4.2 MB (4161453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e7d03d992607295ece45259f5362cdffa8e3620933d03ee8100e7b58f2ced9`  
		Last Modified: Tue, 28 Sep 2021 03:17:59 GMT  
		Size: 48.0 MB (47984206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2e3b13a826fc616ef225b08428059bbbe6fad1d52fab5bca1ed3745152a47070
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102122379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aafc37f0496b761630fecaf39bbcfd07af95e1926751d29862b817689908995d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a914caeb151e7903d0d778c1ae44d420945c84af10ba750a5abfda6b9a99f65`  
		Last Modified: Fri, 01 Oct 2021 06:02:16 GMT  
		Size: 46.1 MB (46125924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6e23d628f55e994db76f3e661ac0277e87952033aed50ecd98e038faafcbded3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105227633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6830661eeccc11f315c1e747ec4620621a116593bacb767fb179bc3631083db5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65cdaa18192aee6f9c254882a3a7f4e57f28681ee263e9fd155fefcd6d9a7e7f`  
		Last Modified: Tue, 28 Sep 2021 02:28:40 GMT  
		Size: 47.7 MB (47737758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6cb79acdbec5f1e26f1db9e369abbf339d784ba8355d2a264afbd67e67b31827
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113283178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9f8abca0902dbb9750099b01bf8c9f575e4a474a26ee4c4d5c24afc4bc20a7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:20 GMT
ADD file:489732b99c09023c7c1cf27548ad2ed82fd8c8411b95a4e155ebcae7546e563e in / 
# Tue, 28 Sep 2021 01:43:21 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:19:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:19:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:436d1bdb32419bd787d72deddc5b6a490ad25f93d42a585923767fae7698cb58`  
		Last Modified: Tue, 28 Sep 2021 01:53:31 GMT  
		Size: 46.1 MB (46097052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f065d2d31786c9f8f0c16da4c76f7636dd71179a92f3ee06802d878377006`  
		Last Modified: Tue, 28 Sep 2021 02:29:48 GMT  
		Size: 11.4 MB (11356018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eefa63906ef252cd12ee512cc28f58ea12d2b0854ad1f13b11af78ea5faff7d`  
		Last Modified: Tue, 28 Sep 2021 02:29:46 GMT  
		Size: 4.6 MB (4565007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2732564fa295ede3b01575a13f6d43177972b7e85de3a1f4f41866c7d611c04`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.3 MB (51265101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:df00248c216c6ee635cfe9ab3ef070aadd0a58d5ac3da08ed2e4273d4800e54d
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
$ docker pull buildpack-deps@sha256:a8b925ea43a7c8274883997d8d99f17e04a538f4341922bf932e568159e77792
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312503548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83822a8b0862d52f928785e1b80bcb435ba149468c258ffc02f097a8328f717c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:52:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4689f0588c1ba01108f5c6d33943d3d542ae339fd526390d07c7a00ded6473`  
		Last Modified: Tue, 28 Sep 2021 02:00:03 GMT  
		Size: 192.4 MB (192395236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cb5619367c2bf980f5783130cb7d9980a7d349cb5cc1812120b21cdc6ffddfdb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286124998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c41bb4eeaabaad7b56074bae8da8102422bde45f973b2122d9133d93ab014a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:08 GMT
ADD file:f4b6a4e04436efee878ec0804c89afd419015b881385db438e7374e421f7609f in / 
# Tue, 28 Sep 2021 01:51:09 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:52:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:52:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:56:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:860bc9b218abb92e3ca4715f45696ea7ad7927f9c74dfc2d5ab04672145effb2`  
		Last Modified: Tue, 28 Sep 2021 02:07:23 GMT  
		Size: 48.2 MB (48153768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a08133922bd88680cb57f3f77cf4659368c851186070f4bde20308826e0e1`  
		Last Modified: Tue, 28 Sep 2021 03:11:09 GMT  
		Size: 7.4 MB (7376971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a684cac2ccf5e45585c1c543d29c97343bdc822cfe2771bef89eec53404dfe3`  
		Last Modified: Tue, 28 Sep 2021 03:11:10 GMT  
		Size: 9.7 MB (9687508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d864b5875ad7a90124a6af2aa184ef6d85c03e202f11334ee9801d1f33f723d7`  
		Last Modified: Tue, 28 Sep 2021 03:11:56 GMT  
		Size: 49.6 MB (49575651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e43481adfc889d8fe3a14c88589e95ac235c7d707521011521cf627d755b5c5`  
		Last Modified: Tue, 28 Sep 2021 03:13:51 GMT  
		Size: 171.3 MB (171331100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:86a29bffda8650549c1ec9c5ea4561d583afd59ff450fceffd9f33aa37a4f318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278335461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b011fe4ff66214904a51adbf9f81990a976446dc90b77a373eea263f4cc173b6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:34 GMT
ADD file:da3730d9c05fab2433637063dc9d51b2505bb6023c391d606419bc9a0874c131 in / 
# Thu, 30 Sep 2021 18:03:35 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:35:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:35:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:38:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d333743b3b21fdfd6ba3f4a0624204b620b72c3d0eb2c3dd9e39d23f3a87e9c`  
		Last Modified: Thu, 30 Sep 2021 18:20:10 GMT  
		Size: 45.9 MB (45917880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d8928e133ca4adc2e7f254a958f120743ac165e45332c8f2713144cf1e1c5`  
		Last Modified: Fri, 01 Oct 2021 05:55:55 GMT  
		Size: 7.1 MB (7124916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a975074459ff1f9c6b99644b138401f840f49a4dc1ef138661e138db9cd00038`  
		Last Modified: Fri, 01 Oct 2021 05:55:56 GMT  
		Size: 9.3 MB (9343736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a11c276eb14e33bd12beadc8185183d0805aee55492c4f89cf581d75ed1b203`  
		Last Modified: Fri, 01 Oct 2021 05:56:40 GMT  
		Size: 47.4 MB (47356508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee394d962f6e270a45df67b6ef4d987de06705c8153be2c5302e564b810af80e`  
		Last Modified: Fri, 01 Oct 2021 05:58:23 GMT  
		Size: 168.6 MB (168592421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37f7f9b7c6198c73db5e169b3bbace227726da55023379ade00652a258056d3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (303046386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb4108496fbc1d39b4a0ff45e7eeda902949c41b35102034c821e37329d5374c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619d0551980848579ec373733f2fb35c7deddf13e6e56747ddf13dedc6ddbf6b`  
		Last Modified: Tue, 28 Sep 2021 02:26:20 GMT  
		Size: 52.2 MB (52167859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2577d89b67b3c6b82eba3af07fcab6fb023276c144328ee678f9ef6cc14d174f`  
		Last Modified: Tue, 28 Sep 2021 02:26:57 GMT  
		Size: 184.0 MB (183975976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7114ff8bb18a281e793d91a8769338f67b1e7a43c815ca8541ec569688236589
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321917223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d3efff9249d5395fa5f207bff8d4204af1201dd7f77de39ca8f554cf61d58c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:28 GMT
ADD file:f0e83dd2590d6bd2d3726ebb3ebb5bfc0c2a52fe9feaeecd60b036c8eff69788 in / 
# Tue, 28 Sep 2021 01:40:28 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6f6f4e486b0370ea7bec101a3770e19279a47ffd7d20a9c48000fe3e63917bc`  
		Last Modified: Tue, 28 Sep 2021 01:49:34 GMT  
		Size: 51.2 MB (51207376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcad00d036c37c4de05381481665b986170717ee59000d1a49fa9e0d73ef484`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 8.0 MB (8000034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f546ea183fd0e99a89120a49252894e7056ddf33329190affa0efa1b5de5d929`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 10.3 MB (10340144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b68564816940e410e66659fa680b3832e7c4d11ee4e50beaf82cacad47ea57`  
		Last Modified: Tue, 28 Sep 2021 02:26:52 GMT  
		Size: 53.4 MB (53438192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60d099a705a23b8d0a57ed92ee5a3d6d96aca2e11c16c06dda6e309641a1a0f`  
		Last Modified: Tue, 28 Sep 2021 02:27:46 GMT  
		Size: 198.9 MB (198931477 bytes)  
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
$ docker pull buildpack-deps@sha256:5368ed059494735fb5715f20cc76c3167ddb776165acde462451e82148dcd4b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333924815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fba6d1a245467d4791c8fdd942cb667cd733fa9d04603f955d2a1b4e47e6a1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:41 GMT
ADD file:1f8eebd902d2881786014a1e5db3cd6f0bab3a55e23befcd6cb6e4d91b9e6d79 in / 
# Fri, 03 Sep 2021 01:23:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:17:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:42:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:20ef04c157f9b9866c6408757e7ba2534608600e6cadbb759175572efc03f830`  
		Last Modified: Fri, 03 Sep 2021 01:38:28 GMT  
		Size: 54.2 MB (54182653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6474492bb0f747d1f925e9a2e0ed1d7b0bd0fdaa043e1fb2e892dde4313615`  
		Last Modified: Fri, 03 Sep 2021 07:12:35 GMT  
		Size: 8.3 MB (8272834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e098e859433301d306293ed680efa3bdc7d574613acc0d17fd90c09e854f779`  
		Last Modified: Fri, 03 Sep 2021 07:12:38 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0210891d190261ad1963160b64e1e7e13a3b1e4b1ac8f297c5280432fa730`  
		Last Modified: Fri, 03 Sep 2021 07:13:03 GMT  
		Size: 57.5 MB (57457148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a2531ea29e5d6a6e910840570189332f132c3c99c3ca0ce21f40c4311be87`  
		Last Modified: Fri, 03 Sep 2021 07:13:52 GMT  
		Size: 203.3 MB (203284346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:de1ca69c22fd69b717ca75b737f12832a22bd0b4a11ca5a232c08569d2486ac8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294546359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c6959dfb787c69963ab5d333eb3409ae0add59a3b30b7b078345761c3c3132`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:11 GMT
ADD file:9eb47cd6584ec05371051b5cae96c24e6f03e66328173f27a9f30d46b8bce760 in / 
# Tue, 28 Sep 2021 01:43:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:09:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:10:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1481e22e2c9526464f32062da733ce595a9491b1e48870f085365fb7f9e8b60c`  
		Last Modified: Tue, 28 Sep 2021 01:49:17 GMT  
		Size: 49.0 MB (49004320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe83b756a24fd473ce558a06ee5b580a63605b4d9d74817e2e1d1289f54fb7f`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 7.4 MB (7400854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ed278d1f7ac1eb211375face0ceb4605c67610e32fce9d7601efdda86b1fc7`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 9.9 MB (9883204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9675b3feffe472a443ef929f8e972471bd03506cf0ad31270751bfaad5feca5d`  
		Last Modified: Tue, 28 Sep 2021 02:16:56 GMT  
		Size: 51.4 MB (51380496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36130191b2129cf0a0e3c1befece18304ff6e2ad271d3d2a846b4bcb4fbea3fb`  
		Last Modified: Tue, 28 Sep 2021 02:17:23 GMT  
		Size: 176.9 MB (176877485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:207f50e59fabb88d78c4176003fe96ac785480475b5cfe356ef8808abd41701d
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
$ docker pull buildpack-deps@sha256:edb926861a9d4f502a93284830ab70dd511f10dba22d427145e7cef74971a4bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68267001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd96ac6c32156cf1a1c658177b9a3ee1c76550262bb5f66ea623755636e8df5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:614551a10c9ad7fccd0189f174cbf1fb15ea6db182f9158bcb7d472e7d0ec87c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65218247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d956c4cef36a85f57f008f68da4d1e02c289909cd4607c52fe1bcfe63079b6a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:08 GMT
ADD file:f4b6a4e04436efee878ec0804c89afd419015b881385db438e7374e421f7609f in / 
# Tue, 28 Sep 2021 01:51:09 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:52:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:52:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:860bc9b218abb92e3ca4715f45696ea7ad7927f9c74dfc2d5ab04672145effb2`  
		Last Modified: Tue, 28 Sep 2021 02:07:23 GMT  
		Size: 48.2 MB (48153768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a08133922bd88680cb57f3f77cf4659368c851186070f4bde20308826e0e1`  
		Last Modified: Tue, 28 Sep 2021 03:11:09 GMT  
		Size: 7.4 MB (7376971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a684cac2ccf5e45585c1c543d29c97343bdc822cfe2771bef89eec53404dfe3`  
		Last Modified: Tue, 28 Sep 2021 03:11:10 GMT  
		Size: 9.7 MB (9687508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f6bf363f70c4023252f05afb24e47707d679a7228fa239d8cab73aa597b22b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62386532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5a3989375ad180ece61400975a554ee45480a60a4f7f27a3815e180bc6edf6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:34 GMT
ADD file:da3730d9c05fab2433637063dc9d51b2505bb6023c391d606419bc9a0874c131 in / 
# Thu, 30 Sep 2021 18:03:35 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:35:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:35:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2d333743b3b21fdfd6ba3f4a0624204b620b72c3d0eb2c3dd9e39d23f3a87e9c`  
		Last Modified: Thu, 30 Sep 2021 18:20:10 GMT  
		Size: 45.9 MB (45917880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d8928e133ca4adc2e7f254a958f120743ac165e45332c8f2713144cf1e1c5`  
		Last Modified: Fri, 01 Oct 2021 05:55:55 GMT  
		Size: 7.1 MB (7124916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a975074459ff1f9c6b99644b138401f840f49a4dc1ef138661e138db9cd00038`  
		Last Modified: Fri, 01 Oct 2021 05:55:56 GMT  
		Size: 9.3 MB (9343736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2616077fc9c85155a8638e3e522d8f64954d4729c41f266ab5c08725865e3863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66902551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd63debe5398b56ac201dd8e696edba5a4ebfbc032935e65f2a77a0697f1785f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bd063e941f2bd56c9767dc264c9725a8aad4b1cb540589077951538b80e08cd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69547554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8221d1cae77e18f41dcecbcf9a45df7f68f7964a3fcd54081714b98ea6f1b9db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:28 GMT
ADD file:f0e83dd2590d6bd2d3726ebb3ebb5bfc0c2a52fe9feaeecd60b036c8eff69788 in / 
# Tue, 28 Sep 2021 01:40:28 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6f6f4e486b0370ea7bec101a3770e19279a47ffd7d20a9c48000fe3e63917bc`  
		Last Modified: Tue, 28 Sep 2021 01:49:34 GMT  
		Size: 51.2 MB (51207376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcad00d036c37c4de05381481665b986170717ee59000d1a49fa9e0d73ef484`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 8.0 MB (8000034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f546ea183fd0e99a89120a49252894e7056ddf33329190affa0efa1b5de5d929`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 10.3 MB (10340144 bytes)  
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
$ docker pull buildpack-deps@sha256:06acd573d66fccb4d006a69d7299464eade5f43cf3257765ff58cfdd52e9c505
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73183321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7c2ade806dee7826b8dc1619005e756a05fc525d79818df01e1bd6779cb8b15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:41 GMT
ADD file:1f8eebd902d2881786014a1e5db3cd6f0bab3a55e23befcd6cb6e4d91b9e6d79 in / 
# Fri, 03 Sep 2021 01:23:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:17:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:20ef04c157f9b9866c6408757e7ba2534608600e6cadbb759175572efc03f830`  
		Last Modified: Fri, 03 Sep 2021 01:38:28 GMT  
		Size: 54.2 MB (54182653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6474492bb0f747d1f925e9a2e0ed1d7b0bd0fdaa043e1fb2e892dde4313615`  
		Last Modified: Fri, 03 Sep 2021 07:12:35 GMT  
		Size: 8.3 MB (8272834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e098e859433301d306293ed680efa3bdc7d574613acc0d17fd90c09e854f779`  
		Last Modified: Fri, 03 Sep 2021 07:12:38 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a0a905bf7ea807b467faf44795dd9bc40297712a3c86f2f4871bc6e031a23f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66288378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7636bb61ce8f549e8684021e135baf9a7a29dfb066c765ef9068fc2e83ac9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:11 GMT
ADD file:9eb47cd6584ec05371051b5cae96c24e6f03e66328173f27a9f30d46b8bce760 in / 
# Tue, 28 Sep 2021 01:43:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:09:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1481e22e2c9526464f32062da733ce595a9491b1e48870f085365fb7f9e8b60c`  
		Last Modified: Tue, 28 Sep 2021 01:49:17 GMT  
		Size: 49.0 MB (49004320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe83b756a24fd473ce558a06ee5b580a63605b4d9d74817e2e1d1289f54fb7f`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 7.4 MB (7400854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ed278d1f7ac1eb211375face0ceb4605c67610e32fce9d7601efdda86b1fc7`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 9.9 MB (9883204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:058827d111a2b33f792842da87bc23c3d158cbb1d8136296a2207890d374c640
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
$ docker pull buildpack-deps@sha256:67148e57c764d3a2c77564eb20f0bb6962c638e6f6466bf95acdacba0767f308
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120108312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9dc095a964929680f2a54eed2cb176fc1d653e640e643055e1f3cb1ed4d2636`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:38ee065e9b6ab25e9c6982fbbb963624343bd3f535f29bdea9904a8de690f9fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114793898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18f8633cc1c6c59527e9f5187fe319343106249601e7853ad38af3bee6a2869`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:08 GMT
ADD file:f4b6a4e04436efee878ec0804c89afd419015b881385db438e7374e421f7609f in / 
# Tue, 28 Sep 2021 01:51:09 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:52:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:52:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:53:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:860bc9b218abb92e3ca4715f45696ea7ad7927f9c74dfc2d5ab04672145effb2`  
		Last Modified: Tue, 28 Sep 2021 02:07:23 GMT  
		Size: 48.2 MB (48153768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a08133922bd88680cb57f3f77cf4659368c851186070f4bde20308826e0e1`  
		Last Modified: Tue, 28 Sep 2021 03:11:09 GMT  
		Size: 7.4 MB (7376971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a684cac2ccf5e45585c1c543d29c97343bdc822cfe2771bef89eec53404dfe3`  
		Last Modified: Tue, 28 Sep 2021 03:11:10 GMT  
		Size: 9.7 MB (9687508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d864b5875ad7a90124a6af2aa184ef6d85c03e202f11334ee9801d1f33f723d7`  
		Last Modified: Tue, 28 Sep 2021 03:11:56 GMT  
		Size: 49.6 MB (49575651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:524f675f694d3c2ecebf0781610fb0ff3e9095192bacf31a0306c7d10ba6c006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109743040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e42e135b01508bd6da66e6686e929d2ed404d2eafeceb8d40e88e23eafef828`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:34 GMT
ADD file:da3730d9c05fab2433637063dc9d51b2505bb6023c391d606419bc9a0874c131 in / 
# Thu, 30 Sep 2021 18:03:35 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:35:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:35:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d333743b3b21fdfd6ba3f4a0624204b620b72c3d0eb2c3dd9e39d23f3a87e9c`  
		Last Modified: Thu, 30 Sep 2021 18:20:10 GMT  
		Size: 45.9 MB (45917880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d8928e133ca4adc2e7f254a958f120743ac165e45332c8f2713144cf1e1c5`  
		Last Modified: Fri, 01 Oct 2021 05:55:55 GMT  
		Size: 7.1 MB (7124916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a975074459ff1f9c6b99644b138401f840f49a4dc1ef138661e138db9cd00038`  
		Last Modified: Fri, 01 Oct 2021 05:55:56 GMT  
		Size: 9.3 MB (9343736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a11c276eb14e33bd12beadc8185183d0805aee55492c4f89cf581d75ed1b203`  
		Last Modified: Fri, 01 Oct 2021 05:56:40 GMT  
		Size: 47.4 MB (47356508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d9567bd2ccf65136c5af5acded3e7cdeb838531c568ff7a33d5ba1a79469f8d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119070410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fa755f8feca4fb8f1c0c45b89d5998448e31303d2a27657f0f05620996c49f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619d0551980848579ec373733f2fb35c7deddf13e6e56747ddf13dedc6ddbf6b`  
		Last Modified: Tue, 28 Sep 2021 02:26:20 GMT  
		Size: 52.2 MB (52167859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f443841afa6578a2062b06c2d45fbbc181c3c2de553f11d0ac93d9dfc070564d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122985746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e542cc9c79fc3e2ec84798dde3789f0b5fc87f754322e41e7064016e05111cfa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:28 GMT
ADD file:f0e83dd2590d6bd2d3726ebb3ebb5bfc0c2a52fe9feaeecd60b036c8eff69788 in / 
# Tue, 28 Sep 2021 01:40:28 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6f6f4e486b0370ea7bec101a3770e19279a47ffd7d20a9c48000fe3e63917bc`  
		Last Modified: Tue, 28 Sep 2021 01:49:34 GMT  
		Size: 51.2 MB (51207376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcad00d036c37c4de05381481665b986170717ee59000d1a49fa9e0d73ef484`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 8.0 MB (8000034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f546ea183fd0e99a89120a49252894e7056ddf33329190affa0efa1b5de5d929`  
		Last Modified: Tue, 28 Sep 2021 02:26:26 GMT  
		Size: 10.3 MB (10340144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b68564816940e410e66659fa680b3832e7c4d11ee4e50beaf82cacad47ea57`  
		Last Modified: Tue, 28 Sep 2021 02:26:52 GMT  
		Size: 53.4 MB (53438192 bytes)  
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
$ docker pull buildpack-deps@sha256:1c8fe95ec981148f1ff039c2319960a221ef986fb127fb37dcae1509e86fda14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130640469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2803b76ec4155b1b5c867fdd64df393b905c116605a8ebf0dd2f213cb99aff17`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:41 GMT
ADD file:1f8eebd902d2881786014a1e5db3cd6f0bab3a55e23befcd6cb6e4d91b9e6d79 in / 
# Fri, 03 Sep 2021 01:23:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:17:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:20ef04c157f9b9866c6408757e7ba2534608600e6cadbb759175572efc03f830`  
		Last Modified: Fri, 03 Sep 2021 01:38:28 GMT  
		Size: 54.2 MB (54182653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6474492bb0f747d1f925e9a2e0ed1d7b0bd0fdaa043e1fb2e892dde4313615`  
		Last Modified: Fri, 03 Sep 2021 07:12:35 GMT  
		Size: 8.3 MB (8272834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e098e859433301d306293ed680efa3bdc7d574613acc0d17fd90c09e854f779`  
		Last Modified: Fri, 03 Sep 2021 07:12:38 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0210891d190261ad1963160b64e1e7e13a3b1e4b1ac8f297c5280432fa730`  
		Last Modified: Fri, 03 Sep 2021 07:13:03 GMT  
		Size: 57.5 MB (57457148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e8a003f034fe144cf84bba783847c2ee4935327acbf51351c152745374668b17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117668874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e805d98391dca367564ea9a17b1e0f8f91f5029a586670ab3629dd1ed0206cbe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:11 GMT
ADD file:9eb47cd6584ec05371051b5cae96c24e6f03e66328173f27a9f30d46b8bce760 in / 
# Tue, 28 Sep 2021 01:43:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:09:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1481e22e2c9526464f32062da733ce595a9491b1e48870f085365fb7f9e8b60c`  
		Last Modified: Tue, 28 Sep 2021 01:49:17 GMT  
		Size: 49.0 MB (49004320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe83b756a24fd473ce558a06ee5b580a63605b4d9d74817e2e1d1289f54fb7f`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 7.4 MB (7400854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ed278d1f7ac1eb211375face0ceb4605c67610e32fce9d7601efdda86b1fc7`  
		Last Modified: Tue, 28 Sep 2021 02:16:42 GMT  
		Size: 9.9 MB (9883204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9675b3feffe472a443ef929f8e972471bd03506cf0ad31270751bfaad5feca5d`  
		Last Modified: Tue, 28 Sep 2021 02:16:56 GMT  
		Size: 51.4 MB (51380496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:aff21a12bf0addfb7d8e7ec0a44f9ab92b3584123f7c53f9fe6cc389cc8937b5
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
$ docker pull buildpack-deps@sha256:7b5d4f456f733f3b3edd7ed483335144b45a696e113345e0de17d68282da6b9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125519512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86feaac141dee4502631bb241160217b3a0ab6ae94d3b92cac8e497122a21bd4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:538c56184e9c046dbf00c862d346eaf338eb52d01e0893de7465ddfad38a8fca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120416221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194745ae83d6667c4aaa0274aa16f19bda1548ec9df3d0f4a31cbaf1cac33cc4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb5b710639fb53421f19a58b60a1a0cf28eea33da972ad7bcbab6628ed94797`  
		Last Modified: Tue, 28 Sep 2021 03:08:48 GMT  
		Size: 52.3 MB (52318852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8ba983722fda8c96eea16075c06ea7ba1d31db604469814964d231058e89a7b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115595846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fca1b7d9db700c661f89b9b85208e186b5102852ed2a757bee9a93d693df7f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:32:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beba146f18f8bf327bfc67faba4e70c717e79ccc563c8b535e44e9c14c2edfc`  
		Last Modified: Fri, 01 Oct 2021 05:53:47 GMT  
		Size: 50.3 MB (50328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ea086e8562101d3a3394d2405d80f211ec6792aed4ddbd25b5e52076e46fabce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124298879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd9f391f5d78e3aaeae0ee78fa5ce45069ef631e2579ddbdcb8873a48c73d44`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7e4e85949ee45bae139f288bc1cd85a740b408abdefaaba118c4c4626b021e`  
		Last Modified: Tue, 28 Sep 2021 02:25:03 GMT  
		Size: 54.7 MB (54669786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:46af4ece25d50f83819e2b897da064fd307a295d2770db9f80951a93e899a26f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128382229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca69ee284e3152e65f20eb98f1ae6c36fbc3ff0127b68c6e8d0d13550e9f6147`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9148b01e8bbfb04fa59f44e2af070eb74a8797213877fc7df3be0467115b9`  
		Last Modified: Tue, 28 Sep 2021 02:24:24 GMT  
		Size: 5.3 MB (5282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda7eaf6b4240f872ceef86fce4f8a87bdad74da3484b9605cb3b2b52cbbf20`  
		Last Modified: Tue, 28 Sep 2021 02:24:25 GMT  
		Size: 11.3 MB (11250636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50bcbe9fc6f4b839121363d75b4325536a717823ee2b2881b0247afe12fd6909`  
		Last Modified: Tue, 28 Sep 2021 02:24:58 GMT  
		Size: 55.9 MB (55916372 bytes)  
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
$ docker pull buildpack-deps@sha256:0079fcd37f046fdbc47f73c68e3301b7cb70947b2a248d6c3fc28008143759bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134696289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a755e8f1b32b86a7e3c3eb1702fb2c523aacade98b66f54fdbd1dc1631465c0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 05:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708d04ed929be54f33cfa94416648dcac9edd8c01746ecc6e250ce046aa54ac0`  
		Last Modified: Fri, 03 Sep 2021 07:09:38 GMT  
		Size: 58.8 MB (58849139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cc8ac782325035a5a46cf050e7b6611363ec94c8185f01f0b41b2d32a65f1720
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ee600655618ac729e88fc65d35e10aa6b00c909cee23ef5ab5b3c92ceee8f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:08:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f5b44618c39b6606db01fa6d460b6b7e1415b3a9c5a0b2f8b179c9b2c3fcfe`  
		Last Modified: Tue, 28 Sep 2021 02:16:05 GMT  
		Size: 54.0 MB (54049595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:448b2c42cadb43e92092f29207cdce0a01d084199a51bbb585cd0b13f6c1a5b9
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
$ docker pull buildpack-deps@sha256:efb1a54d6562d3ae971617eecbdf896ecefb73b5797344583caaf1776dea4162
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.0 MB (325002318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7599afc8b9104ad6cb6c92ab4734d15c10c7c2ef8a132422ef3ba88bdb7d657`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:24:18 GMT
ADD file:43a49c0ac74573bd560d191480bb30b2950f21ec76e9b3bdffdf73eb74628c50 in / 
# Tue, 28 Sep 2021 01:24:19 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:53:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e3fead4ded84f6449ee17b9deabf1e9144512edf86da02e0f93fbf81df3fd6fb`  
		Last Modified: Tue, 28 Sep 2021 01:31:21 GMT  
		Size: 55.7 MB (55702084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b8f6b86e3a84210feef982a4953fcc1b15003e51b2fb7b861ae18f18e914f`  
		Last Modified: Tue, 28 Sep 2021 02:00:14 GMT  
		Size: 5.2 MB (5181002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8e6a19825e33b3ebf505b0ae79fe6cf49091e693c4d8971abde683746f445`  
		Last Modified: Tue, 28 Sep 2021 02:00:15 GMT  
		Size: 10.9 MB (10900815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8600ac737a89c73eb8b73b618e244774719a3cc4caaa7325dbf6d6e04706ed`  
		Last Modified: Tue, 28 Sep 2021 02:00:34 GMT  
		Size: 55.7 MB (55730660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258a146afb1bcd19c174d0f8eb33a43c049127a82f2e1bffead6c9f03cfb84b3`  
		Last Modified: Tue, 28 Sep 2021 02:01:13 GMT  
		Size: 197.5 MB (197487757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fe1b2fc6392319cf2a844c4b7fa0da4838f388f6e2d2413b66e14c313f4128ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297514333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2959efdc159d70ab1117f74eb0e80050f090ee66ca49e693a0910f7b53d397da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:54:15 GMT
ADD file:bcd1f002a3a38be54eed5da9d7a2e3822ecdf63ba82a59931124557d1f97007b in / 
# Tue, 28 Sep 2021 01:54:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:00:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4bd09bbbe96b85664474243c833d73be517c92e7172b8d740101438ee21d5561`  
		Last Modified: Tue, 28 Sep 2021 02:11:21 GMT  
		Size: 53.2 MB (53207754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70c595ca5d004271509bd463bf50b3dc2d385630237ea30f5e4936f414a9b7`  
		Last Modified: Tue, 28 Sep 2021 03:14:06 GMT  
		Size: 5.1 MB (5088778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526e46f7c293bb67a0ab1c2bbce082b844bc145c04bb54e588fa2146980730af`  
		Last Modified: Tue, 28 Sep 2021 03:14:08 GMT  
		Size: 10.6 MB (10606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e39f8615ccdb2930517a3daed84ef9540d8f34f9a6a2447c42b05dd7e6d93`  
		Last Modified: Tue, 28 Sep 2021 03:14:58 GMT  
		Size: 53.4 MB (53435709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6669aa2732e897328c267a2d8b14ff0b2ba22b9e012b47944f5d6679f6c4f6`  
		Last Modified: Tue, 28 Sep 2021 03:16:54 GMT  
		Size: 175.2 MB (175175214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ce12648e9765e996822d2b6c0bffecc95bc1f445f4f22addb576279d8e9101b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.9 MB (284880273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927850025a048f1566f31c32e4eaac519e826ffee7f84a15e5aa18f57d9740da`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:06:54 GMT
ADD file:d9a8e8032b2f681adb1be7e9dfacdf1838167068f97e052c3173223cb1d2c303 in / 
# Thu, 30 Sep 2021 18:06:55 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:39:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:40:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:42:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90a9a2564a394330c4b6320f33e007b55c6f40a9006b85fe17fa2ed9fe260cee`  
		Last Modified: Thu, 30 Sep 2021 18:23:58 GMT  
		Size: 50.8 MB (50822436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f06eb4253b6bc5ee446db688fa4b3052465b6890ef2f7157f1a345118360e`  
		Last Modified: Fri, 01 Oct 2021 05:58:43 GMT  
		Size: 4.9 MB (4946836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b50232f315931bda767b06cac42d2688e34c66a06877f32bc9bdb103575e50`  
		Last Modified: Fri, 01 Oct 2021 05:58:45 GMT  
		Size: 10.2 MB (10249907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6189d745298f970340832970521c77f9df62fa058d6a498469ecaac7cdd9e`  
		Last Modified: Fri, 01 Oct 2021 05:59:31 GMT  
		Size: 51.4 MB (51371485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626fd6dc0bb62c7a429172fe52c51d82255b7b0b7e9cd7a377c2ae9b272e0e41`  
		Last Modified: Fri, 01 Oct 2021 06:01:16 GMT  
		Size: 167.5 MB (167489609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:524d70b0c8fb2f1a271185979c1d4d275f123c70b768ccf86467bb1a62b2a6f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.7 MB (316687005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41db0b469d56879a649dec194de46b605e0a658813fe6140127b8d6aa23e0c01`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:20 GMT
ADD file:714781c9fce1c450e5f9cc5529167eaa33fdff089ab48a1dcac0a813d768be30 in / 
# Tue, 28 Sep 2021 01:42:20 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:18:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:19:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd53cd90ab526d30a2e414c3951333db1b1b814fe009621017a07b5eea3cad0f`  
		Last Modified: Tue, 28 Sep 2021 01:51:10 GMT  
		Size: 54.7 MB (54725302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945f16b6588acc2f82d3f0371dd15803436b26df556a96921d086d035a320cd`  
		Last Modified: Tue, 28 Sep 2021 02:27:09 GMT  
		Size: 5.2 MB (5169449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba2c20fe4248de05c9d215800868bdf9800fbc648f764ff6aabe878e837cf5e`  
		Last Modified: Tue, 28 Sep 2021 02:27:10 GMT  
		Size: 10.9 MB (10899138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb38129bed7931b18a48dcbaa75e8350149907c137d95496ab9e8fbb32aa6d6`  
		Last Modified: Tue, 28 Sep 2021 02:27:30 GMT  
		Size: 55.9 MB (55867003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0836b49579e1ee352ee58e9b6c1320c3328fe03fb098d7a2d4d7c1f5bfbdc`  
		Last Modified: Tue, 28 Sep 2021 02:28:07 GMT  
		Size: 190.0 MB (190026113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d626cefcea6ec3c6654f1b94b8db3fda2595ec1b38a111dec9a79a2ce72caf31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.3 MB (328291208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924bd8ae3a1df8c572a1ebfb6a23252af19a419fd4759ce71b78689e68e85f0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:17 GMT
ADD file:07dfd2960f3649fbe7a701ad0b551f48b4815ff5eabaefe7aaf62e770435e5f2 in / 
# Tue, 28 Sep 2021 01:42:18 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ed4b6e2f624e3ac187bdfdafce616f76387ede25afbec70c204c9d6300d2e0`  
		Last Modified: Tue, 28 Sep 2021 01:52:05 GMT  
		Size: 56.7 MB (56733325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a4c8e238708f81b44eb4ba40b5c8f710f262c0c1745ffcdb299c8387dc061`  
		Last Modified: Tue, 28 Sep 2021 02:27:58 GMT  
		Size: 5.3 MB (5312381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e976216252ce09cde1548cf4c9a4e367e1cc4c4fee46d9a25408720edd938df`  
		Last Modified: Tue, 28 Sep 2021 02:27:59 GMT  
		Size: 11.3 MB (11282013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6ebec24d20e38092d845932f91387b27fb11b3740ba554966788b972768db`  
		Last Modified: Tue, 28 Sep 2021 02:28:26 GMT  
		Size: 57.2 MB (57151017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cedae44a9ec227abfbabebaeb53f31f845d9886fed86f7eb2a35f62e398dcb2`  
		Last Modified: Tue, 28 Sep 2021 02:29:30 GMT  
		Size: 197.8 MB (197812472 bytes)  
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
$ docker pull buildpack-deps@sha256:6ebc81f3c1a34e2586abf1f4fd150c75d8459eb2b0c040dfc336ca955f1d88bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334296089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7572ef35d6da465015e1104284fd7fb00fa202aea43ba80271f3808fec3a0fa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:05:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a95302a54a7fa51cdd0cd0117968b05d9f71d3c40eafe66873816a3b43ba14`  
		Last Modified: Fri, 03 Sep 2021 07:14:06 GMT  
		Size: 5.4 MB (5422617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da11fea16e40da1a9b66dee60a49dee27fffb468c778b12670ed59f3cd11837`  
		Last Modified: Fri, 03 Sep 2021 07:14:07 GMT  
		Size: 11.7 MB (11650959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd39c289a3baa1fff8358db49e63fac02746752ceae177b4b7a19642ba640995`  
		Last Modified: Fri, 03 Sep 2021 07:14:30 GMT  
		Size: 60.1 MB (60114890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f3c7ffcb3f63c765e1e528a5bcf0e279cc85c94b4feb1db90889365457802b`  
		Last Modified: Fri, 03 Sep 2021 07:15:16 GMT  
		Size: 197.6 MB (197573551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82a5f039001206c34e9980c0b125465287f9eae25b375c0f6208ea0eda1102a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331495706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc78af4ec6bd0acab27b6933fd88cc1d5cf6518dd1357312a98bc90d3db091c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:14:19 GMT
ADD file:c8ff49735749af794fa2a6ca03eb4ac0fb66dffd4ead8d9902ee04483db97aff in / 
# Tue, 28 Sep 2021 02:14:22 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:56:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:58:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:12:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f903d1b59452679ad13935f22aa7eb73ffa71398303161a843221e41855e5bce`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.5 MB (51531137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec6ba981ab80c88267fed9b741a2a2ace934d0bb03930338f0126518120a416`  
		Last Modified: Tue, 28 Sep 2021 03:35:59 GMT  
		Size: 5.0 MB (4997888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736a4b194f9d38dde15b4c734cd79228a198fb0314eed4526e0135d4254874b4`  
		Last Modified: Tue, 28 Sep 2021 03:36:02 GMT  
		Size: 10.3 MB (10314682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36c310fdfaed216b6a43fd07fe77c729b8d8abfb8772e830cda42b0cca7024f`  
		Last Modified: Tue, 28 Sep 2021 03:38:07 GMT  
		Size: 51.8 MB (51783989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36eab1b54c6853b466e19a2e6ec879edac6a7bd66f7175578c5f0b0fb23b89b`  
		Last Modified: Tue, 28 Sep 2021 03:43:51 GMT  
		Size: 212.9 MB (212868010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a3ec81993a54920402b059f89de3f61e3753d964f3f5b7651dafb27db2c64287
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.2 MB (298164614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3477144a143fac537af824ce79d485fab57e51a91aeeac7bcb59b9167ecdcf8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:11 GMT
ADD file:797f09f7e25e9194e8845d5783ab9078062d7caad45c75201a4ad699145b1305 in / 
# Tue, 28 Sep 2021 01:44:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:12:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8463103c03054c6dd4bf0a387d658bdf4d12ddbb0d87ce07eaa15b2b13f1d733`  
		Last Modified: Tue, 28 Sep 2021 01:50:20 GMT  
		Size: 54.0 MB (53953837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32362b87984c1bba14b0f80546944827886c7cc7accd0865b4ccc7f34a9f3b8a`  
		Last Modified: Tue, 28 Sep 2021 02:17:31 GMT  
		Size: 5.2 MB (5165065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aadefacf33492b3a74622a982ea04f1605a554feeaa2ef0abdd214a94280744`  
		Last Modified: Tue, 28 Sep 2021 02:17:32 GMT  
		Size: 10.8 MB (10793806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217921cacc4173d4ddbf287e61dbfb88ee91ded7acf28b93d6b7db50ca7ca75`  
		Last Modified: Tue, 28 Sep 2021 02:17:48 GMT  
		Size: 55.2 MB (55159873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e09838e2681cac8b641b6a8bd947c86ce543872a81967a64ab4cfd78c35c8f3`  
		Last Modified: Tue, 28 Sep 2021 02:18:13 GMT  
		Size: 173.1 MB (173092033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:0ff93d51e83675d401c67c79e63e476d548b325b652aab348e14f616711390bf
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
$ docker pull buildpack-deps@sha256:876cfe58c039fd813ff318d4e53e2707c884cb7b8c7952464dcf2e27cca17b5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71783901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:506d6fd65061be41934c131b48e3c840c7e841b27244c6d3c657f0c4008db311`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:24:18 GMT
ADD file:43a49c0ac74573bd560d191480bb30b2950f21ec76e9b3bdffdf73eb74628c50 in / 
# Tue, 28 Sep 2021 01:24:19 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:53:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e3fead4ded84f6449ee17b9deabf1e9144512edf86da02e0f93fbf81df3fd6fb`  
		Last Modified: Tue, 28 Sep 2021 01:31:21 GMT  
		Size: 55.7 MB (55702084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b8f6b86e3a84210feef982a4953fcc1b15003e51b2fb7b861ae18f18e914f`  
		Last Modified: Tue, 28 Sep 2021 02:00:14 GMT  
		Size: 5.2 MB (5181002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8e6a19825e33b3ebf505b0ae79fe6cf49091e693c4d8971abde683746f445`  
		Last Modified: Tue, 28 Sep 2021 02:00:15 GMT  
		Size: 10.9 MB (10900815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e87ec835044393c77ab96a3c4fbf5d4f999fe5c2aea983a35c8a24f333106911
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68903410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9a5d7085c78c1d80020d21fdc2bfcb29fe53b22a93b588e0d67af242ef17aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:54:15 GMT
ADD file:bcd1f002a3a38be54eed5da9d7a2e3822ecdf63ba82a59931124557d1f97007b in / 
# Tue, 28 Sep 2021 01:54:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4bd09bbbe96b85664474243c833d73be517c92e7172b8d740101438ee21d5561`  
		Last Modified: Tue, 28 Sep 2021 02:11:21 GMT  
		Size: 53.2 MB (53207754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70c595ca5d004271509bd463bf50b3dc2d385630237ea30f5e4936f414a9b7`  
		Last Modified: Tue, 28 Sep 2021 03:14:06 GMT  
		Size: 5.1 MB (5088778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526e46f7c293bb67a0ab1c2bbce082b844bc145c04bb54e588fa2146980730af`  
		Last Modified: Tue, 28 Sep 2021 03:14:08 GMT  
		Size: 10.6 MB (10606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ec123566e37f91cf7dc999a213d362dfbf1413d9ac4ad6232d3bee77c01ca4c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66019179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f8848536df00d83694de40159ebe8595caf2bf001797c4d47dea972c82eb99`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:06:54 GMT
ADD file:d9a8e8032b2f681adb1be7e9dfacdf1838167068f97e052c3173223cb1d2c303 in / 
# Thu, 30 Sep 2021 18:06:55 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:39:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:90a9a2564a394330c4b6320f33e007b55c6f40a9006b85fe17fa2ed9fe260cee`  
		Last Modified: Thu, 30 Sep 2021 18:23:58 GMT  
		Size: 50.8 MB (50822436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f06eb4253b6bc5ee446db688fa4b3052465b6890ef2f7157f1a345118360e`  
		Last Modified: Fri, 01 Oct 2021 05:58:43 GMT  
		Size: 4.9 MB (4946836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b50232f315931bda767b06cac42d2688e34c66a06877f32bc9bdb103575e50`  
		Last Modified: Fri, 01 Oct 2021 05:58:45 GMT  
		Size: 10.2 MB (10249907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3cacb2497db42e4160cef77ad2ebed9249918ab55507fe1ca75a48a3b384ec58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70793889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e7747dd728e45e46bfbd2d710d52a2e130eae3b33fc78392bb548807e00939a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:20 GMT
ADD file:714781c9fce1c450e5f9cc5529167eaa33fdff089ab48a1dcac0a813d768be30 in / 
# Tue, 28 Sep 2021 01:42:20 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:18:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bd53cd90ab526d30a2e414c3951333db1b1b814fe009621017a07b5eea3cad0f`  
		Last Modified: Tue, 28 Sep 2021 01:51:10 GMT  
		Size: 54.7 MB (54725302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945f16b6588acc2f82d3f0371dd15803436b26df556a96921d086d035a320cd`  
		Last Modified: Tue, 28 Sep 2021 02:27:09 GMT  
		Size: 5.2 MB (5169449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba2c20fe4248de05c9d215800868bdf9800fbc648f764ff6aabe878e837cf5e`  
		Last Modified: Tue, 28 Sep 2021 02:27:10 GMT  
		Size: 10.9 MB (10899138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:138dafec4d1ffcacfb0d88e1ec201cefc8e953f8e5e2b566dc381409fe1df3ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73327719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0a6347fe9bfe440f7f7bee5c7628ea6b41d05955bcfc1e8025699c51acd5cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:17 GMT
ADD file:07dfd2960f3649fbe7a701ad0b551f48b4815ff5eabaefe7aaf62e770435e5f2 in / 
# Tue, 28 Sep 2021 01:42:18 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e7ed4b6e2f624e3ac187bdfdafce616f76387ede25afbec70c204c9d6300d2e0`  
		Last Modified: Tue, 28 Sep 2021 01:52:05 GMT  
		Size: 56.7 MB (56733325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a4c8e238708f81b44eb4ba40b5c8f710f262c0c1745ffcdb299c8387dc061`  
		Last Modified: Tue, 28 Sep 2021 02:27:58 GMT  
		Size: 5.3 MB (5312381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e976216252ce09cde1548cf4c9a4e367e1cc4c4fee46d9a25408720edd938df`  
		Last Modified: Tue, 28 Sep 2021 02:27:59 GMT  
		Size: 11.3 MB (11282013 bytes)  
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
$ docker pull buildpack-deps@sha256:f686e9380a7ddf6bd2900de9f550ad307efaec5625ed23c223f0bc49e5b4eb11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76607648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:458f349d2522ffbef1b1dc6a5f6f49b9c4cec344f768cabcf7a36baec2536acd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a95302a54a7fa51cdd0cd0117968b05d9f71d3c40eafe66873816a3b43ba14`  
		Last Modified: Fri, 03 Sep 2021 07:14:06 GMT  
		Size: 5.4 MB (5422617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da11fea16e40da1a9b66dee60a49dee27fffb468c778b12670ed59f3cd11837`  
		Last Modified: Fri, 03 Sep 2021 07:14:07 GMT  
		Size: 11.7 MB (11650959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0a6ecb3329f5b8d000b8e6e5e10ff4a66e34755b3f2f51f80bd52ee98f763704
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66843707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ea89476054b4f64f3f7013eaa3d25bfdb786c2b2a83de0b362dee8da2c37c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:14:19 GMT
ADD file:c8ff49735749af794fa2a6ca03eb4ac0fb66dffd4ead8d9902ee04483db97aff in / 
# Tue, 28 Sep 2021 02:14:22 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:56:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:58:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f903d1b59452679ad13935f22aa7eb73ffa71398303161a843221e41855e5bce`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.5 MB (51531137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec6ba981ab80c88267fed9b741a2a2ace934d0bb03930338f0126518120a416`  
		Last Modified: Tue, 28 Sep 2021 03:35:59 GMT  
		Size: 5.0 MB (4997888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736a4b194f9d38dde15b4c734cd79228a198fb0314eed4526e0135d4254874b4`  
		Last Modified: Tue, 28 Sep 2021 03:36:02 GMT  
		Size: 10.3 MB (10314682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b734c11fedc4319a44595c49e3541d7a69e4c3bde2e5b12f1082ed915b59a556
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69912708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f80b8e561ff61c6a6d9bd4db8e89f29950f901bce96b85d1b662f440d23f5c4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:11 GMT
ADD file:797f09f7e25e9194e8845d5783ab9078062d7caad45c75201a4ad699145b1305 in / 
# Tue, 28 Sep 2021 01:44:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8463103c03054c6dd4bf0a387d658bdf4d12ddbb0d87ce07eaa15b2b13f1d733`  
		Last Modified: Tue, 28 Sep 2021 01:50:20 GMT  
		Size: 54.0 MB (53953837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32362b87984c1bba14b0f80546944827886c7cc7accd0865b4ccc7f34a9f3b8a`  
		Last Modified: Tue, 28 Sep 2021 02:17:31 GMT  
		Size: 5.2 MB (5165065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aadefacf33492b3a74622a982ea04f1605a554feeaa2ef0abdd214a94280744`  
		Last Modified: Tue, 28 Sep 2021 02:17:32 GMT  
		Size: 10.8 MB (10793806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:20d37c1005ae07c16a77312fa565ac3990399a169d5feac9e5368d43845087eb
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
$ docker pull buildpack-deps@sha256:0abecfd3831c9b69c830ddadefd33d2ab68555ce081e9eb05c0cd44c2bd0b153
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127514561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3557e30291bd8748d13ae0a1df0419cd78a45eddb9d3e6f26d3ab66dcfe91cb6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:24:18 GMT
ADD file:43a49c0ac74573bd560d191480bb30b2950f21ec76e9b3bdffdf73eb74628c50 in / 
# Tue, 28 Sep 2021 01:24:19 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:53:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e3fead4ded84f6449ee17b9deabf1e9144512edf86da02e0f93fbf81df3fd6fb`  
		Last Modified: Tue, 28 Sep 2021 01:31:21 GMT  
		Size: 55.7 MB (55702084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b8f6b86e3a84210feef982a4953fcc1b15003e51b2fb7b861ae18f18e914f`  
		Last Modified: Tue, 28 Sep 2021 02:00:14 GMT  
		Size: 5.2 MB (5181002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8e6a19825e33b3ebf505b0ae79fe6cf49091e693c4d8971abde683746f445`  
		Last Modified: Tue, 28 Sep 2021 02:00:15 GMT  
		Size: 10.9 MB (10900815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8600ac737a89c73eb8b73b618e244774719a3cc4caaa7325dbf6d6e04706ed`  
		Last Modified: Tue, 28 Sep 2021 02:00:34 GMT  
		Size: 55.7 MB (55730660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4cd97ee516ec215abbd5b3ac462930d5ce96d603e843d9e3c16f2f89b92fa7cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122339119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5cd7b304c5341441e3c2c40eeb8cb460e041906d3883be6d82bebca44295a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:54:15 GMT
ADD file:bcd1f002a3a38be54eed5da9d7a2e3822ecdf63ba82a59931124557d1f97007b in / 
# Tue, 28 Sep 2021 01:54:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4bd09bbbe96b85664474243c833d73be517c92e7172b8d740101438ee21d5561`  
		Last Modified: Tue, 28 Sep 2021 02:11:21 GMT  
		Size: 53.2 MB (53207754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70c595ca5d004271509bd463bf50b3dc2d385630237ea30f5e4936f414a9b7`  
		Last Modified: Tue, 28 Sep 2021 03:14:06 GMT  
		Size: 5.1 MB (5088778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526e46f7c293bb67a0ab1c2bbce082b844bc145c04bb54e588fa2146980730af`  
		Last Modified: Tue, 28 Sep 2021 03:14:08 GMT  
		Size: 10.6 MB (10606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e39f8615ccdb2930517a3daed84ef9540d8f34f9a6a2447c42b05dd7e6d93`  
		Last Modified: Tue, 28 Sep 2021 03:14:58 GMT  
		Size: 53.4 MB (53435709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7a0d1efa6e01ca27a3c8b6ce00256addbf9e6a87727403382b3bb85867f46245
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.4 MB (117390664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30ca238d4f10dd5e6d87c27eca2dbd6a378f05ea84b11758f19a8a33cb2b27e0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:06:54 GMT
ADD file:d9a8e8032b2f681adb1be7e9dfacdf1838167068f97e052c3173223cb1d2c303 in / 
# Thu, 30 Sep 2021 18:06:55 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:39:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:40:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90a9a2564a394330c4b6320f33e007b55c6f40a9006b85fe17fa2ed9fe260cee`  
		Last Modified: Thu, 30 Sep 2021 18:23:58 GMT  
		Size: 50.8 MB (50822436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f06eb4253b6bc5ee446db688fa4b3052465b6890ef2f7157f1a345118360e`  
		Last Modified: Fri, 01 Oct 2021 05:58:43 GMT  
		Size: 4.9 MB (4946836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b50232f315931bda767b06cac42d2688e34c66a06877f32bc9bdb103575e50`  
		Last Modified: Fri, 01 Oct 2021 05:58:45 GMT  
		Size: 10.2 MB (10249907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6189d745298f970340832970521c77f9df62fa058d6a498469ecaac7cdd9e`  
		Last Modified: Fri, 01 Oct 2021 05:59:31 GMT  
		Size: 51.4 MB (51371485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3b8e35be88c4a91d8413351d8c621c65496a35142b7b0e4c7f97c9ade9a3f078
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126660892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51de9ff568cdc9fcc755ffef64b86ff3ac486276a65accf31b79039ae9812ff3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:20 GMT
ADD file:714781c9fce1c450e5f9cc5529167eaa33fdff089ab48a1dcac0a813d768be30 in / 
# Tue, 28 Sep 2021 01:42:20 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:18:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd53cd90ab526d30a2e414c3951333db1b1b814fe009621017a07b5eea3cad0f`  
		Last Modified: Tue, 28 Sep 2021 01:51:10 GMT  
		Size: 54.7 MB (54725302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945f16b6588acc2f82d3f0371dd15803436b26df556a96921d086d035a320cd`  
		Last Modified: Tue, 28 Sep 2021 02:27:09 GMT  
		Size: 5.2 MB (5169449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba2c20fe4248de05c9d215800868bdf9800fbc648f764ff6aabe878e837cf5e`  
		Last Modified: Tue, 28 Sep 2021 02:27:10 GMT  
		Size: 10.9 MB (10899138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb38129bed7931b18a48dcbaa75e8350149907c137d95496ab9e8fbb32aa6d6`  
		Last Modified: Tue, 28 Sep 2021 02:27:30 GMT  
		Size: 55.9 MB (55867003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:06b714e4afeeaf5a5ea67a0e493064f71329a8a8a9b01d40f8d5b0bc87b04e16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130478736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42882d2ad744ca8f780a934a350b370b9184646c9ba3a6fe87ec9da44ee3ae33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:17 GMT
ADD file:07dfd2960f3649fbe7a701ad0b551f48b4815ff5eabaefe7aaf62e770435e5f2 in / 
# Tue, 28 Sep 2021 01:42:18 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ed4b6e2f624e3ac187bdfdafce616f76387ede25afbec70c204c9d6300d2e0`  
		Last Modified: Tue, 28 Sep 2021 01:52:05 GMT  
		Size: 56.7 MB (56733325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a4c8e238708f81b44eb4ba40b5c8f710f262c0c1745ffcdb299c8387dc061`  
		Last Modified: Tue, 28 Sep 2021 02:27:58 GMT  
		Size: 5.3 MB (5312381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e976216252ce09cde1548cf4c9a4e367e1cc4c4fee46d9a25408720edd938df`  
		Last Modified: Tue, 28 Sep 2021 02:27:59 GMT  
		Size: 11.3 MB (11282013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6ebec24d20e38092d845932f91387b27fb11b3740ba554966788b972768db`  
		Last Modified: Tue, 28 Sep 2021 02:28:26 GMT  
		Size: 57.2 MB (57151017 bytes)  
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
$ docker pull buildpack-deps@sha256:a5c418dd1d0e473e559b3a703a9e40757ead45790002b65bfc2bb736e31a077f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136722538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf7cb6d58a64ecbd4e666e5dc9905f0bb6786a021d2c2d955cf233ab37f7ef`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a95302a54a7fa51cdd0cd0117968b05d9f71d3c40eafe66873816a3b43ba14`  
		Last Modified: Fri, 03 Sep 2021 07:14:06 GMT  
		Size: 5.4 MB (5422617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da11fea16e40da1a9b66dee60a49dee27fffb468c778b12670ed59f3cd11837`  
		Last Modified: Fri, 03 Sep 2021 07:14:07 GMT  
		Size: 11.7 MB (11650959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd39c289a3baa1fff8358db49e63fac02746752ceae177b4b7a19642ba640995`  
		Last Modified: Fri, 03 Sep 2021 07:14:30 GMT  
		Size: 60.1 MB (60114890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:f39ef8a4165175de61f83dc3174aa76194916a15f5137f0e1bf51f5b86cc7ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118627696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1485f61f1c24b7322dfb4b732919e5862c78ff48a917cb91cdae8e09b3e50e75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:14:19 GMT
ADD file:c8ff49735749af794fa2a6ca03eb4ac0fb66dffd4ead8d9902ee04483db97aff in / 
# Tue, 28 Sep 2021 02:14:22 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:56:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:58:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f903d1b59452679ad13935f22aa7eb73ffa71398303161a843221e41855e5bce`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.5 MB (51531137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec6ba981ab80c88267fed9b741a2a2ace934d0bb03930338f0126518120a416`  
		Last Modified: Tue, 28 Sep 2021 03:35:59 GMT  
		Size: 5.0 MB (4997888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736a4b194f9d38dde15b4c734cd79228a198fb0314eed4526e0135d4254874b4`  
		Last Modified: Tue, 28 Sep 2021 03:36:02 GMT  
		Size: 10.3 MB (10314682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36c310fdfaed216b6a43fd07fe77c729b8d8abfb8772e830cda42b0cca7024f`  
		Last Modified: Tue, 28 Sep 2021 03:38:07 GMT  
		Size: 51.8 MB (51783989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:32b95e6cbcac8947758c681cc7c6e8995abc6b755ad8853070676f621ccf168b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125072581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d879c30c528729314fbb2e692c8bfb507fd458de13198f1af75a320ad2fd8d7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:11 GMT
ADD file:797f09f7e25e9194e8845d5783ab9078062d7caad45c75201a4ad699145b1305 in / 
# Tue, 28 Sep 2021 01:44:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8463103c03054c6dd4bf0a387d658bdf4d12ddbb0d87ce07eaa15b2b13f1d733`  
		Last Modified: Tue, 28 Sep 2021 01:50:20 GMT  
		Size: 54.0 MB (53953837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32362b87984c1bba14b0f80546944827886c7cc7accd0865b4ccc7f34a9f3b8a`  
		Last Modified: Tue, 28 Sep 2021 02:17:31 GMT  
		Size: 5.2 MB (5165065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aadefacf33492b3a74622a982ea04f1605a554feeaa2ef0abdd214a94280744`  
		Last Modified: Tue, 28 Sep 2021 02:17:32 GMT  
		Size: 10.8 MB (10793806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217921cacc4173d4ddbf287e61dbfb88ee91ded7acf28b93d6b7db50ca7ca75`  
		Last Modified: Tue, 28 Sep 2021 02:17:48 GMT  
		Size: 55.2 MB (55159873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:e54ae211c5b7f7bef56152bd3004a28989c31d88a6a12e104ba91e715194af2a
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
$ docker pull buildpack-deps@sha256:dc426fff2922e74aa6934ccd1df91e1298cb3ccde18c2f1835f12e70f6220371
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (321969341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:714418fd1dff72d98cd2a7fe82a6a4636418db789278fba59735ebda645e9b27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8e6af58ed3a502f0c3c15dce636d9d362a742eb5b67770d0cfcb72f3a9884`  
		Last Modified: Tue, 28 Sep 2021 01:58:51 GMT  
		Size: 196.4 MB (196449829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7123e9831bb45f888b6806417d2dfe1f180e62e19c677b0d09abb7f80c311de8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295057178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6fd0cb97521cc96a0089159a684d52da508f86d751d5ccb9fa131a6b417689`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb5b710639fb53421f19a58b60a1a0cf28eea33da972ad7bcbab6628ed94797`  
		Last Modified: Tue, 28 Sep 2021 03:08:48 GMT  
		Size: 52.3 MB (52318852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff0c2fb11e77b1bab4e3d2c8b9ff79d5a4bfa2a4c81e291370227cdcf5eae2f`  
		Last Modified: Tue, 28 Sep 2021 03:10:48 GMT  
		Size: 174.6 MB (174640957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:337edfa1be8e16858eddd085e94b6742ba6d116a6e3734497043b26664d576a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282490296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d74011c8e2e7e4542e3f3cd14eafdc2eaff461a41a64d1cef541a8c4b30b501`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:32:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beba146f18f8bf327bfc67faba4e70c717e79ccc563c8b535e44e9c14c2edfc`  
		Last Modified: Fri, 01 Oct 2021 05:53:47 GMT  
		Size: 50.3 MB (50328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd4233acc34086e6db32b75d876bd6ea7538de484ea9b48c9ddd1907aa74ca0`  
		Last Modified: Fri, 01 Oct 2021 05:55:36 GMT  
		Size: 166.9 MB (166894450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3609418ae510b339d73ab6f19ba3a82c8e0bdc171f50df8949f0a3735de06667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313636281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a992d40e6a046b86ed17052793e80b837e5266c1a03f3261b2c558ddd77837f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7e4e85949ee45bae139f288bc1cd85a740b408abdefaaba118c4c4626b021e`  
		Last Modified: Tue, 28 Sep 2021 02:25:03 GMT  
		Size: 54.7 MB (54669786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69e7bcc0bc59e0f5c70e40bc8adebeb94f60240a71e7f8add74d8b9146bbc16`  
		Last Modified: Tue, 28 Sep 2021 02:25:44 GMT  
		Size: 189.3 MB (189337402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:777672fe2d3733ca92041d6bf3fe878cb1f5fdacc449e71e2217750a840bcdf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327745828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be8f244a554fc912c1932f609263329ff9b3d7bcabed8cb7ed0d6d657f5787f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9148b01e8bbfb04fa59f44e2af070eb74a8797213877fc7df3be0467115b9`  
		Last Modified: Tue, 28 Sep 2021 02:24:24 GMT  
		Size: 5.3 MB (5282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda7eaf6b4240f872ceef86fce4f8a87bdad74da3484b9605cb3b2b52cbbf20`  
		Last Modified: Tue, 28 Sep 2021 02:24:25 GMT  
		Size: 11.3 MB (11250636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50bcbe9fc6f4b839121363d75b4325536a717823ee2b2881b0247afe12fd6909`  
		Last Modified: Tue, 28 Sep 2021 02:24:58 GMT  
		Size: 55.9 MB (55916372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3de1989e93fff2054295962d5bbfbfb11bfa4533ad691aaa17c9a52e3a8a22b`  
		Last Modified: Tue, 28 Sep 2021 02:26:07 GMT  
		Size: 199.4 MB (199363599 bytes)  
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
$ docker pull buildpack-deps@sha256:decae382d4f56e845e9800f3b79f315daccccfb47340e44c9f09f0310e8b98d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330495335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c4c1fd57c37be3803887ab8eee646176344caa36226b3c0131b4cd932867afd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 05:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:13:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708d04ed929be54f33cfa94416648dcac9edd8c01746ecc6e250ce046aa54ac0`  
		Last Modified: Fri, 03 Sep 2021 07:09:38 GMT  
		Size: 58.8 MB (58849139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287624e1f6e58d3860703363b792d02bb699c973abd9dadfa2db8495b51ceb93`  
		Last Modified: Fri, 03 Sep 2021 07:12:15 GMT  
		Size: 195.8 MB (195799046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:51e14eaab3cc2825279677ba4a729da747e7686e4de1df8f933005cf8f8bc13b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295585571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa2779752696eb6bfd10f0076125e41a51fad44a72ed6a636d376f337c439375`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:08:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:08:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f5b44618c39b6606db01fa6d460b6b7e1415b3a9c5a0b2f8b179c9b2c3fcfe`  
		Last Modified: Tue, 28 Sep 2021 02:16:05 GMT  
		Size: 54.0 MB (54049595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6589c0454003c1deeaf24f87ae908e9816d7cb9a945148cf89e75038aba3c8`  
		Last Modified: Tue, 28 Sep 2021 02:16:32 GMT  
		Size: 172.4 MB (172435364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:8f4b29031e8204331606d488fb6290f99bc6ccc7f50623272e1e76a966487520
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
$ docker pull buildpack-deps@sha256:6d3bd0093dc57538be1da3cda96a80f944ab167c2f9fcff321db397d15923754
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70952632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f020ab5dd0cef2c0b20ded3f290546ae4b2a84986d4e02446879a72cf0d1cbd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:151b67336eac36e8c7376d2f603965b3d613b838a8c6c00df65ecb6b81ebb7e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68097369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecfe7b5c5061f7480a7a1a7306e93ea2082b63b6b9d1f29c9b01b70d4ae129e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:96c3837335e336493dd4ec502568a24fb8a0f808d15ed1a844c573d738b99ff4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65267580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feef68d841ccaedfa1bae704efe715b0f162812c549f94539d335e6784b6a512`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d685bcbd37d39eab77c65ae1e04e72d35d3ae193256f074d84a5c87d59842bf2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69629093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990cb9bf14263220789cdd25eb191d564fb567f94c522c1494a07737584426c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d4f08dbf769815a4db9592b6f8911b61ada4280051f115b8b5bf88c9ae6d6e18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72465857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f109721ea809e5ae6fcfd2a47160b846d943350a073e5e431b4bbbf9688d9d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9148b01e8bbfb04fa59f44e2af070eb74a8797213877fc7df3be0467115b9`  
		Last Modified: Tue, 28 Sep 2021 02:24:24 GMT  
		Size: 5.3 MB (5282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda7eaf6b4240f872ceef86fce4f8a87bdad74da3484b9605cb3b2b52cbbf20`  
		Last Modified: Tue, 28 Sep 2021 02:24:25 GMT  
		Size: 11.3 MB (11250636 bytes)  
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
$ docker pull buildpack-deps@sha256:e645211432960dea9563d3ce20b165c647ec21f29d3bc873e80e417076f5b108
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75847150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b9a35d2eb70c2fbc27b4c72a127f42b6b685425398b8ead7a2283f10e32ac5c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:076601aae27650f44b4dbe20132157de742e741af9d5fc796db9032604ab6cf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69100612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73dbb50e50b5a3c5d39455f73ca943eb867aba4106eb831077daf48cee43647a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:aff21a12bf0addfb7d8e7ec0a44f9ab92b3584123f7c53f9fe6cc389cc8937b5
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
$ docker pull buildpack-deps@sha256:7b5d4f456f733f3b3edd7ed483335144b45a696e113345e0de17d68282da6b9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125519512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86feaac141dee4502631bb241160217b3a0ab6ae94d3b92cac8e497122a21bd4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:538c56184e9c046dbf00c862d346eaf338eb52d01e0893de7465ddfad38a8fca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120416221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194745ae83d6667c4aaa0274aa16f19bda1548ec9df3d0f4a31cbaf1cac33cc4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb5b710639fb53421f19a58b60a1a0cf28eea33da972ad7bcbab6628ed94797`  
		Last Modified: Tue, 28 Sep 2021 03:08:48 GMT  
		Size: 52.3 MB (52318852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8ba983722fda8c96eea16075c06ea7ba1d31db604469814964d231058e89a7b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115595846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fca1b7d9db700c661f89b9b85208e186b5102852ed2a757bee9a93d693df7f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:32:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beba146f18f8bf327bfc67faba4e70c717e79ccc563c8b535e44e9c14c2edfc`  
		Last Modified: Fri, 01 Oct 2021 05:53:47 GMT  
		Size: 50.3 MB (50328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ea086e8562101d3a3394d2405d80f211ec6792aed4ddbd25b5e52076e46fabce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124298879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd9f391f5d78e3aaeae0ee78fa5ce45069ef631e2579ddbdcb8873a48c73d44`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7e4e85949ee45bae139f288bc1cd85a740b408abdefaaba118c4c4626b021e`  
		Last Modified: Tue, 28 Sep 2021 02:25:03 GMT  
		Size: 54.7 MB (54669786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:46af4ece25d50f83819e2b897da064fd307a295d2770db9f80951a93e899a26f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128382229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca69ee284e3152e65f20eb98f1ae6c36fbc3ff0127b68c6e8d0d13550e9f6147`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:39:47 GMT
ADD file:a666560999115997edd232185b410db82d88832f98f754ee331f505de6fca72b in / 
# Tue, 28 Sep 2021 01:39:48 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdfe255b6e1e8f9836f895e8f412f81c3be9ff0081a6e681c62b3bd736c4118a`  
		Last Modified: Tue, 28 Sep 2021 01:48:32 GMT  
		Size: 55.9 MB (55932237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9148b01e8bbfb04fa59f44e2af070eb74a8797213877fc7df3be0467115b9`  
		Last Modified: Tue, 28 Sep 2021 02:24:24 GMT  
		Size: 5.3 MB (5282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fda7eaf6b4240f872ceef86fce4f8a87bdad74da3484b9605cb3b2b52cbbf20`  
		Last Modified: Tue, 28 Sep 2021 02:24:25 GMT  
		Size: 11.3 MB (11250636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50bcbe9fc6f4b839121363d75b4325536a717823ee2b2881b0247afe12fd6909`  
		Last Modified: Tue, 28 Sep 2021 02:24:58 GMT  
		Size: 55.9 MB (55916372 bytes)  
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
$ docker pull buildpack-deps@sha256:0079fcd37f046fdbc47f73c68e3301b7cb70947b2a248d6c3fc28008143759bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134696289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a755e8f1b32b86a7e3c3eb1702fb2c523aacade98b66f54fdbd1dc1631465c0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 05:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708d04ed929be54f33cfa94416648dcac9edd8c01746ecc6e250ce046aa54ac0`  
		Last Modified: Fri, 03 Sep 2021 07:09:38 GMT  
		Size: 58.8 MB (58849139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cc8ac782325035a5a46cf050e7b6611363ec94c8185f01f0b41b2d32a65f1720
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123150207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ee600655618ac729e88fc65d35e10aa6b00c909cee23ef5ab5b3c92ceee8f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:08:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f5b44618c39b6606db01fa6d460b6b7e1415b3a9c5a0b2f8b179c9b2c3fcfe`  
		Last Modified: Tue, 28 Sep 2021 02:16:05 GMT  
		Size: 54.0 MB (54049595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stretch`

```console
$ docker pull buildpack-deps@sha256:57d5d14748554b31c75a2e95e63c51e8cdfb24393e33c1431982123b7d0c2280
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
$ docker pull buildpack-deps@sha256:2b296bf57a668992a939c1ec7142f5988a567efef9697b95b16feb7259883bcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.2 MB (325213629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44762cca409b0b11184b876627c74da895f48b6035cf6876eeb55505ae5cf300`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:56:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fee6a1847b07f4933116726f66b9218dde8c59d1f7b94de92f9f0683571a362`  
		Last Modified: Tue, 28 Sep 2021 02:01:42 GMT  
		Size: 49.8 MB (49761752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cce3519052443b6eb66426edcfd7b395d8b97913e15256b77924964e8e6291`  
		Last Modified: Tue, 28 Sep 2021 02:02:22 GMT  
		Size: 214.4 MB (214431930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ef3ae3980658ba40e4a7d978df8752ee3c378406892f6b43418c56a6d6e7dc23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309141024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b006505cf9416d4acaf813ebff5a91b4d95ea360736beb0b6c213465a61fdd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:05 GMT
ADD file:f294a28ee9da17e8a289348f6b85aa865b9f1925aebadee96124e1d4a81c8401 in / 
# Tue, 28 Sep 2021 01:56:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 03:01:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:01:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:05:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a237f80116468b0593b0195bd02cdb78fb8bea8e44f206ec86fd61a9377d7a06`  
		Last Modified: Tue, 28 Sep 2021 02:13:48 GMT  
		Size: 44.1 MB (44091934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ebbdc0a8d4cc096a5c44b4a13000717d6e8dfeb21442b4b375e5d1b9327935`  
		Last Modified: Tue, 28 Sep 2021 03:17:12 GMT  
		Size: 10.4 MB (10350664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa304c7ee32783cf53bf48ea782d989a9874bd108e27ddae6d1adfb8b2eb3f`  
		Last Modified: Tue, 28 Sep 2021 03:17:09 GMT  
		Size: 4.2 MB (4161453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e7d03d992607295ece45259f5362cdffa8e3620933d03ee8100e7b58f2ced9`  
		Last Modified: Tue, 28 Sep 2021 03:17:59 GMT  
		Size: 48.0 MB (47984206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b03b8461331cb46d4d7d615cb7070035da816499bb75244a0b92e0c380dc2`  
		Last Modified: Tue, 28 Sep 2021 03:20:12 GMT  
		Size: 202.6 MB (202552767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7b8e69331b0f73e2b60e38a8cc2ac0918ed47b74b0c31b042fa9a56ebb89aa9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.2 MB (297172181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28f85dbdcf266bfca7d7f5f0acbce80a8946aeff5603bf47a8a765c08f73b697`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:46:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a914caeb151e7903d0d778c1ae44d420945c84af10ba750a5abfda6b9a99f65`  
		Last Modified: Fri, 01 Oct 2021 06:02:16 GMT  
		Size: 46.1 MB (46125924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed5634f1108d505f7a942e1c9e9129321f15004050ed21d2bf392b54e802feb`  
		Last Modified: Fri, 01 Oct 2021 06:04:17 GMT  
		Size: 195.0 MB (195049802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f5181b80a371eb18c642363bf22573aa28f809712d3eb9d52fdd8cd73b497a5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (306986243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9ca4a29cf7dc0349ab14654efaedcd290d15587838b9d2f6d7a5607be0625d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:21:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65cdaa18192aee6f9c254882a3a7f4e57f28681ee263e9fd155fefcd6d9a7e7f`  
		Last Modified: Tue, 28 Sep 2021 02:28:40 GMT  
		Size: 47.7 MB (47737758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445c016c41e0197a8c0587a7bdc804370e31412e49c9bd80ba6baa0b67074d1c`  
		Last Modified: Tue, 28 Sep 2021 02:29:20 GMT  
		Size: 201.8 MB (201758610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bb880314f7580d50f63ff28c7e3c47e3a1fd1b79cd10885c4280d567a8bd7a8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332749683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c905aaccf431950e830a05cc74895c752a57081f68d45d5dc7657bca959b1f3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:20 GMT
ADD file:489732b99c09023c7c1cf27548ad2ed82fd8c8411b95a4e155ebcae7546e563e in / 
# Tue, 28 Sep 2021 01:43:21 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:19:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:19:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:21:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:436d1bdb32419bd787d72deddc5b6a490ad25f93d42a585923767fae7698cb58`  
		Last Modified: Tue, 28 Sep 2021 01:53:31 GMT  
		Size: 46.1 MB (46097052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f065d2d31786c9f8f0c16da4c76f7636dd71179a92f3ee06802d878377006`  
		Last Modified: Tue, 28 Sep 2021 02:29:48 GMT  
		Size: 11.4 MB (11356018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eefa63906ef252cd12ee512cc28f58ea12d2b0854ad1f13b11af78ea5faff7d`  
		Last Modified: Tue, 28 Sep 2021 02:29:46 GMT  
		Size: 4.6 MB (4565007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2732564fa295ede3b01575a13f6d43177972b7e85de3a1f4f41866c7d611c04`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.3 MB (51265101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff272836df0bfc90314e2f8fb0eb0085d5ed17686bb6bcd7479e69073cabade0`  
		Last Modified: Tue, 28 Sep 2021 02:31:23 GMT  
		Size: 219.5 MB (219466505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stretch-curl`

```console
$ docker pull buildpack-deps@sha256:8c1faeb579deafbc6a453a0ccf4788be816da27ddd3f09bc7c63fddd1811172d
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
$ docker pull buildpack-deps@sha256:7f14fa6118ddab254eb9584f9d6464f97308059eef313f8aa2d9332de370f6e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61019947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026f5a52486111dfd84569e20d902d7cb134f2239af648ee071cef3502b4a2f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9bfdf437f588dd9ff11dd21891f40d3b70cf9cb234f71da1f7f6cd735ed586d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58604051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4c90ab387c8c56dbfafed822b87fe3193450d8635bd0c9247cb4500cea0030`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:05 GMT
ADD file:f294a28ee9da17e8a289348f6b85aa865b9f1925aebadee96124e1d4a81c8401 in / 
# Tue, 28 Sep 2021 01:56:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 03:01:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:01:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a237f80116468b0593b0195bd02cdb78fb8bea8e44f206ec86fd61a9377d7a06`  
		Last Modified: Tue, 28 Sep 2021 02:13:48 GMT  
		Size: 44.1 MB (44091934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ebbdc0a8d4cc096a5c44b4a13000717d6e8dfeb21442b4b375e5d1b9327935`  
		Last Modified: Tue, 28 Sep 2021 03:17:12 GMT  
		Size: 10.4 MB (10350664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa304c7ee32783cf53bf48ea782d989a9874bd108e27ddae6d1adfb8b2eb3f`  
		Last Modified: Tue, 28 Sep 2021 03:17:09 GMT  
		Size: 4.2 MB (4161453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:caea6201c9ee83e004d3dc8ac457f9d6029f0fe6a70188e5d719188022c4f519
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55996455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c023407259091d6cc756cfbdf78d84a1f5476a85ac967e8c55457a244eb9a824`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:954e54995ba061f8f12a7b1c5a3d352e8445cb1379b5dee8e3b61aead89ba056
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57489875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:410f50617ef6056fa47e2f6f85769a3ea11e18612c2e00c549e7eb7f5a75651e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:46ef012bbfc060f6c02c30dab11fbff22c64146722df2452c42c2d31ac5afc26
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62018077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd9a8ed29e31095fa7217eb4a4f4bced6b0f3751904e15d227fb5c9b7dff8083`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:20 GMT
ADD file:489732b99c09023c7c1cf27548ad2ed82fd8c8411b95a4e155ebcae7546e563e in / 
# Tue, 28 Sep 2021 01:43:21 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:19:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:19:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:436d1bdb32419bd787d72deddc5b6a490ad25f93d42a585923767fae7698cb58`  
		Last Modified: Tue, 28 Sep 2021 01:53:31 GMT  
		Size: 46.1 MB (46097052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f065d2d31786c9f8f0c16da4c76f7636dd71179a92f3ee06802d878377006`  
		Last Modified: Tue, 28 Sep 2021 02:29:48 GMT  
		Size: 11.4 MB (11356018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eefa63906ef252cd12ee512cc28f58ea12d2b0854ad1f13b11af78ea5faff7d`  
		Last Modified: Tue, 28 Sep 2021 02:29:46 GMT  
		Size: 4.6 MB (4565007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:1da383fbe3812219a3b9632c5c973b9ad46c6b560b45ded8c101352f886f6668
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
$ docker pull buildpack-deps@sha256:e042672f1de31e5ecc5bbf7df2a9eac7d1cc012a5a620ec3b0b5aa0ccae9e610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110781699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49daeb05d0974f360f43581a6691f08a5b169f1813fcc867a41293f40e7e4b5e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fee6a1847b07f4933116726f66b9218dde8c59d1f7b94de92f9f0683571a362`  
		Last Modified: Tue, 28 Sep 2021 02:01:42 GMT  
		Size: 49.8 MB (49761752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6a816944d99fd57824326754aafd407ee856c330276eb41194f40c7ad02ada82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106588257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf701630150bd83ffd677ef202986223117afacb24dc86cc90592ff66cefd33c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:05 GMT
ADD file:f294a28ee9da17e8a289348f6b85aa865b9f1925aebadee96124e1d4a81c8401 in / 
# Tue, 28 Sep 2021 01:56:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 03:01:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:01:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a237f80116468b0593b0195bd02cdb78fb8bea8e44f206ec86fd61a9377d7a06`  
		Last Modified: Tue, 28 Sep 2021 02:13:48 GMT  
		Size: 44.1 MB (44091934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ebbdc0a8d4cc096a5c44b4a13000717d6e8dfeb21442b4b375e5d1b9327935`  
		Last Modified: Tue, 28 Sep 2021 03:17:12 GMT  
		Size: 10.4 MB (10350664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa304c7ee32783cf53bf48ea782d989a9874bd108e27ddae6d1adfb8b2eb3f`  
		Last Modified: Tue, 28 Sep 2021 03:17:09 GMT  
		Size: 4.2 MB (4161453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e7d03d992607295ece45259f5362cdffa8e3620933d03ee8100e7b58f2ced9`  
		Last Modified: Tue, 28 Sep 2021 03:17:59 GMT  
		Size: 48.0 MB (47984206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2e3b13a826fc616ef225b08428059bbbe6fad1d52fab5bca1ed3745152a47070
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102122379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aafc37f0496b761630fecaf39bbcfd07af95e1926751d29862b817689908995d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a914caeb151e7903d0d778c1ae44d420945c84af10ba750a5abfda6b9a99f65`  
		Last Modified: Fri, 01 Oct 2021 06:02:16 GMT  
		Size: 46.1 MB (46125924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6e23d628f55e994db76f3e661ac0277e87952033aed50ecd98e038faafcbded3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105227633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6830661eeccc11f315c1e747ec4620621a116593bacb767fb179bc3631083db5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65cdaa18192aee6f9c254882a3a7f4e57f28681ee263e9fd155fefcd6d9a7e7f`  
		Last Modified: Tue, 28 Sep 2021 02:28:40 GMT  
		Size: 47.7 MB (47737758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6cb79acdbec5f1e26f1db9e369abbf339d784ba8355d2a264afbd67e67b31827
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113283178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9f8abca0902dbb9750099b01bf8c9f575e4a474a26ee4c4d5c24afc4bc20a7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:20 GMT
ADD file:489732b99c09023c7c1cf27548ad2ed82fd8c8411b95a4e155ebcae7546e563e in / 
# Tue, 28 Sep 2021 01:43:21 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:19:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:19:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:436d1bdb32419bd787d72deddc5b6a490ad25f93d42a585923767fae7698cb58`  
		Last Modified: Tue, 28 Sep 2021 01:53:31 GMT  
		Size: 46.1 MB (46097052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f065d2d31786c9f8f0c16da4c76f7636dd71179a92f3ee06802d878377006`  
		Last Modified: Tue, 28 Sep 2021 02:29:48 GMT  
		Size: 11.4 MB (11356018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eefa63906ef252cd12ee512cc28f58ea12d2b0854ad1f13b11af78ea5faff7d`  
		Last Modified: Tue, 28 Sep 2021 02:29:46 GMT  
		Size: 4.6 MB (4565007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2732564fa295ede3b01575a13f6d43177972b7e85de3a1f4f41866c7d611c04`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.3 MB (51265101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:448b2c42cadb43e92092f29207cdce0a01d084199a51bbb585cd0b13f6c1a5b9
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
$ docker pull buildpack-deps@sha256:efb1a54d6562d3ae971617eecbdf896ecefb73b5797344583caaf1776dea4162
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.0 MB (325002318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7599afc8b9104ad6cb6c92ab4734d15c10c7c2ef8a132422ef3ba88bdb7d657`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:24:18 GMT
ADD file:43a49c0ac74573bd560d191480bb30b2950f21ec76e9b3bdffdf73eb74628c50 in / 
# Tue, 28 Sep 2021 01:24:19 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:53:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e3fead4ded84f6449ee17b9deabf1e9144512edf86da02e0f93fbf81df3fd6fb`  
		Last Modified: Tue, 28 Sep 2021 01:31:21 GMT  
		Size: 55.7 MB (55702084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b8f6b86e3a84210feef982a4953fcc1b15003e51b2fb7b861ae18f18e914f`  
		Last Modified: Tue, 28 Sep 2021 02:00:14 GMT  
		Size: 5.2 MB (5181002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8e6a19825e33b3ebf505b0ae79fe6cf49091e693c4d8971abde683746f445`  
		Last Modified: Tue, 28 Sep 2021 02:00:15 GMT  
		Size: 10.9 MB (10900815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8600ac737a89c73eb8b73b618e244774719a3cc4caaa7325dbf6d6e04706ed`  
		Last Modified: Tue, 28 Sep 2021 02:00:34 GMT  
		Size: 55.7 MB (55730660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258a146afb1bcd19c174d0f8eb33a43c049127a82f2e1bffead6c9f03cfb84b3`  
		Last Modified: Tue, 28 Sep 2021 02:01:13 GMT  
		Size: 197.5 MB (197487757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fe1b2fc6392319cf2a844c4b7fa0da4838f388f6e2d2413b66e14c313f4128ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297514333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2959efdc159d70ab1117f74eb0e80050f090ee66ca49e693a0910f7b53d397da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:54:15 GMT
ADD file:bcd1f002a3a38be54eed5da9d7a2e3822ecdf63ba82a59931124557d1f97007b in / 
# Tue, 28 Sep 2021 01:54:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:00:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4bd09bbbe96b85664474243c833d73be517c92e7172b8d740101438ee21d5561`  
		Last Modified: Tue, 28 Sep 2021 02:11:21 GMT  
		Size: 53.2 MB (53207754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70c595ca5d004271509bd463bf50b3dc2d385630237ea30f5e4936f414a9b7`  
		Last Modified: Tue, 28 Sep 2021 03:14:06 GMT  
		Size: 5.1 MB (5088778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526e46f7c293bb67a0ab1c2bbce082b844bc145c04bb54e588fa2146980730af`  
		Last Modified: Tue, 28 Sep 2021 03:14:08 GMT  
		Size: 10.6 MB (10606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e39f8615ccdb2930517a3daed84ef9540d8f34f9a6a2447c42b05dd7e6d93`  
		Last Modified: Tue, 28 Sep 2021 03:14:58 GMT  
		Size: 53.4 MB (53435709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6669aa2732e897328c267a2d8b14ff0b2ba22b9e012b47944f5d6679f6c4f6`  
		Last Modified: Tue, 28 Sep 2021 03:16:54 GMT  
		Size: 175.2 MB (175175214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ce12648e9765e996822d2b6c0bffecc95bc1f445f4f22addb576279d8e9101b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.9 MB (284880273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927850025a048f1566f31c32e4eaac519e826ffee7f84a15e5aa18f57d9740da`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:06:54 GMT
ADD file:d9a8e8032b2f681adb1be7e9dfacdf1838167068f97e052c3173223cb1d2c303 in / 
# Thu, 30 Sep 2021 18:06:55 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:39:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:40:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:42:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90a9a2564a394330c4b6320f33e007b55c6f40a9006b85fe17fa2ed9fe260cee`  
		Last Modified: Thu, 30 Sep 2021 18:23:58 GMT  
		Size: 50.8 MB (50822436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f06eb4253b6bc5ee446db688fa4b3052465b6890ef2f7157f1a345118360e`  
		Last Modified: Fri, 01 Oct 2021 05:58:43 GMT  
		Size: 4.9 MB (4946836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b50232f315931bda767b06cac42d2688e34c66a06877f32bc9bdb103575e50`  
		Last Modified: Fri, 01 Oct 2021 05:58:45 GMT  
		Size: 10.2 MB (10249907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6189d745298f970340832970521c77f9df62fa058d6a498469ecaac7cdd9e`  
		Last Modified: Fri, 01 Oct 2021 05:59:31 GMT  
		Size: 51.4 MB (51371485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626fd6dc0bb62c7a429172fe52c51d82255b7b0b7e9cd7a377c2ae9b272e0e41`  
		Last Modified: Fri, 01 Oct 2021 06:01:16 GMT  
		Size: 167.5 MB (167489609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:524d70b0c8fb2f1a271185979c1d4d275f123c70b768ccf86467bb1a62b2a6f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.7 MB (316687005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41db0b469d56879a649dec194de46b605e0a658813fe6140127b8d6aa23e0c01`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:20 GMT
ADD file:714781c9fce1c450e5f9cc5529167eaa33fdff089ab48a1dcac0a813d768be30 in / 
# Tue, 28 Sep 2021 01:42:20 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:18:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:19:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd53cd90ab526d30a2e414c3951333db1b1b814fe009621017a07b5eea3cad0f`  
		Last Modified: Tue, 28 Sep 2021 01:51:10 GMT  
		Size: 54.7 MB (54725302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945f16b6588acc2f82d3f0371dd15803436b26df556a96921d086d035a320cd`  
		Last Modified: Tue, 28 Sep 2021 02:27:09 GMT  
		Size: 5.2 MB (5169449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba2c20fe4248de05c9d215800868bdf9800fbc648f764ff6aabe878e837cf5e`  
		Last Modified: Tue, 28 Sep 2021 02:27:10 GMT  
		Size: 10.9 MB (10899138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb38129bed7931b18a48dcbaa75e8350149907c137d95496ab9e8fbb32aa6d6`  
		Last Modified: Tue, 28 Sep 2021 02:27:30 GMT  
		Size: 55.9 MB (55867003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0836b49579e1ee352ee58e9b6c1320c3328fe03fb098d7a2d4d7c1f5bfbdc`  
		Last Modified: Tue, 28 Sep 2021 02:28:07 GMT  
		Size: 190.0 MB (190026113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d626cefcea6ec3c6654f1b94b8db3fda2595ec1b38a111dec9a79a2ce72caf31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.3 MB (328291208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924bd8ae3a1df8c572a1ebfb6a23252af19a419fd4759ce71b78689e68e85f0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:17 GMT
ADD file:07dfd2960f3649fbe7a701ad0b551f48b4815ff5eabaefe7aaf62e770435e5f2 in / 
# Tue, 28 Sep 2021 01:42:18 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ed4b6e2f624e3ac187bdfdafce616f76387ede25afbec70c204c9d6300d2e0`  
		Last Modified: Tue, 28 Sep 2021 01:52:05 GMT  
		Size: 56.7 MB (56733325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a4c8e238708f81b44eb4ba40b5c8f710f262c0c1745ffcdb299c8387dc061`  
		Last Modified: Tue, 28 Sep 2021 02:27:58 GMT  
		Size: 5.3 MB (5312381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e976216252ce09cde1548cf4c9a4e367e1cc4c4fee46d9a25408720edd938df`  
		Last Modified: Tue, 28 Sep 2021 02:27:59 GMT  
		Size: 11.3 MB (11282013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6ebec24d20e38092d845932f91387b27fb11b3740ba554966788b972768db`  
		Last Modified: Tue, 28 Sep 2021 02:28:26 GMT  
		Size: 57.2 MB (57151017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cedae44a9ec227abfbabebaeb53f31f845d9886fed86f7eb2a35f62e398dcb2`  
		Last Modified: Tue, 28 Sep 2021 02:29:30 GMT  
		Size: 197.8 MB (197812472 bytes)  
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
$ docker pull buildpack-deps@sha256:6ebc81f3c1a34e2586abf1f4fd150c75d8459eb2b0c040dfc336ca955f1d88bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334296089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7572ef35d6da465015e1104284fd7fb00fa202aea43ba80271f3808fec3a0fa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:05:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a95302a54a7fa51cdd0cd0117968b05d9f71d3c40eafe66873816a3b43ba14`  
		Last Modified: Fri, 03 Sep 2021 07:14:06 GMT  
		Size: 5.4 MB (5422617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da11fea16e40da1a9b66dee60a49dee27fffb468c778b12670ed59f3cd11837`  
		Last Modified: Fri, 03 Sep 2021 07:14:07 GMT  
		Size: 11.7 MB (11650959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd39c289a3baa1fff8358db49e63fac02746752ceae177b4b7a19642ba640995`  
		Last Modified: Fri, 03 Sep 2021 07:14:30 GMT  
		Size: 60.1 MB (60114890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f3c7ffcb3f63c765e1e528a5bcf0e279cc85c94b4feb1db90889365457802b`  
		Last Modified: Fri, 03 Sep 2021 07:15:16 GMT  
		Size: 197.6 MB (197573551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82a5f039001206c34e9980c0b125465287f9eae25b375c0f6208ea0eda1102a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331495706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc78af4ec6bd0acab27b6933fd88cc1d5cf6518dd1357312a98bc90d3db091c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:14:19 GMT
ADD file:c8ff49735749af794fa2a6ca03eb4ac0fb66dffd4ead8d9902ee04483db97aff in / 
# Tue, 28 Sep 2021 02:14:22 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:56:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:58:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:12:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f903d1b59452679ad13935f22aa7eb73ffa71398303161a843221e41855e5bce`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.5 MB (51531137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec6ba981ab80c88267fed9b741a2a2ace934d0bb03930338f0126518120a416`  
		Last Modified: Tue, 28 Sep 2021 03:35:59 GMT  
		Size: 5.0 MB (4997888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736a4b194f9d38dde15b4c734cd79228a198fb0314eed4526e0135d4254874b4`  
		Last Modified: Tue, 28 Sep 2021 03:36:02 GMT  
		Size: 10.3 MB (10314682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36c310fdfaed216b6a43fd07fe77c729b8d8abfb8772e830cda42b0cca7024f`  
		Last Modified: Tue, 28 Sep 2021 03:38:07 GMT  
		Size: 51.8 MB (51783989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36eab1b54c6853b466e19a2e6ec879edac6a7bd66f7175578c5f0b0fb23b89b`  
		Last Modified: Tue, 28 Sep 2021 03:43:51 GMT  
		Size: 212.9 MB (212868010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a3ec81993a54920402b059f89de3f61e3753d964f3f5b7651dafb27db2c64287
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.2 MB (298164614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3477144a143fac537af824ce79d485fab57e51a91aeeac7bcb59b9167ecdcf8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:11 GMT
ADD file:797f09f7e25e9194e8845d5783ab9078062d7caad45c75201a4ad699145b1305 in / 
# Tue, 28 Sep 2021 01:44:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:12:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8463103c03054c6dd4bf0a387d658bdf4d12ddbb0d87ce07eaa15b2b13f1d733`  
		Last Modified: Tue, 28 Sep 2021 01:50:20 GMT  
		Size: 54.0 MB (53953837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32362b87984c1bba14b0f80546944827886c7cc7accd0865b4ccc7f34a9f3b8a`  
		Last Modified: Tue, 28 Sep 2021 02:17:31 GMT  
		Size: 5.2 MB (5165065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aadefacf33492b3a74622a982ea04f1605a554feeaa2ef0abdd214a94280744`  
		Last Modified: Tue, 28 Sep 2021 02:17:32 GMT  
		Size: 10.8 MB (10793806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217921cacc4173d4ddbf287e61dbfb88ee91ded7acf28b93d6b7db50ca7ca75`  
		Last Modified: Tue, 28 Sep 2021 02:17:48 GMT  
		Size: 55.2 MB (55159873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e09838e2681cac8b641b6a8bd947c86ce543872a81967a64ab4cfd78c35c8f3`  
		Last Modified: Tue, 28 Sep 2021 02:18:13 GMT  
		Size: 173.1 MB (173092033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:0ff93d51e83675d401c67c79e63e476d548b325b652aab348e14f616711390bf
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
$ docker pull buildpack-deps@sha256:876cfe58c039fd813ff318d4e53e2707c884cb7b8c7952464dcf2e27cca17b5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71783901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:506d6fd65061be41934c131b48e3c840c7e841b27244c6d3c657f0c4008db311`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:24:18 GMT
ADD file:43a49c0ac74573bd560d191480bb30b2950f21ec76e9b3bdffdf73eb74628c50 in / 
# Tue, 28 Sep 2021 01:24:19 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:53:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e3fead4ded84f6449ee17b9deabf1e9144512edf86da02e0f93fbf81df3fd6fb`  
		Last Modified: Tue, 28 Sep 2021 01:31:21 GMT  
		Size: 55.7 MB (55702084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b8f6b86e3a84210feef982a4953fcc1b15003e51b2fb7b861ae18f18e914f`  
		Last Modified: Tue, 28 Sep 2021 02:00:14 GMT  
		Size: 5.2 MB (5181002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8e6a19825e33b3ebf505b0ae79fe6cf49091e693c4d8971abde683746f445`  
		Last Modified: Tue, 28 Sep 2021 02:00:15 GMT  
		Size: 10.9 MB (10900815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e87ec835044393c77ab96a3c4fbf5d4f999fe5c2aea983a35c8a24f333106911
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68903410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9a5d7085c78c1d80020d21fdc2bfcb29fe53b22a93b588e0d67af242ef17aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:54:15 GMT
ADD file:bcd1f002a3a38be54eed5da9d7a2e3822ecdf63ba82a59931124557d1f97007b in / 
# Tue, 28 Sep 2021 01:54:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4bd09bbbe96b85664474243c833d73be517c92e7172b8d740101438ee21d5561`  
		Last Modified: Tue, 28 Sep 2021 02:11:21 GMT  
		Size: 53.2 MB (53207754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70c595ca5d004271509bd463bf50b3dc2d385630237ea30f5e4936f414a9b7`  
		Last Modified: Tue, 28 Sep 2021 03:14:06 GMT  
		Size: 5.1 MB (5088778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526e46f7c293bb67a0ab1c2bbce082b844bc145c04bb54e588fa2146980730af`  
		Last Modified: Tue, 28 Sep 2021 03:14:08 GMT  
		Size: 10.6 MB (10606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ec123566e37f91cf7dc999a213d362dfbf1413d9ac4ad6232d3bee77c01ca4c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66019179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f8848536df00d83694de40159ebe8595caf2bf001797c4d47dea972c82eb99`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:06:54 GMT
ADD file:d9a8e8032b2f681adb1be7e9dfacdf1838167068f97e052c3173223cb1d2c303 in / 
# Thu, 30 Sep 2021 18:06:55 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:39:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:90a9a2564a394330c4b6320f33e007b55c6f40a9006b85fe17fa2ed9fe260cee`  
		Last Modified: Thu, 30 Sep 2021 18:23:58 GMT  
		Size: 50.8 MB (50822436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f06eb4253b6bc5ee446db688fa4b3052465b6890ef2f7157f1a345118360e`  
		Last Modified: Fri, 01 Oct 2021 05:58:43 GMT  
		Size: 4.9 MB (4946836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b50232f315931bda767b06cac42d2688e34c66a06877f32bc9bdb103575e50`  
		Last Modified: Fri, 01 Oct 2021 05:58:45 GMT  
		Size: 10.2 MB (10249907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3cacb2497db42e4160cef77ad2ebed9249918ab55507fe1ca75a48a3b384ec58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70793889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e7747dd728e45e46bfbd2d710d52a2e130eae3b33fc78392bb548807e00939a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:20 GMT
ADD file:714781c9fce1c450e5f9cc5529167eaa33fdff089ab48a1dcac0a813d768be30 in / 
# Tue, 28 Sep 2021 01:42:20 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:18:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bd53cd90ab526d30a2e414c3951333db1b1b814fe009621017a07b5eea3cad0f`  
		Last Modified: Tue, 28 Sep 2021 01:51:10 GMT  
		Size: 54.7 MB (54725302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945f16b6588acc2f82d3f0371dd15803436b26df556a96921d086d035a320cd`  
		Last Modified: Tue, 28 Sep 2021 02:27:09 GMT  
		Size: 5.2 MB (5169449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba2c20fe4248de05c9d215800868bdf9800fbc648f764ff6aabe878e837cf5e`  
		Last Modified: Tue, 28 Sep 2021 02:27:10 GMT  
		Size: 10.9 MB (10899138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:138dafec4d1ffcacfb0d88e1ec201cefc8e953f8e5e2b566dc381409fe1df3ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73327719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0a6347fe9bfe440f7f7bee5c7628ea6b41d05955bcfc1e8025699c51acd5cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:17 GMT
ADD file:07dfd2960f3649fbe7a701ad0b551f48b4815ff5eabaefe7aaf62e770435e5f2 in / 
# Tue, 28 Sep 2021 01:42:18 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e7ed4b6e2f624e3ac187bdfdafce616f76387ede25afbec70c204c9d6300d2e0`  
		Last Modified: Tue, 28 Sep 2021 01:52:05 GMT  
		Size: 56.7 MB (56733325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a4c8e238708f81b44eb4ba40b5c8f710f262c0c1745ffcdb299c8387dc061`  
		Last Modified: Tue, 28 Sep 2021 02:27:58 GMT  
		Size: 5.3 MB (5312381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e976216252ce09cde1548cf4c9a4e367e1cc4c4fee46d9a25408720edd938df`  
		Last Modified: Tue, 28 Sep 2021 02:27:59 GMT  
		Size: 11.3 MB (11282013 bytes)  
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
$ docker pull buildpack-deps@sha256:f686e9380a7ddf6bd2900de9f550ad307efaec5625ed23c223f0bc49e5b4eb11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76607648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:458f349d2522ffbef1b1dc6a5f6f49b9c4cec344f768cabcf7a36baec2536acd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a95302a54a7fa51cdd0cd0117968b05d9f71d3c40eafe66873816a3b43ba14`  
		Last Modified: Fri, 03 Sep 2021 07:14:06 GMT  
		Size: 5.4 MB (5422617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da11fea16e40da1a9b66dee60a49dee27fffb468c778b12670ed59f3cd11837`  
		Last Modified: Fri, 03 Sep 2021 07:14:07 GMT  
		Size: 11.7 MB (11650959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0a6ecb3329f5b8d000b8e6e5e10ff4a66e34755b3f2f51f80bd52ee98f763704
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66843707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ea89476054b4f64f3f7013eaa3d25bfdb786c2b2a83de0b362dee8da2c37c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:14:19 GMT
ADD file:c8ff49735749af794fa2a6ca03eb4ac0fb66dffd4ead8d9902ee04483db97aff in / 
# Tue, 28 Sep 2021 02:14:22 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:56:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:58:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f903d1b59452679ad13935f22aa7eb73ffa71398303161a843221e41855e5bce`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.5 MB (51531137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec6ba981ab80c88267fed9b741a2a2ace934d0bb03930338f0126518120a416`  
		Last Modified: Tue, 28 Sep 2021 03:35:59 GMT  
		Size: 5.0 MB (4997888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736a4b194f9d38dde15b4c734cd79228a198fb0314eed4526e0135d4254874b4`  
		Last Modified: Tue, 28 Sep 2021 03:36:02 GMT  
		Size: 10.3 MB (10314682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b734c11fedc4319a44595c49e3541d7a69e4c3bde2e5b12f1082ed915b59a556
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69912708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f80b8e561ff61c6a6d9bd4db8e89f29950f901bce96b85d1b662f440d23f5c4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:11 GMT
ADD file:797f09f7e25e9194e8845d5783ab9078062d7caad45c75201a4ad699145b1305 in / 
# Tue, 28 Sep 2021 01:44:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8463103c03054c6dd4bf0a387d658bdf4d12ddbb0d87ce07eaa15b2b13f1d733`  
		Last Modified: Tue, 28 Sep 2021 01:50:20 GMT  
		Size: 54.0 MB (53953837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32362b87984c1bba14b0f80546944827886c7cc7accd0865b4ccc7f34a9f3b8a`  
		Last Modified: Tue, 28 Sep 2021 02:17:31 GMT  
		Size: 5.2 MB (5165065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aadefacf33492b3a74622a982ea04f1605a554feeaa2ef0abdd214a94280744`  
		Last Modified: Tue, 28 Sep 2021 02:17:32 GMT  
		Size: 10.8 MB (10793806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:20d37c1005ae07c16a77312fa565ac3990399a169d5feac9e5368d43845087eb
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
$ docker pull buildpack-deps@sha256:0abecfd3831c9b69c830ddadefd33d2ab68555ce081e9eb05c0cd44c2bd0b153
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127514561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3557e30291bd8748d13ae0a1df0419cd78a45eddb9d3e6f26d3ab66dcfe91cb6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:24:18 GMT
ADD file:43a49c0ac74573bd560d191480bb30b2950f21ec76e9b3bdffdf73eb74628c50 in / 
# Tue, 28 Sep 2021 01:24:19 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:53:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e3fead4ded84f6449ee17b9deabf1e9144512edf86da02e0f93fbf81df3fd6fb`  
		Last Modified: Tue, 28 Sep 2021 01:31:21 GMT  
		Size: 55.7 MB (55702084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b8f6b86e3a84210feef982a4953fcc1b15003e51b2fb7b861ae18f18e914f`  
		Last Modified: Tue, 28 Sep 2021 02:00:14 GMT  
		Size: 5.2 MB (5181002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8e6a19825e33b3ebf505b0ae79fe6cf49091e693c4d8971abde683746f445`  
		Last Modified: Tue, 28 Sep 2021 02:00:15 GMT  
		Size: 10.9 MB (10900815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8600ac737a89c73eb8b73b618e244774719a3cc4caaa7325dbf6d6e04706ed`  
		Last Modified: Tue, 28 Sep 2021 02:00:34 GMT  
		Size: 55.7 MB (55730660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4cd97ee516ec215abbd5b3ac462930d5ce96d603e843d9e3c16f2f89b92fa7cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122339119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5cd7b304c5341441e3c2c40eeb8cb460e041906d3883be6d82bebca44295a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:54:15 GMT
ADD file:bcd1f002a3a38be54eed5da9d7a2e3822ecdf63ba82a59931124557d1f97007b in / 
# Tue, 28 Sep 2021 01:54:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4bd09bbbe96b85664474243c833d73be517c92e7172b8d740101438ee21d5561`  
		Last Modified: Tue, 28 Sep 2021 02:11:21 GMT  
		Size: 53.2 MB (53207754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70c595ca5d004271509bd463bf50b3dc2d385630237ea30f5e4936f414a9b7`  
		Last Modified: Tue, 28 Sep 2021 03:14:06 GMT  
		Size: 5.1 MB (5088778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526e46f7c293bb67a0ab1c2bbce082b844bc145c04bb54e588fa2146980730af`  
		Last Modified: Tue, 28 Sep 2021 03:14:08 GMT  
		Size: 10.6 MB (10606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e39f8615ccdb2930517a3daed84ef9540d8f34f9a6a2447c42b05dd7e6d93`  
		Last Modified: Tue, 28 Sep 2021 03:14:58 GMT  
		Size: 53.4 MB (53435709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7a0d1efa6e01ca27a3c8b6ce00256addbf9e6a87727403382b3bb85867f46245
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.4 MB (117390664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30ca238d4f10dd5e6d87c27eca2dbd6a378f05ea84b11758f19a8a33cb2b27e0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:06:54 GMT
ADD file:d9a8e8032b2f681adb1be7e9dfacdf1838167068f97e052c3173223cb1d2c303 in / 
# Thu, 30 Sep 2021 18:06:55 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:39:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:40:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90a9a2564a394330c4b6320f33e007b55c6f40a9006b85fe17fa2ed9fe260cee`  
		Last Modified: Thu, 30 Sep 2021 18:23:58 GMT  
		Size: 50.8 MB (50822436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f06eb4253b6bc5ee446db688fa4b3052465b6890ef2f7157f1a345118360e`  
		Last Modified: Fri, 01 Oct 2021 05:58:43 GMT  
		Size: 4.9 MB (4946836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b50232f315931bda767b06cac42d2688e34c66a06877f32bc9bdb103575e50`  
		Last Modified: Fri, 01 Oct 2021 05:58:45 GMT  
		Size: 10.2 MB (10249907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6189d745298f970340832970521c77f9df62fa058d6a498469ecaac7cdd9e`  
		Last Modified: Fri, 01 Oct 2021 05:59:31 GMT  
		Size: 51.4 MB (51371485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3b8e35be88c4a91d8413351d8c621c65496a35142b7b0e4c7f97c9ade9a3f078
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126660892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51de9ff568cdc9fcc755ffef64b86ff3ac486276a65accf31b79039ae9812ff3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:20 GMT
ADD file:714781c9fce1c450e5f9cc5529167eaa33fdff089ab48a1dcac0a813d768be30 in / 
# Tue, 28 Sep 2021 01:42:20 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:18:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd53cd90ab526d30a2e414c3951333db1b1b814fe009621017a07b5eea3cad0f`  
		Last Modified: Tue, 28 Sep 2021 01:51:10 GMT  
		Size: 54.7 MB (54725302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945f16b6588acc2f82d3f0371dd15803436b26df556a96921d086d035a320cd`  
		Last Modified: Tue, 28 Sep 2021 02:27:09 GMT  
		Size: 5.2 MB (5169449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba2c20fe4248de05c9d215800868bdf9800fbc648f764ff6aabe878e837cf5e`  
		Last Modified: Tue, 28 Sep 2021 02:27:10 GMT  
		Size: 10.9 MB (10899138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb38129bed7931b18a48dcbaa75e8350149907c137d95496ab9e8fbb32aa6d6`  
		Last Modified: Tue, 28 Sep 2021 02:27:30 GMT  
		Size: 55.9 MB (55867003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:06b714e4afeeaf5a5ea67a0e493064f71329a8a8a9b01d40f8d5b0bc87b04e16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130478736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42882d2ad744ca8f780a934a350b370b9184646c9ba3a6fe87ec9da44ee3ae33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:17 GMT
ADD file:07dfd2960f3649fbe7a701ad0b551f48b4815ff5eabaefe7aaf62e770435e5f2 in / 
# Tue, 28 Sep 2021 01:42:18 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ed4b6e2f624e3ac187bdfdafce616f76387ede25afbec70c204c9d6300d2e0`  
		Last Modified: Tue, 28 Sep 2021 01:52:05 GMT  
		Size: 56.7 MB (56733325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a4c8e238708f81b44eb4ba40b5c8f710f262c0c1745ffcdb299c8387dc061`  
		Last Modified: Tue, 28 Sep 2021 02:27:58 GMT  
		Size: 5.3 MB (5312381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e976216252ce09cde1548cf4c9a4e367e1cc4c4fee46d9a25408720edd938df`  
		Last Modified: Tue, 28 Sep 2021 02:27:59 GMT  
		Size: 11.3 MB (11282013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6ebec24d20e38092d845932f91387b27fb11b3740ba554966788b972768db`  
		Last Modified: Tue, 28 Sep 2021 02:28:26 GMT  
		Size: 57.2 MB (57151017 bytes)  
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
$ docker pull buildpack-deps@sha256:a5c418dd1d0e473e559b3a703a9e40757ead45790002b65bfc2bb736e31a077f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136722538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf7cb6d58a64ecbd4e666e5dc9905f0bb6786a021d2c2d955cf233ab37f7ef`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a95302a54a7fa51cdd0cd0117968b05d9f71d3c40eafe66873816a3b43ba14`  
		Last Modified: Fri, 03 Sep 2021 07:14:06 GMT  
		Size: 5.4 MB (5422617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da11fea16e40da1a9b66dee60a49dee27fffb468c778b12670ed59f3cd11837`  
		Last Modified: Fri, 03 Sep 2021 07:14:07 GMT  
		Size: 11.7 MB (11650959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd39c289a3baa1fff8358db49e63fac02746752ceae177b4b7a19642ba640995`  
		Last Modified: Fri, 03 Sep 2021 07:14:30 GMT  
		Size: 60.1 MB (60114890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:f39ef8a4165175de61f83dc3174aa76194916a15f5137f0e1bf51f5b86cc7ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118627696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1485f61f1c24b7322dfb4b732919e5862c78ff48a917cb91cdae8e09b3e50e75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:14:19 GMT
ADD file:c8ff49735749af794fa2a6ca03eb4ac0fb66dffd4ead8d9902ee04483db97aff in / 
# Tue, 28 Sep 2021 02:14:22 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:56:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:58:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f903d1b59452679ad13935f22aa7eb73ffa71398303161a843221e41855e5bce`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.5 MB (51531137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec6ba981ab80c88267fed9b741a2a2ace934d0bb03930338f0126518120a416`  
		Last Modified: Tue, 28 Sep 2021 03:35:59 GMT  
		Size: 5.0 MB (4997888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736a4b194f9d38dde15b4c734cd79228a198fb0314eed4526e0135d4254874b4`  
		Last Modified: Tue, 28 Sep 2021 03:36:02 GMT  
		Size: 10.3 MB (10314682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36c310fdfaed216b6a43fd07fe77c729b8d8abfb8772e830cda42b0cca7024f`  
		Last Modified: Tue, 28 Sep 2021 03:38:07 GMT  
		Size: 51.8 MB (51783989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:32b95e6cbcac8947758c681cc7c6e8995abc6b755ad8853070676f621ccf168b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125072581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d879c30c528729314fbb2e692c8bfb507fd458de13198f1af75a320ad2fd8d7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:11 GMT
ADD file:797f09f7e25e9194e8845d5783ab9078062d7caad45c75201a4ad699145b1305 in / 
# Tue, 28 Sep 2021 01:44:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8463103c03054c6dd4bf0a387d658bdf4d12ddbb0d87ce07eaa15b2b13f1d733`  
		Last Modified: Tue, 28 Sep 2021 01:50:20 GMT  
		Size: 54.0 MB (53953837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32362b87984c1bba14b0f80546944827886c7cc7accd0865b4ccc7f34a9f3b8a`  
		Last Modified: Tue, 28 Sep 2021 02:17:31 GMT  
		Size: 5.2 MB (5165065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aadefacf33492b3a74622a982ea04f1605a554feeaa2ef0abdd214a94280744`  
		Last Modified: Tue, 28 Sep 2021 02:17:32 GMT  
		Size: 10.8 MB (10793806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217921cacc4173d4ddbf287e61dbfb88ee91ded7acf28b93d6b7db50ca7ca75`  
		Last Modified: Tue, 28 Sep 2021 02:17:48 GMT  
		Size: 55.2 MB (55159873 bytes)  
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
